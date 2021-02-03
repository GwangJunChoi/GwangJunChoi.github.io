#### git 명령어 정리
>##### 바로 이전의 커밋으로 이력 변경 (관련 블로그글)[http://blog.weirdx.io/post/3111]
```
git reset --hard ORIG_HEAD
```

>##### global 변수 미설정 commit
```
git -c user.name='gwangjunchoi' -c user.email='namsookill@gmail.com' commit -m ""
```
