# VIM的一些配置
新增满足NERDTree插件的安装，以下需求请在.vimrc里自行添加
```bash
autocmd vimenter * NERDTree "自动打开NERDTree
"没有指定文件自动打开NERDTree
autocmd StdinReadPre * let s:std_in=1
autocmd VimEnter * if argc() == 0 && !exists("s:std_in") | NERDTree | endif 
"当vim启动打开目录时，自动打开NERDTree
autocmd StdinReadPre * let s:std_in=1
autocmd VimEnter * if argc() == 1 && isdirectory(argv()[0]) && !exists("s:std_in") | exe 'NERDTree' argv()[0] | wincmd p | ene | endif 
```
还有就是这里手动打开NERDTree插件快捷键是Ctrl+f，具体请修改vimrc配置
---
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
