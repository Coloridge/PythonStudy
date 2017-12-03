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
/*# include <stdio.h>

float Ort(float a,char op,float b);
float Alge(float a,char op1,float b,char op2,float c);
int main()
{
	float a,b,c;
	char op1,op2;
	scanf("%f",&a);
	op1 = getchar();
	scanf("%f",&b);
	op2 = getchar();
	scanf("%f",&c);
	float x = Alge(a,op1,b,op2,c);
	printf("%.2f",x);
	return 0;
}
float Ort(float a,char op,float b)
{
	switch(op)
	{
		case '+':
			return a + b;
		case '-':
			return a - b;
		case '*':
			return a * b;
		case '/':
			return a / b;
	}
}
float Alge(float a,char op1,float b,char op2,float c)
{
	if((op1 == '+' || op1 == '-') && (op2 == '*' || op2 == '/'))
		return Ort(a,op1,Ort(b,op2,c));
	else
		return Ort(Ort(a,op1,b),op2,c);
}*///三元四则运算
/*# include <stdio.h>

void pat1();void pat2();void pat3();void pat4();
void pat5();void pat6();void pat7();void pat8();
void pat9();void pat10();void pat11();void pat12();
int main()
{
	int i;
	scanf("%d",&i);
	switch(i)
	{
	case 1:
		pat1();
		break;
	case 2:
		pat2();
		break;
	case 3:
		pat3();
		break;
	case 4:
		pat4();
		break;
	case 5:
		pat5();
		break;
	case 6:
		pat6();
		break;
	case 7:
		pat7();
		break;
	case 8:
		pat8();
		break;
	case 9:
		pat9();
		break;
	case 10:
		pat10();
		break;
	case 11:
		pat11();
		break;
	case 12:
		pat12();
		break;
	}
	return 0;
}
void pat1()
{
	printf("#####\n");
	printf("## ##\n");
	printf("#   #\n");
	printf("## ##\n");
	printf("#####\n");
}
void pat2()
{
	printf("*********\n");
	for(int i = 1;i <= 9;i++)
	{
		for(int j = i;j <= 9;j++)
			printf("%d",j);
		printf("\n");
	}
	printf("*********\n");
}
void pat3()
{
	for(int i = 0;i < 11;i++)
		printf("*");
	printf("\n");
	printf("*1+'1'='2'*\n");
	for(int i = 0;i < 11;i++)
		printf("*");
}
void pat4()
{
	for(int j = 0;j < 2;j++)
	{
		printf("*");
		for(int i = 1;i <= 9;i++)
			printf("%d",i);
	}
	printf("\n");
	int a = 0;
	for(int  i = 0;i <= 18;i = i + 2)
	{
		for(int j = 0;j < a;j++)
			printf(" ");
		a++;
		for(int j = 19 - i;j > 0;j--)
			printf("@");
		printf("\n");
	}
	for(int j = 0;j < 2;j++)
	{
		printf("*");
		for(int i = 1;i <= 9;i++)
			printf("%d",i);
	}
}
void pat5()
{
	printf("*123456789*123456789*1234\n");
	int num[20] = {0,1},count = 0;
	for(int i = 2;i < 20;i++)
		num[i] = num[i-2] + num[i-1];
	for(int i = 0;i < 20;i++)
	{
		int a = num[i] / 10;
		if(a == 0)
			printf("   ");
		else if(a > 0 && a < 10)
			printf("  ");
		else if(a >= 10 && a < 100)
			printf(" ");
		else if(a >= 100 && a <1000);
			printf(" ");
		printf("%d",num[i]);
		count++;
		if(count % 5 == 0)
		{
			printf("\n");
		}
	}
	printf("*123456789*123456789*1234\n");
}
void pat6()
{
	printf("*****");
	for(int i = 0;i < 3;i++)
	{
		printf("\n");
		printf("*   *");
	}
	printf("\n");
	printf("*****");
}
void pat7()
{
	printf("*********\n");
	for(int i = 1;i <= 9;i++)
	{
		for(int j = 0;j < i - 1;j++)
			printf(" ");
		for(int j = i;j <= 9;j++)
		{
			printf("%d",j);
		}
		printf("\n");
	}
	printf("*********\n");
}
void pat8()
{
	printf("**********\n");
	printf("*\"Hello!\"*\n");
	printf("**********\n");
}
void pat9()
{
	for(int i = 0;i < 2;i++)
	{
		printf("*123456789");
	}
	printf("\n");
	int a = 9;
	for(int i = 1;i <= 19;i = i + 2)
	{
		for(int j = a;j > 0;j--)
			printf(" ");
		a--;
		for(int j = 0;j < i;j++)
			printf("@");
		printf("\n");
	}
	for(int i = 0;i < 2;i++)
	{
		printf("*123456789");
	}
}
void pat10()
{
	for(int i = 0;i < 8;i++)
	{
		printf("*123456789");
	}
	//杨辉三角

	for(int i = 0;i < 8;i++)
	{
		printf("*123456789");
	}
}
void pat11()
{
	for(int i = 0;i < 8;i++)
	{
		printf("*123456789");
	}
	printf("\n");
	int x,y;
	for(int i = 1;i <= 20;i++)
	{
		for(int j = 1;j <= i;j++)
		{
			x = i * j;
			y = x / 10;
			if(y == 0)
				printf("   ");
			else if(y > 0 && y < 10)
				printf("  ");
			else if(y >= 10 && y < 100)
				printf(" ");
			printf("%d",x);
		}
		printf("\n");
	}
	for(int i = 0;i < 8;i++)
	{
		printf("*123456789");
	}
}
void pat12()
{
	for(int i = 0;i < 8;i++)
	{
		printf("*123456789");
	}
	printf("\n");
	for(int i = 1;i <= 400;i++)
	{
		int a = i / 10;
		if(a == 0)
			printf("   ");
		else if(a > 0 && a < 10)
			printf("  ");
		else if(a >= 10 && a < 100)
			printf(" ");
		printf("%d",i);
		if(i % 20 == 0)
			printf("\n");
	}
	for(int i = 0;i < 8;i++)
	{
		printf("*123456789");
	}
}*///图案输出
/*# include <stdio.h>

int Ort(int a,char op,int b);
int Alge(int a,char op1,int b,char op2,int c);
int main()
{
	int a,b,c;
	char op1,op2;
	scanf("%d",&a);
	op1 = getchar();
	scanf("%d",&b);
	op2 = getchar();
	scanf("%d",&c);
	int x = Alge(a,op1,b,op2,c);
	printf("%d",x);
	return 0;
}
int Ort(int a,char op,int b)
{
	switch(op)
	{
		case '+':
			return a + b;
		case '-':
			return a - b;
		case '%':
			return a % b;
		case '^':
			{
				int sum = 1;
				for(int i = 0;i < b;i++)
				{
					sum *= a;
				}
				return sum;
			}
	}
}
int Alge(int a,char op1,int b,char op2,int c)
{
	if((op1 == '+' || op1 == '-') && (op2 == '%' || op2 == '^'))
		return Ort(a,op1,Ort(b,op2,c));
	else
		return Ort(Ort(a,op1,b),op2,c);
}*///附加1
import sys
filename = sys.argv[0]
f = open(filename,'r',encoding = 'utf-8')
line_no = 0
while True:
    line_no += 1
    line = f.readline()
    if line:
        print(line_no,':',line)
    else:
        break;
