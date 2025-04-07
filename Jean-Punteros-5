#include <iostream>
#include <vector>
#include <string>

using namespace std;

class Persona {
public:
	void saludar() {
		cout << "Hola" << endl;
	}
};

int main() {
	int* p = new int;
	*p = 1;
	p[0] = 1;

	cout << &*(p) << " ";
	cout << p << " ";
	cout << p[0] << " ";
	cout << *(p) << endl;

	Persona* persona = new Persona;
	persona->saludar();
	persona[0].saludar();
	(*persona).saludar();

	return 0;
}
