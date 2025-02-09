#include<stdio.h>
int sumarray(int *arr, int size){
int sum=0;
for(int i=0; i<size;i++){
    sum+=*(arr+i);
}
return sum;
}
int main(){
int n;
printf("enter the value of n:");
scanf("%d", &n);
int arr[n];
printf("\nenter %d elements:",n);
for(int i=0;i<n;i++){
    scanf("%d", arr+i);
}
int sum=sumarray(arr, n);
printf("\nthe sum of array elements:%d\n", sum);
return 0;
}
