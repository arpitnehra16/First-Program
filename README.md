

// Online C++ compiler to run C++ program online
//First code source
#include <iostream>
#include<bits/stdc++.h>
using namespace std;
void delarr(int ele,int size,int arr[]){
    int h=0;
    for(int i=0;i<size;i++){
       
        if(arr[i]==ele)
        {
            //h+=1;
            for(int j=i;j<size-1;j++){
                arr[j]=arr[j+1];
            }
            i-=1;
            size--;
    }
}
 for(int i=0;i<size;i++)
   {
       cout<<arr[i]<<" ";
   }
}


int main() {
    // Write C++ code here
    std::cout << "Hello world!";
    int arr[]={12,2,23,4,34,3,4,4,32,4,3,43};
    int ele;
    cout<<"Enter the element and positon of the element";
   int l= sizeof(arr)/sizeof(int);
   cout<<"size of array "<<l<<endl;
   cout<<"Enter element you want delete "<<endl;
   cin>>ele;
   delarr(ele,l,arr);
  

    return 0;
}
