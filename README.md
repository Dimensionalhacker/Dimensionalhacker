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

    cout<<"-----------Adding values--------------"<< endl;
    
    cars.push_back("Tesla"); //adds elements at the end of the vector
    for (string cars : cars){
        cout<< cars<<endl;
    }
    
    cout << "-----------removing elements--------------"<<endl;
    
    cars.pop_back(); //removes elements form the back of the vector 
    for (string cars : cars){
        cout<<cars<<endl;
    }
    
    cout<<"-------checking the size of the vector-------------"<<endl;
    cout<<cars.size();
    
    cout<<"---------clearing the vector------------"<<endl;
    cout<<cars.empty()<<endl;
    
    cout<< "---------------lopping through a vector----------"<<endl;
    
    for (string cars : cars){
        cout<< cars <<endl;
    }
    cout<< "------------------------------------"<<endl;
    
    for(int i = 0; i<cars.size() ; i++){
        cout << cars[i] <<endl;
    }

	return 0;
}
