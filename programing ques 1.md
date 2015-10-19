#include <iostream>
#include <string>
using namespace std;



class bank_account
{
public:

void show(string name, string number , double balance);
void withdraw(double balance, double amount);
void deposit(double balance , double amount);

private:
string depositor_name , account_number;
double balance;
};
void bank_account::withdraw(double balance, double amount)
{
if(amount>balance)
cout<<"you can’t withdraw amount you don’t have in your balance\n";
else
balance=balance-amount;
}
void bank_account::deposit(double balance,double amount)
{
if (amount<=0)
cout<<"you can’t deposit amount of zero\n";
else
balance=balance+amount;
}
void bank_account::show(string name, string number , double balance)
{ cout<<"Bank account name: "<<name<<endl<<"bank account number: "<<number<<endl<<"balance :"<<balance<<endl;
}
void main()
{
bank_account x;
x.withdraw(10,15);
x.deposit(25,32);
x.show("HSBC","1232131", 81);
}
