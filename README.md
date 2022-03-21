# c-lab
this repository contians c lab programs
#include<stdio.h>
#include<math.h>
int main()
{
   int i,n;
   float a[20],std,var,mean,sum;
   float *p;
   printf("Enter n:");
   scanf("%d",&n);
   printf("Enter %d no of elements\n",n);
   p=a;
   for(i=0;i<n;i++)
   {
	scanf("%f",p);
	p++;
   }
   p=a;
   sum:var=std=mean=0.0;
   for(i=0;i<n;i++)
     {
	sum=sum+*p;
	p++;
     }
     mean=sum/n;
     p=a;
     for(i=0;i<n;i++)
     {
      var=var+pow((*p-mean),2);
       p++;
     }
     var=var/n;
     std=sqrt(var);
     printf("sum=%f\n",sum);
     printf("variance=%f\n",var);
     printf("mean=%f\n",mean);
     printf("stander=%f\n",std);
    return 0;
}
     	
