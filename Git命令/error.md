# 使用Git出现问题

## 在.gitignore中添加的文件push后却依然存在

使用Git管理代码的过程中，可以修改.gitignore文件中的标示的方法来忽略开发者想忽略掉的文件或目录，如果没有.gitignore文件，可以自己手工创建。在.gitignore文件中的每一行保存一个匹配的规则例如：

```.gitignore
*.app       # 忽略所有.app结尾的文件
!app.log    # 但app.log除外
/java       # 仅仅忽略项目根目录下的java文件，不包括 test/java
build/      # 忽略build/目录下的所有文件
test/*.txt  # 会忽略 test/log.txt 但不包括 test/app/log.txt
```

有时候.gitignore中添加的文件，当git push的时候还会出现在push的目录中，原因是因为在git忽略目录中，新建的文件在git中会有缓存，如果某些文件已经被纳入了版本管理中，就算是在.gitignore中已经声明了忽略路径也是不起作用的，这时候应该先把本地缓存删除，然后再进行git的push，这样就不会出现忽略的文件了。git清除本地缓存命令如下：

```bash
git rm -r --cached .
git add .
git commit -m 'update .gitignore'
```