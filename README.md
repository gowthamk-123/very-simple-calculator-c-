# very-simple-calculator-c-
This calculator contains basic mathematical operations like ADDITION,SUBTRACTION,MULTIPLICATION,DIVISION
#include<iostream>
using namespace std;
class caluclator{
    int a,b;
    public:
       void result()
       {
              cout<<"the value of 1st number is:";
              cin>>a;
              cout<<"the value of 2nd number is:";
              cin>>b;
       }
       int add();
       int subtract();
       int division();
       int multplication();
};
int caluclator::add(){
    return a + b;
}
int caluclator::subtract(){
    return a - b;
}
int caluclator::multplication(){
    return a * b;
}
int caluclator::division()
{
   if(b==0){
             cout<<"infinity";
             return 1;
           }
   else{
        cout<< a / b;
       }
       return 0;
}

int main(){
    caluclator c;
    int  ch;
    cout<<"\n   MENU   \n1.ADDITION\n2.SUBTRACTION\n3.MULTIPLICATION\n4.DIVISION\n0.EXIT\n"<<endl;
    
    do
    {
        cout<<"ENTER YOUR CHOICE";
        cin >> ch;
        switch(ch)
        {
        case 1:
           
              c.result();    
              cout << "Result: " <<
                     c.add() << endl;
              break;
        case 2:
             
            c.result();
            cout << "Result: " <<
                     c.subtract() << endl;
            break;
        case 3:
            c.result();
            cout << "Result: " <<
                     c.multplication() << endl;
            break;
        case 4:
            c.result();
            cout << "Result: " <<
                     c.division() << endl;
            break; 
            
            
        }
        
    }while(ch >= 1 && ch <= 4);
     return 0;
    
    
}
