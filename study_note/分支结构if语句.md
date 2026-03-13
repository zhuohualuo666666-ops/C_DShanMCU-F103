<!-- 分支结构if语句 -->
if()
{
}
else if()
{
}

执行到else if时，其语句之前的if或者else if语句中的条件便是确定为不满足，
可通过这个原理进行范围缩小，
例如

int a=18;

if(a>=1000)
{
    printf("这是个四位以上的数");
}
else if(a>=100)
{
    printf("这是个三位数");
}
else if(a>=10)
{
    printf("这是个两位数");
}