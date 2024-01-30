# VIM
## 1.查找功能
输入 / 然后紧随一个字符串是在当前所编辑的文档中正项查找   
用n(next)重复上命令 N查找相反方向
> 用 ? 来逆向查找

## 2.替换功能
替换一行的第一个
> :s/old/new
替换一行的所有项
> :s/old/new/g
替换两行的所有项
> :#,#s/old/new
替换全文的所有项
> :%s/old/new/g
替换全文的所有项并询问
> :%s/old/new/gc

## 3.跳转功能
1）C-g 显示位置和文件信息
2）G跳转至最后一行
3）gg跳转至第一行
4）先输入 “行号” 在输入一个 G 实现跳转 

## 4.复制粘贴
1）按 v 进入可视模式 移动光标选取文字
2）按 y 复制文本，按p（place）粘贴文本
3）删除（dw.de,dd...）的文本会进入缓存区，可被粘贴（即剪切）

## Appendix
> 词条缩写
w(word) e(end of word) a(after) i(insert)       
q(quit) $(sentence行末) d(delete)      
> 常用命令
u(undo撤销）U(撤销该行变化）C-r(撤销被撤销的命令)       
> 冷门命令 
           c(change)    
