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
      가) git init :  
      나) git status : 변경 상태를 확인
      다) git add 파일경로 : staging area로 파일을 옮기는 과정
        * 공백으로 여러 파일경로를 올릴 수 있음
      라) git commit : 버전을 기록
        * 로컬에서만 관리
        ** --global : 전역변수
        *** 터미널서 복사 : 드래그 + 우클릭 / 붙여넣기 : 우클릭
        **** 이메일 기록은 edu.ssafy계정, 개인 github 계정
        ***** ~/.gitconfig를 통해 user 이름과 이메일을 확인 및 수정 가능하다
        1)) insert 또는 키보드 a를 누르면 수정 가능
        2)) 수정 모드에서 벗어나는 키는 ESC
        3)) 저장하고 종료는 :wq
        ***** git log : 로그를 기록