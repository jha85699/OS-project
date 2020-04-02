#include<stdio.h>
#include<conio.h>
int main()
{
  printf("\t\t\t----------------------- Scheduling -----------------------\n\n\n\n");
  long int n,i=0,j=0;
  printf("Enter Number of Processes : ");
  scanf("%ld",&n ); 
  double priority[n],avg_waiting,avg_turnaround,burstTime[n],arrivalTime[n],waitingTime[n],turnaroundTime[n], process[n], temp, completionTime[n],min,sum=0,sum2=0,wait_final, turnaround_final, wait_avg, turnaround_avg;
  for(i=0;i<n;i++)
  {
    printf("\nEnter Burst Time for Process [%d] : ", i+1 );
    scanf("%lf", &burstTime[i]);
    printf("Enter Arrival Time for Process [%d] : ", i+1 );
    scanf("%lf", &arrivalTime[i] );
    process[i]=i+1;
  }
