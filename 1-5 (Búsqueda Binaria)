#include <iostream>
#include <vector>
#include <algorithm>

using namespace std;

int busquedaBinaria(vector<int>& arr, int objetivo) {
	int izquierda = 0;
	int derecha = arr.size() - 1;

	while (izquierda <= derecha) {
		int medio = izquierda + (derecha - izquierda) / 2;

		if (arr[medio] == objetivo) {
			return medio;
		}
		
		if (arr[medio] < objetivo) {
			izquierda = medio + 1;
		}
		else {
			derecha = medio - 1;
		}
	}

	return -1;
}

int main() {
	srand(time(0));
	
	vector<int> arr (100);

	for (int& valor : arr) {
		valor = rand() % 100;
	}
	sort(arr.begin(), arr.end());

	cout << "Contenido del arreglo: ";
	for (int& valor : arr) {
		cout << valor << " ";
	}
	cout << endl;

	int resultado = busquedaBinaria(arr, 80);
	cout << "El numero 80 se encuentra en el indice: " << resultado;
	return 0;
}
