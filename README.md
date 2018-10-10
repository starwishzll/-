# # include <stdio.h>
int main()
{
    int a,b,c,i;
    while(~scanf("%d/%d/%d",&a,&b,&c))
    {
        int d=0;
        int e[12]={31,28,31,30,31,30,31,31,30,31,30,31};
        if((a%100==0&&a%400==0)||(a%100!=0&&a%4==0))
            e[1]=29;
        else
            e[1]=28;
        for(i=0;i<b-1;i++)
        {
            d=e[i]+d;
        }
        d=d+c;
        printf("%d",d);
    }
}
