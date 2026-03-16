<!-- 循环结构for语句 -->
for(;;)等价于while(1)，都是产生一个无限循环



char *str = "asfasdfc12421sdfasf3452ad34";
	
	for (i = 0; str[i] != 0; i++)
	{
		if (str[i] >= '0' && str[i] <= '9')
			printf("%c", str[i]);
	}
	printf("\n\r");



char *str = "asfasdfc12421sdfasf3452ad34"

字符串是由多个元素组成的，每个元素都有自己的地址，而指针一次只能指向一个地址，
所以这句话意思hi将字符串字面量 "asfasdfc12421sdfasf3452ad34" 的第一个字符的地址赋给指针变量 str。