#### git 명령어 정리
>##### OROGIN CURRENT HEAD 커밋으로 이력 hard 변경
```
git reset --hard ORIG_HEAD
```
[rest blog contents](http://blog.weirdx.io/post/3111)
>##### global 변수 미설정 commit
```
git -c user.name='gwangjunchoi' -c user.email='namsookill@gmail.com' commit -m ""
```
