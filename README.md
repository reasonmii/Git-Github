Git, Github, Git Immersion
- github is where you can collaborate with others

<b>git commit message convention</b>
- 기본 구성 : type:subject, body, footer
- type
  - feat : 새로운 기능 추가
  - fix : 버그 수정
  - docs : 문서 수정
  - style : code formatting, semicolon 누락, 코드 변경이 없는 경우
  - refactor : refactoring production code
    - ※ refactoring : 결과의 변경 없이 코드 구조 재조정함 (가독성↑, 유지보수 굿)
  - test : adding/refactoring test code (no production code change)
  - chore : updating build tasks, package manager configs (no production code change)
- subject : 50자 내, 마침표X, 현재시제 사용, 명령어로 작성
- body (optional)
  - commit 부연설명
  - 72자 내, 제목과 구분하여 한 칸 띄어 작성
- footer (optional)
  - issue tracker id 작성할 때 사용

<b>git commit으로 issue 종료하기</b>
- commit message에 종료 keyword, issue no. 기입하면 push 할 때 해당 이슈 자동으로 종료 처리
- 종료 keyword : close, closes, closed, fix, fixes, fixed, resolve, resolves, resolved
- ex) `git commit -m "fixed XSS Vulnerability - #20"`
- 여러 개 이슈 모두 종료하기 : `git commit -m "fixed XSS Vulnerability - #20", #21, #23`
- 다른 repository의 이슈 종료하기 : `git commit -m "close issue #21 #22 and [other_repo_path]#10"

<b>.gitignore</b>
- git push 하고 싶지 않은 파일명들 입력
- 작업 중인 파일을 전부 github에 업로드 하면 용량이 크니, 특정 파일들은 업로드 하지 않기 위함

