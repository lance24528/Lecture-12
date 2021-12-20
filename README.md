//Months
#include <iostream>
#include <string>
#include <iomanip>
#include <array>

using namespace std;

int main()
{

	string Months[12] = { "January","February","March","April","May","June","July","August","September","October","November","December" };


	return 0;
}
//Time Travel
#include <iostream>
#include <string>
#include <iomanip>
#include <array>

using namespace std;

int main()
{
	string Months[12] = { "January","February","March","April","May","June","July","August","September","October","November","December" };
	for (int i = 0; i < 12; i++)
	{
		cout << Months[i] << endl;
	}
	return 0;
}                             
//Marks
                             
#include <iostream>
#include <string>
#include <iomanip>
#include <array>

using namespace std;
float studentAverage;
float total;

int main()
{
	int StudentMarks[5];

	for (int i = 0; i < 5; i++){
		cout << "Enter Mark " << i + 1 << " : ";
		cin >> StudentMarks[i];
		while (cin.fail()){
			cin.clear();
			cin.ignore(1000, '\n');
			cout << "Invalid Input! Try again \nEnter Mark " << i + 1 << " : ";
			cin >> StudentMarks[i];
		}
	}
	for (int i = 0; i < 5; i++){
		total = total + StudentMarks[i];
	}
	studentAverage = total / 5;

	cout << "The student's Average is : " << studentAverage;
	return 0;
}                             
                                                          
