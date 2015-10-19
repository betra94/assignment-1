# assignment-1
Name: Peter Nagy Alfred                                                      Section: 1


Chapter Review
Q1: What is a Class?
A1: 
A class is a programming construct that defines the common state and behavior of a group of similar objects.

Q2: How does a class accomplish abstraction, encapsulation, and data hiding?
A2: The class accomplish abstraction by giving each part a well-defined interface so that all the other parts and drivers can be able to use it, and it can accomplish encapsulation by making each part well isolated from other parts that it only knows what it has to do and nothing more, and did the data hiding by adding the protected and private parts in the classes so their data are always hidden from users.

Q3: What is the relationship between an object and a class?
A3: 
A class is a definition of the behavior of an object and 
Objects are instances of classes.

Q4: In what way, aside from being functions, are class function members different from
Class data members?

A4: Classes can contain static member data and member functions. When a data member is declared as static only one copy of the data
is maintained for all objects of the class.

Q5: Define a class to represent a bank account. Data members should include the
Depositor’s name, the account number (use a string), and the balance?

A5: The code;
#include <iostream>
#include <string>
Using namespace std;





Class bank_account()
{
Public:

Void show(string name, string number , double balance);
void withdraw(double balance, double amount);
Void deposit(double balance , double amount);

Private:
String depositor_name , account_number;
double balance;
};
Void bank_account::withdraw(double balance, double amount)
{
if(amount>balance)
cout<<”you can’t withdraw amount you don’t have in your balance\n”;
else
Balance=balance-amount;
}
void bank_account::deposit(double balance,double amount)
{
if (deposit<=0)
cout<<”you can’t deposit amount of zero\n”;
Else
Balance=balance+amount;
}
Void bank_account::show(string name, string number , double balance)
{ cout<<”Bank account name: ”<<name<<endl<<”bank account number: ”<<number<<endl<<”balance :”<<balance<<endl;
}
Void main()
{
bank_account x;
x.withdraw(10,15);
x.deposit(25,32);
x.show(“HSBC”,”1232131”, 81);
}





Q6: When are class constructors called? When are class destructors called?
A6: We call the constructor to create an object from a class, and the destructor to end the life time of an object or free the resources that the object may have acquired during its life time.

Q8: What is a default constructor? What is the advantage of having one?
A8: 
A default constructor is a constructor that is used to create an object when you don’t provide explicit initialization values and is called with no arguments.

Q10: What are this and *this?
A10: If you had a function that returns (this) it would be a pointer to the current object while a function that returns (*this) would be a clone of the current object allocated on the stack.


