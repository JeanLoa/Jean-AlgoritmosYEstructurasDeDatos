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
	return 0;
}
