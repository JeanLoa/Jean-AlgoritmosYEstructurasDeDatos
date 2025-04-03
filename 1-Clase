#include <iostream>
#include <fstream>

using namespace std;

template<typename T>

class Cuadrado {
private:
	T lado;
public:
	Cuadrado(T lado) : lado(lado) {}
	~Cuadrado() {}

	T area() { return lado * lado; }
	T volumenreflejado() { return lado * lado * lado; }
};


int main() {

	Cuadrado <int>* cuadrado = new Cuadrado<int>(5);
	cout << cuadrado->area() << endl;

	const char* mensaje_escrito = "Hola";
	fstream* archivo = new fstream("Archivo.txt");

	archivo->write(mensaje_escrito, strlen(mensaje_escrito));

	archivo->seekg(0, ios::end);

	int tamanio = archivo->tellg();

	archivo->seekg(0, ios::beg);

	char* mensaje_leido = new char[tamanio];

	if (archivo) {
		archivo->read(mensaje_leido, tamanio);
		cout << mensaje_leido;
	}
	else {
		cout << "No se pudo abrir el archivo";
	}

	delete[] mensaje_leido;
	delete archivo;

	return 0;
}
