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

	cout << "-------adding elements to the front and back of the vector--------" << endl;

	cout << cars.front() << endl; //gets the first element
	cout << cars.back() << endl; //gets the last element




	return 0;
}
