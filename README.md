# Biography
#display name, age, current and permanent address
#include<iostream>
using namespace std;
int main()
{
	string name;                    /*declaring variable with datatype*/
	string currentadd, permanentadd;
	int age;
	cout << "\n\t\t\t\t\tYour name : ";
	cin >> name;
	cout << "\t\t\t\t\tYour age : " ;
	cin >> age;
	while (cin.fail() != 0)   //if the user enters a special character or alphabet then it will ask the user to enter the number again
	{
		cout << "\a\t\t\t\t\tInvalid Command\nEnter number again   : ";
		cin.clear();
		cin.ignore();
		cin >> age;
	}
	cout << "\t\t\t\t\tYour current address : ";
	cin >> currentadd;
	cout << "\t\t\t\t\tYour permanent address : ";
	cin >> permanentadd;
	cout << "\n\t\t\t\t\tNAME : " << name << endl;
	cout << "\t\t\t\t\tAGE : " << age << endl;
	cout << "\t\t\t\t\tCURRENT ADDRESS : " << currentadd << endl;
	cout << "\t\t\t\t\tPERMANENT ADDRESS : " << permanentadd << endl;
	return 0;
}
