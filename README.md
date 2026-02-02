# GitHub를 이용한 CI/CD workflow 맛보기

git을 이용하는 방법은 간단하게 자신이 만드는 프로그램의 버전 관리에 지나지 않습니다.   
진정한 git의 유용성은 다른 사람들과 함께 GitHub를 사용할 때 나옵니다.   

이 리포지토리에서는 EoN 동아리의 부원들끼리 어떤 프로그램을 만들면서 발생할 상황을 시뮬레이션 하듯이 진행합니다.

1) 자신의 Repository로 해당 git_prac 리포 forking
2) vscode의 Terminal에서 git clone을 이용해 로컬로 복제
3) Upstream 등록, git remote add upstream https://github.com/KyonggiEoN/git_prac
4) GitHub Issues 탭에서 맡을 문제 확인하고, 댓글 남겨서 작업 알리기
5) 새로운 Branch, fix/{name} 으로 작업 Branch 변경
   git switch -C feature/issue-1-idamin 처럼 {이슈+이름}
7) LLMs를 이용하는 등으로 미리 만들어진 문제있는 프로그램 수정
  수정하고 프로그램 실행해서 정상 동작 확인 필수(유닛 테스트 과정)
9) add, commit, git pull upstream main (Conflict 발생하면 잘 해결해보기)
10) git push origin feature/{branch_name}
11) Pull Request를 upstream(git_prac)으로 보내기
12) Code Review, 모든 PR은 Approve 두 개를 받아야 Merge되도록 만들 예정
