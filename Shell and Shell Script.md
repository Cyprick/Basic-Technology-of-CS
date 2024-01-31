# [Shell and Shell Script](https://www.shellscript.sh/)
## Variables
1.在shell中执行脚本实际上是打开了一个 "子shell" ，因此 "子shell" 并不继承 "父shell" 的参数，这需要使用export+parameter来引入参数  
> export 只影响从其被调用的那个 shell 开始的新 shell，它不会影响任何已经运行的 shell 的环境变量。
> [同样，子 shell 中对导出变量进行的修改不会影响到父 shell 中的相应变量。](https://www.shellscript.sh/variables1.html)

> . ./myvar2.sh 这一命令的含义是在当前 shell 中某个环境下执行myvar2.sh脚本。
> . 是一个命令别名，等同于 source 命令，其功能主要是在当前的 shell 上下文中执行脚本。
> 这样就可以使用当前shell中的变量

2.Curly Brackets{}
```shell
#!/bin/sh
echo "What is your name?"
read USER_NAME
echo "Hello $USER_NAME"
echo "I will create you a file called ${USER_NAME}_file"
touch "${USER_NAME}_file"
#引号避免了USER_NAME中空格的影响
```
3.预设变量
1）\$1-\$9 :\$1 .. \$9 are the first 9 additional parameters the script was called with.  
2) \$0 :The variable \$0 is the basename of the program as it was called.  
3) \$# : is the number of parameters the script was called with.  
4) #@ :all parameters.
5) $? :This contains the exit value of the last run command.
```shell
#!/bin/sh
/usr/local/bin/my-command
if [ "$?" -ne "0" ]; then
  echo "Sorry, we had a problem there!"
fi
```
6) shift 命令将每个参数变量左移一位。
> 例如，参数的值 \$2 变成 \$1，值 \$3 变成 \$2，以此类推。

7) 至于[\$\$ \$!](https://www.shellscript.sh/variables2.html)

## Appendix
