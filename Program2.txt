#include <iostream>
#include <string>
using namespace std;

class person {
private:
	string name;
	int age;
public:
	person() {
		age = 0;
	}
	void setName(string name) {
		this->name = name;
	}
	void setAge(int age) {
		this->age = age;
	}
	int getAge() {
		return age;
	}
	string getName() {
		return name;
	}
	void display() {
		cout << name <<endl;
		cout << age <<endl;
	}
};
int main() {
	person waqar;
	int Age = 56;
	string name = "Waqar Asghar";
	waqar.setAge(Age); 
	waqar.setName(name); 
	cout << waqar.getName() << endl;
	cout << waqar.getAge() << endl;

	cout << endl;
	cout << "Using function: \n";
	waqar.display();


	return 0;
}