# .vim
关于我的vim的一些配置和插件。  
先上两张效果图  
![image](https://github.com/sqwlly/.vim/blob/master/images/vim_cpp.png)  
![image](https://github.com/sqwlly/.vim/blob/master/images/vim_php.png)  
(前情提示：需要vim支持lca和Python2、Python3，请先查看是否支持，如果不支持请自行百度如何重新编译vim支持lca、Python2、Python3)  
克隆下来后把这些文件放到用户主目录下的.vim文件下
```bash
$ sudo cp -r ~/Downloads/.vim/* /home/用户名/.vim
```
接着进入vim编辑界面输入vim命令
```bash
$ vim
:PluginInstall
```
然后将.vimrc文件同样放到用户主目录下
```bash
$ sudo cp ~/Downloads/.vim/.vimrc /home/用户名/
```
