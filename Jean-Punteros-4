#include <iostream>

using namespace std;

int main() {
	int n1 = 5, n2 = 20;
	int** a = new int*[n1];
	for (int i = 0; i < n1; ++i) {
		a[i] = new int[n2];
	}

	for (int i = 0; i < n1; ++i) {
		cout << "Dimension 2 - indice: " << i << ": ";
		cout << endl;
		for (int j = 0; j < n2; ++j) {
			a[i][j] = rand() % 100;
			cout << "Dimension 1 - indice " << j << ": " << a[i][j];
			cout << endl;
		}
		cout << endl;
	}
	cout << endl;

	int* b = &a[1][0];

	cout << "Contenido de b referencia de a[1]: ";
	for (int i = 0; i < n2; ++i) {
		cout << b[i] << " ";
	}

	cout << endl << endl;

	a[1][2] = 100;
	cout << b[2];

	return 0;
}
