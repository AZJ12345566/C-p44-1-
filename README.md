# C-p44-1-
C语言学习笔记 p44作业讲解(1)
#include<stdio.h>
#include<string.h>
#include<assert.h>
#include<math.h>
int main()
{
    unsigned long pulArray[]={6,7,8,9,10};
    unsigned long* pulPtr;
    pulPtr=pulArray;
    *(pulPtr+3)+=3;
    printf("%d,%d\n",pulPtr,*(pulPtr+3));
    return 0;
}//输出为6,12



void reverse(char* str)
{
    int len=strlen(str)
    assert(str)
    char* left=str;
    char* right=str+len-1;

    while(left<right)
    {
        char tmp=*left;
        *left=*right;
        *right=tmp;
        left++;
        right--;
    }
}
int main()
{
    char arr[256]={0};
    scanf("%s",arr);//abcdef--->fedcba
    //逆序函数
    reverse(arr);
    printf("%s\n",arr);
    return 0;
}

int main()
{
    int a=0;
    int n=0;
    scanf("%d%d",&a,&n);
    int sum=0;
    int i=0;
    int ret=0;
    for(i=0;i<n;i++)
    {
        ret=ret*10+a;
        sum+=ret;
    }
    printf("%d\n",sum);
    return 0;
}


int main()
{
    //水仙花
    int i=0;
    for(i=0;i<=100000;i++)
    {
        //判断i是否为水仙花数(自幂数)
        //1.计算i的位数-n位数 
        int n=1;
        int tmp=i;
        while(tmp/=10)
        {
            n++;
        }
        //123/10 n++
        //12/10 n++
        //1/10
        
        //2.计算i的每一位的n次方之和 sum
        tmp=i;
        while()
        {
            pow(tmp%10,n);
            tmp/=10;
        }
        //3.比较i==sum
        if(i==sum)
        {
            printf("%d",i;)
        }
    }
    return 0;
}


int main()
{
    int line=0;
    scanf("%d",&line);//
    //打印上半部分
    int i=0;
    for(i=0;i<;j++)
    {
        //打印空格
        int j=0;
        for(j=0;j<line-1-i;j++)
        {
            printf(" ");
        }
        //打印*
        for(j=0;j<2*i+1;j++)
        {
            printf("*");
        }
        printf("\n");
    }
    //打印下半部分
    for(i=0;i<line-1;i++)
    {
        int j=0;
        //打印空格
        for(j=0;j<=i;j++)
        {
            printf(" ");
        }
        //打印*
        for(j=0;j<2*(lin-1-i)-1;j++)
        {
            printf("*");
        }
        printf("\n");
    }
    return 0;
}
