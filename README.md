#include <iostream>
#include <vector>

using namespace std;


int main() {

	cout << "---------first method-------------" << endl;

	vector<string>cars = { "Benz", "BMW" , "Ford" };
	
	for (string cars : cars) {
		cout << cars << endl;
	}

	cout << "---------------next method------------------" << endl;


	cout << cars[0] << endl;
	cout << cars[1] << endl;
	cout << cars[2] << endl;

	cout << "------------next method----------------" << endl;

	cout << cars.front() << endl; //gets the first element
	cout << cars.back() << endl; //gets the last element



	cout << cars.at(1) << endl; //gets the second element
	cout << cars.at(2)<< endl; // gets the third element

	cout << "-------changing vector elements------------" << endl;

	cars[1] = "bugatti";
	for (string cars : cars) {
		cout << cars << endl; 
	}



	return 0;
}
