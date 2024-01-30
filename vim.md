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

## 5.执行外部命令
1）：！command
> :!ls
:!rm FILENAME

2）v motion :w FILENAME 
>可将当前编辑文件中可视模式下选中的内容保存到文件FILENAME 中。

3）:r FILENAME 
>可提取磁盘文件 FILENAME 并将其插入到当前文件的光标位置后面。

4）:r !ls 
>可以读取 ls 命令的输出并将其放置到当前文件的光标位置后面。

## Appendix
> 词条缩写

w(word) e(end of word) a(after) 
i(insert)  q(quit) $(sentence行末) d(delete)      
> 常用命令

u(undo撤销)U（撤销该行变化）
C-r(撤销被撤销的命令)  

> 冷门命令 

1）c(change)
2）如果光标当前位置是括号(、)、[、]、{、}，按 % 会将光标移动到配对的括号上

> 提示

1）编辑vimrc保存对vim的偏好          
2）输入 :set xxx 可以设置 xxx 选项。一些有用的选项如下：
        'ic' 'ignorecase'       查找时忽略字母大小写
        'is' 'incsearch'        查找短语时显示部分匹配
        'hls' 'hlsearch'        高亮显示所有的匹配短语
     选项名可以用完整版本，也可以用缩略版本。

3）在选项前加上 no 可以关闭选项：  :set noic
