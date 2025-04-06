#include <iostream>

using namespace std;

int main() {
	// Asignación mixta arreglo estático - dinámico
	const int n1 = 10, n2 = 10;
	int n3 = 20, n4 = 20;
	int** p[10][10];
	for (int i = 0; i < n1; ++i) {

		for (int j = 0; j < n2; ++j) {
			
			p[i][j] = new int* [n3];
			
			for (int k = 0; k < n3; ++k) {
				
				p[i][j][k] = new int [n4];
			
			}
		}
	}
	int** a = new int*[2];
	
	a[0] = new int[2] {1, 2};
	a[1] = new int[2] {3, 4};

	p[0][0][0] = a[0];
	p[0][0][1] = a[1]; // Esta línea es una mala práctica, ya que sobredefine siempre desde la primera casilla. Si es la primera vez, es permitible y con bastante advertencias, es mejor reemplazar individualmente, o llenar columnas pero respecto a un iterador, que recorra la columna, yendo fila por fila.
	
	// Si modifico p en el índice indicado, el valor de a varía.
	a[0][0] += 2; // 3
	a[0][1] += 5; // 7

	p[0][0][0][0] -= 1; // 2 - posición de a[0][0]
	p[0][0][0][1] -= 2; // 5 - posición de a[0][1] debido a la concatenación

	cout << a[0][0] << " " << a[0][1];

	return 0;
}
