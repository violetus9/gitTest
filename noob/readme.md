## 2021/11/17 메모용

git >> https || ssh

기존 https, 새 계정 ssh

발단: ssh-keygen

```
//
remote: Repository not found.
fatal: repository [url] not found.
+ fatal: authentication failed for [~else]
//
git config --global credential.helper [sth]
//
+ Credencial Manager
//
+ submodule
//
git remote set-url origin git@github.com:IDIDID/REPOREPO.git
```

- links

  https://git-scm.com/book/ko/v2/Git-%EB%8F%84%EA%B5%AC-Credential-%EC%A0%80%EC%9E%A5%EC%86%8C

............
