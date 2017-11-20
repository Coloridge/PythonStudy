# PythonStudy
There are simple programs which I code during my study of Python
I`m Coloridge,a undergraduate at present.
The time is at 15:20 on Nov. 20th in 2017.
Hello,world!
//字符串连接
# include <stdio.h>
# include <string.h>

int main()
{
	char arr1[20],arr2[20];
	gets(arr1);
	gets(arr2);
	int l = strlen(arr1);
	int l2 = strlen(arr2);
	int i = 0;
	while(i < l2)
	{
		arr1[l] = arr2[i];
		i++,l++;
	}
	arr1[l] = '\0';
	puts(arr1);
	return 0 ;
}
