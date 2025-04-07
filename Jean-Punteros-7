#include <iostream>
#include <vector>
#include <string>

using namespace std;

class Persona {
private:
	string nombre = " ";
public:
	Persona(){}
	Persona(string n) : nombre(n){}
	~Persona(){}
	void saludar() {
		cout << "Hola " << nombre << endl;
	}
};

int main() {
	int* p = new int[5];
	*(p + 1) = 1;
	p[1] = 1;

	cout << p[1] << " ";
	cout << *(p + 1) << endl;

	Persona* personas = new Persona[5];

	personas[0] = Persona("Jean");
	(*(personas)) = Persona("Jean");
	(*(personas + 1)) = Persona("Ana");

	personas->saludar(); // Jean
	personas[0].saludar(); // Jean
	(*(personas)).saludar(); // Jean
	
	personas[1].saludar(); // Ana
	(*(personas + 1)).saludar(); // Ana

	(*(personas + 2)).saludar(); // null

	return 0;
}
