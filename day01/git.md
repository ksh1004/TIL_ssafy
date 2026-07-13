# GIT

1. 버전 관리 시스템
  가. Git : 분산 버전 관리 시스템
    1) 버전 관리 : 변화를 기록하고 추적
      * ex) 3. 11. 7. 중 3은 major version, 11은 minor version, 12는 patch
      가) major : 대규모 업데이트
      나) minor : 
      다) patch : 
      라) **프로젝트마다 버전이 달라질 수 있음, 그리고 관리해야 할 필요**
    2) 중앙 vs 분산
      가) 중앙 집중식 : 버전은 중앙 서버에 저장 및 관리
        * 중앙 서버에 화재 등 물리적 파괴 시 취약함
      나) 분산식 : 버전을 여러 개의 복제된 저장소에 저장 및 관리
    3) git의 영역
      가) Working Directory : 실제 작업중인 영역
      나) Staging Area : 준비 단계, 다음 버전에 포함시킬 파일들에 대해 준비
      다) commit(커밋) : 작업 사항에 대해 Staging Area에서 Repository로 옮기는 과정
      라) Repository : 새로운 버전을 등록
    4) git의 동작
      가) git init : 최초 1회에 한하여 사용
      나) git status : 변경 상태를 확인
      다) git add 파일경로 : staging area로 파일을 옮기는 과정
        * 공백으로 여러 파일경로를 올릴 수 있음
      라) git commit : 버전을 기록
          * 로컬에서만 관리
          (1) --global : 전역변수
          (2) 터미널서 복사 : 드래그 + 우클릭 / 붙여넣기 : 우클릭
            * 이메일 기록은 edu.ssafy계정 또는 개인 github 계정(권장)
          ** ~/.gitconfig를 통해 user 이름과 이메일을 확인 및 수정 가능하다
          (3) insert 또는 키보드 a를 누르면 수정 가능
          (4) 수정 모드에서 벗어나는 키는 ESC
          (5) 저장하고 종료는 :wq
          (6) git commit 뒤 -m "넣을내용"을 통해 커밋 메시지 탑재 가능
      마) git log : 로그를 기록
          (1) --oneline : 로그를 1줄로 관리
      바) git remote add origin 주소
        (1) origin은 별명, 다른 단어로 사용해도 상관없음
          * origin으로 관습처럼 사용
        (2) git remote -v로 저장한 주소 확인 가능
        (3) git push 
      사) push : 모든 작업을 진짜 끝나면 실행
        * git push 뒤 -u를 추가하면 다음부터는 origin master를 생략할 수 있다. (git push -u origin master)
      아) clone : 최초로 다른 이의 프로젝트를 복제할 때