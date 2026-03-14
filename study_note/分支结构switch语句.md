<!-- 分支结构switch语句 -->

switch语句中如果某个 case 后面没有 break，程序会继续往下执行后面的 case 代码，直到遇到 break 或 switch 结束

例：
    char day;
    printf("请输入1到7之间的数字: ");
    scanf("%c", &day); // 由于mircolib的问题它无法使用%d获得正确的整数,但是可以使用%c

    switch (day) {
        default:
            printf("输入无效，请输入1到7之间的数字。\n\r");
		    break;
        case '4':
            printf("星期四\n\r");
            break;
        case '1':
            printf("星期一\n\r");
            break;
        case '2':
            printf("星期二\n\r");
          
        case '3':
            printf("星期三\n\r");
            break;
        case '5':
            printf("星期五\n\r");
            break;
        case '6':
            printf("星期六\n\r");
            break;
        case '7':
            printf("星期日\n\r");
            break;
    }

当输入2时，会打印出：
    星期二
    星期三


其本质结构类似：
switch(day)
{
    if(day=='1') goto L1;
    if(day=='2') goto L2;
    if(day=='3') goto L3;

L1:
    printf("星期一");
    break;

L2:
    printf("星期二");

L3:
    printf("星期三");
    break;
}