f.close()
# 输出图案
/*# include <stdio.h>

int Ort(int a,char op,int b);
int Alge(int a,char op1,int b,char op2,int c);
int main()
{
	int a,b,c;
	char op1,op2;
	scanf("%d",&a);
	op1 = getchar();
	scanf("%d",&b);
	op2 = getchar();
	scanf("%d",&c);
	int x = Alge(a,op1,b,op2,c);
	printf("%d",x);
	return 0;
}
int Ort(int a,char op,int b)
{
	switch(op)
	{
		case '+':
			return a + b;
		case '-':
			return a - b;
		case '%':
			return a % b;
		case '^':
			{
				int sum = 1;
				for(int i = 0;i < b;i++)
				{
					sum *= a;
				}
				return sum;
			}
	}
}
int Alge(int a,char op1,int b,char op2,int c)
{
	if((op1 == '+' || op1 == '-') && (op2 == '%' || op2 == '^'))
		return Ort(a,op1,Ort(b,op2,c));
	else
		return Ort(Ort(a,op1,b),op2,c);
}*///附加1
/*# include <stdio.h>
# include <string.h>

void wow(char a[],char);
int main()
{
	char a[40],c;
	gets(a);
	c = getchar();
	wow(a,c);
	puts(a);
	return 0;
}
void wow(char a[],char c)
{
	int i,l = strlen(a);
	a[2 * l - 1] = '\0';
	for(i = l - 1;i > 0;i--)
	{
		a[2 * i] = a[i];
		a[2 * i - 1] = c;
	}
}*///字符串插入
# include <stdio.h>
# include <string.h>

void qaq(char *,char);
int main()
{
	char s[20],c;
	gets(s);
	c = getchar();
	qaq(s,c);
	puts(s);
	return 0;
}
void qaq(char a[],char c)
{
	int i,count = 0,l = strlen(a);
	for(i = 0;i < l;i++)
	{
		if(a[i] == c)
			count++;
		else
			a[i - count] = a[i];
	}
	a[i - count] = '\0';
}//附加2（字符删除）
/*# include <stdio.h>
# include <string.h>

void qaq(char *,char);
int main()
{
	char s[20],c;
	gets(s);
	c = getchar();
	qaq(s,c);
	puts(s);
	return 0;
}
void qaq(char a[],char c)
{
	int i,j,count = 0,l = strlen(a);
	for(i = 0;i < l;i++)
	{
		if(a[i] == c)
			count++;
		else
			a[i - count] = a[i];
	}
	j = i - count + 1;
	for(i = 0;i < count - 1;i++,j++)
		a[j] = c;
	a[j] = '\0';
}*///附加3（字符换位）

import sys
def a(n):
    print(('*'*n).center(50))
line = int(sys.argv[1])
for i in range(1,2 * line,2):
    a(line)
#传递不可变对象
def plus(a,b):
    a += b
    return a
i  = 100
i = plus(i,10)
print(i)
#随机排序
import random
def exchange(a,i,r):
    temp = a[i]
    a[i] = a[r]
    a[r] = temp
def shuffle(a):
    n = len(a)
    for i in range(n):
        r = random.randrange(i,n)
        exchange(a,i,r)
a = [1,2,3,4,5,6]
shuffle(a)
print(a)
#shuffle函数(随机排序列表元素)
import random
a = [1,2,3,4,5,6]
random.shuffle(a)
print(a)

