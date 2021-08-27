## git 실험용 & 문제 해결

<br><br><br>

---

## 파일 통합 test

### mkdir subtree

### cd subtree

### git init

### git remote add origin <rootRepo>

###### add, commit, push

### git subtree add --prefix=fileName <wantTmoveURL> branchName

<br><br>

---

## 2021/06/18

- github 프로젝트 main에 PR 보냈을때 conflict 없이 병합됨
  근데 거기서 몇 명의 커밋내용이 다 날아갔는데

  > 1. 왜 conflict체크 없이 몇몇파일 강제 삭제됐는지
  > 2. 내 브랜치랑 main이랑 왜 원활히 합쳐지지 않고 두개의 메인인듯 따로노는지

  > 도무지 알 길이 없어 메모를 남김....

<br>

## 2021/08/28

- 파일 디렉토리 변경시(프로젝트의 통합이라던가 카테고리를 다시 나눈다거나 하는 작업) 추적되지 않는 현상

  캐시에 문제가 있는 것이다.

  해결은 파일 구성을 다 갖춰놓은 다음(커밋해도 이상 없는 상태로 디렉토리를 재구성 한다는 이야기) VSC를 종료한다.

  1. cmd (관리자 권한) 실행
  2. npm cache clean --force
  3. VSC 켠 후 다시 커밋한다.

  > 깃 캐시가 꼬인다...는건 브라우저도 언젠가 꼬일 여지가 있다는건가 캐시관리에대한 자료를 더 찾아볼것

  <br>

- 문제 발견

  위 방식대로 디렉토리 구성 다시하고 git push 했을 때, 원격 저장소엔 삭제된 파일들에 대한 내용이 반영되지 않아서 깃허브에서 일일히 삭제했다.

  (깃에서 캐시된 내용을 삭제해서 그런거라고 추정)

  할튼 이렇게도 해결은 되는데.. 원론적으로 이런 충돌원인?에 대한 내용이 분명 있을것임.. 기억은 해두자 일단
