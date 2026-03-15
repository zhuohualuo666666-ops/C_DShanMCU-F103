<!-- 循环结构while语句 -->
while和do while：
while先判断后执行
do while先执行后判断

char *str="1234567890";
int cnt=0
while(str[cnt]!=0)
{
 cnt++;
}
printf("字符个数=%d\n\r",cnt);

打印结果为10。
在C语言中，对于任何指针 p 和整数索引 i，表达式 p[i] 等价于 *(p + i)，
因此str[cnt]!=0这个写法是可以的，相当于*(str+cnt)