# 6주차 내용 정리

우리는 보통 파일을 수정하면 바꾸기전에 파일들을 저장해둔다.<br>
하지만 이름을 계속 바꾸면서 저장하다보면 용량낭비가 일어나면서 나중에는 버전 체크가 힘들어진다.<br>

### Changes vs Snapshot
- 전자는 버전이 바뀔때마다 바뀌는 부분만 저장한다.
- 후자는 버전이 바뀌더라도 이전 버전의 파일들을 저장하고 있다.

### Local, Centralized, Distributed

- Local: 내 컴퓨터에서만 파일들을 저장해 놓는 경우<br>
- Centralized: 중앙화된 서버에서 파일들을 다운로드 업로드 할 수 있는 경우<br>
- Distributed: 서버, 서버를 이용하는 컴퓨터들이 각자 상호작용하여 서버 컴퓨터가 다운되도 파일들을 다운로드, 업로드 할 수 있다.

### Three States in Git
- Modified: 작업전
- Staged: 작업후 수정된버전 (아무리 수정해도 Commit되지 않으면 바뀐건지 다른 사람이 알 수 없음)
- Committed: 관리자가 승인하여 서버에 올라간 버전

### Git 사용하기

- Global level: 보통 유저들이 사용하는 단계

- #### git 명령어들
- - git config --global ... : 사용자 이름과 이메일등 유저정보 수정
  - git init: 디렉토리 만들기
  - git status: 현재 디렉토리 상태 확인
  - git add 파일이름: add된 파일은 commit, add뒤에 .을 쓰면 폴더 안에 있는 모든 파일 commit
  - git rm --cached 파일이름: commit된 파일을 uncommit
  - ignore: commit하지 않을 파일을 설정 할 수 있음
  - git commit -m "commit message": commit 할 메시지를 추가
  - git branch: 현재 branch이름을 볼 수 있음 branch뒤에 현재 branch 바꿀 branch이름을 넣으면 바꾸기 가능
