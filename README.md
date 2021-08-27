# git 실험용 & 문제 해결

<br><br><br>

---

# 파일 통합 test

### mkdir subtree

### cd subtree

### git init

### git remote add origin <rootRepo>

###### add, commit, push

### git subtree add --prefix=fileName <wantTmoveURL> branchName

<br>

#### 원본에 수정내용을 적용하고 싶으면 add 대신 push!

<br><br>

---

# 저장소명 변경시 url 변경

### git remote set -url

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

- 파일 디렉토리 변경시 추적되지 않는 현상

  캐시에 문제가 있는 것이다.

  해결은 파일 구성을 다 갖춰놓은 다음(커밋해도 이상 없는 상태로 디렉토리를 재구성 한다는 이야기) VSC를 종료한다.

  1. cmd (관리자 권한) 실행
  2. npm cache clean --force
  3. VSC 켠 후 다시 커밋한다.

  > 깃 캐시가 꼬인다...는건 브라우저도 언젠가 꼬일 여지가 있다는건가 캐시관리에대한 자료를 더 찾아볼것
