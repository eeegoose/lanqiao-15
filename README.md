# lanqiao-15
#include<iostream>
using namespace std;
int main(){
    int sum=0;
    //第一个人和其他49个人握，
    //第二个跟除第一个人的其他48个握（因为和1握过了）
    //以此类推，倒数第二个和最后一个握，一共49+...+1次
    for(int i=49;i>0;i--){
        sum+=i;
    }
    //减去7个人互握次数
    for(int i=6;i>0;i--){
        sum-=i;
    }
    cout<<sum;
    return 0;
}
