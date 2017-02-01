# PowerRecur

#include<iostream>
using namespace std; 

int RecurPower(int base, int power) 
{
	if (power<0) 
	{
		cout<< "Please enter a positive exponent: " <<endl; 
		cin>>power; 
		RecurPower(base,power); 
	}



	else if (power==0)
	{
		return 1; 
	}


	else 

	{

		return base *RecurPower(base,power-1); 
	}




}




int main()
{


	cout<<RecurPower(-3,3); 


	system("Pause"); 
	return 0; 
}
