# mygit (이거저거 실험용)
# MarkDown으로 project 설명합니다.
### #하나가 h1, ##하면 h2, ###하면 h3 ...


markdown 문법을 찾아봅시다!
<br><br><br>


***

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
***

# 저장소명 변경시 url 변경

### git remote set -url
<br><br>

***

## 2021/06/18

* github 프로젝트 main에 PR 보냈을때 conflict 없이 병합됨
    근데 거기서 몇 명의 커밋내용이 다 날아갔는데
    > 1. 왜 conflict체크 없이 몇몇파일 강제 삭제됐는지
    > 2. 내 브랜치랑 main이랑 왜 원활히 합쳐지지 않고 두개의 메인인듯 따로노는지

    > 도무지 알 길이 없어 메모를 남김....
