# -Shengzhen-Li-weekly-report
1) Learning hours: Around 15 hours
2) Learning progress: Have learned the basic rules and usage of C Language.Now,I am learning the basice usage of linux.
3) Your implementation of the tasks you have done this week: Have learned how to synchronize the code with Git
4) Unsolved problems: Didn't know how to connet the server.
5) Plan for the next week: Have a good command of linux.Try to finish the 2.5week's task. And learn to connet the server.
6) This Week's Study Report(about C Language):

#include <stdio.h>



//make a monthly calender with C Language



int main()
{
    int month[12]={31,28,31,30,31,30,31,31,30,31,30,31,};

    int mon;
    printf("please input the month of 2022\n");
    scanf("%d",&mon);

    printf("%10s%10s%10s%10s%10s%10s%10s\n","Mon.","Tue.","Wed.","Thu.","Fri.","Sat.","Sun.");

    int i,weekday;

        int day=0;
        int x;
        for(x=0;x<mon-1;x++)
        {
        day=day+month[x];
        }

        weekday=day%7+6;
        if(weekday>7)
        {
        weekday=weekday-7;
        }
        else
        {
            ;
        }

        int counter;
        for(counter=1;counter<weekday;counter++)
        {
            printf("          ");
        }

    for(i=1;i<=month[mon-1];i++)
    {
        printf("%10d",i);

        if(i%7==0&&weekday==1)
        {
            printf("\n");
        }
        if(i%7==8-weekday)
        {
            printf("\n");
        }




}
return 0;
}



