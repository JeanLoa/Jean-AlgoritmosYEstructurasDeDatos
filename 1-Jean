#include <iostream>

using namespace std;

void pausa() {
	system("pause>0");
	system("cls");
}

int main() {
	int a, b, c;
	int *p1, *p2;

	/* Uso de referencia */

	// Modelo referencia (individual - sin reserva de memoria | definición del tamaño de array dinámico).
	a = 10;

	p1;
	p1 = &a;

	// Modelo referencia (individual - con reserva de memoria | definición del tamaño de array dinámico).
	p2 = new int [1];
	p2 = &a;

	p1[0] += 2; // Acceso del arreglo de datos que maneja, pero referenciados.

	cout << a << " " << *p1 << " " << *p2 << endl; // 12

	pausa();
	// Modelo referencia (múltiple - sin reserva de memoria | definición del tamaño de array dinámico).
	a = 10, b = 20, c = 30;
	int num[] = { a, b, c };
	p1;
	// En este caso, p1 tiene 2 opciones:
	// - Referenciarse a otra matriz de similares caracteristicas (bidimensión).
	// - Crear una matriz independiente de otras, asignando valores a cada índice.
	p1 = num; // En caso de matrices, dejamos de lado el signo de referencia, se omite, porque cuando usemos el índice, nos referimos a la matriz que controla independientemente p1.
	
	// Modelo referencia (múltiple - con reserva de memoria | definición del tamaño de array dinámico).
	p2 = new int [3];
	p2 = num;

	num[0] += 1;

	for (int i = 0; i < 3; ++i) {
		cout << num[i] << " " << p1[i] << " " << p2[i] << endl; // i = 0 -> 11
	}
	pausa();
	
	// Modelo no referencia (individual - sin reserva de memoria | definición del tamaño de array dinámico).
	a = 10;
	// int* q1; Ya no es posible generar punteros que apuntan a arreglos dinámicos con tamaño no definido
	// q1[0] = a;
	// q1[0] -= 1;

	// Modelo no referencia (individual - con reserva de memoria | definición del tamaño de array dinámico).
	int* q2 = new int[1]; // Solo este modelo es posible
	q2[0] = a;

	a += 1;

	cout << a << " " << q2[0] << endl; // a = 11, p2[0] = 10

	pausa();

	// Modelo no referencia (múltiple - sin reserva de memoria | definición del tamaño de array dinámico).
	a = 10, b = 20, c = 30;
	// int *q1; Lo mismo, no es posible generar arreglos dinámicos no definidos en su tamaño
	// q1[0] = a;
	// q1[1] = b;
	// q1[2] = c;

	// Modelo no referencia (múltiple - sin reserva de memoria | definición del tamaño de array dinámico).
	q2 = new int[3];
	q2[0] = a;
	q2[1] = b;
	q2[2] = c;

	q2[0] -= 1;
	a += 1;

	for (int i = 0; i < 3; ++i) {
		cout << " " << q2[0] << " " << a << endl; // i = 0 -> 9 11
	}

	pausa();

	// Como conclusión:
	// - Las referencias apegan un conjunto de datos a un modelo de puntero del mismo tipo, siempre que las dimensiones encajen, el apunte será posible.
	// - Las copias individuales ocurren cuando asignamos indexadamente al arreglo del puntero disponible, de esta manera, no se asocia a ningún dato externo de manera referenciada.
	// Un ejemplo: Teniendo | int a = 5, *p1; | -> *p1 = a; no es lo mismo que -> p1[0] = a; |
	// El primero referencia el modelo de a junto a sus dimensiones y lo encaja dentro del puntero, el otro solo rellena sus dimensiones posibles gracias al indexado. 
	// Punto positivo (sin inicialización):
	// El puntero sin inicializar, es útil cuando queremos referenciar directamente, la definición de tamaños por dimensión se asigna automáticamente.
	// Si el puntero tiene una parte definida, ejemplo -> int * p[3], es de forma [und, 3] - de manera que cuando usemos sus indexaciones, nos dará error. 
	// El puntero debe tener la forma de la forma a referenciar para que funcione correctamente la referencia y el mapeado, el número de * indica sus dimensiones.
	// Punto positivo (con inicialización):
	// El puntero inicializado sirve para mapear elementos sin necesidad de ser referencias directas de todo el cuerpo del puntero.
	// Si el puntero al ser referenciado, no encaja con su definición, a pesar de ser las mismas dimensiones, por ejemplo.
	// int * p = new int[3], d[] = {1,2,3,4}; si p = d, dará error, porque p ya está definido en tamaño, y d no encaja en él.

	// Un dato adicional, en operaciones con punteros, este flujo es normal, pero cuando tenemos matrices independientes, ya sea dinámica o estática, esta puede contener elementos referenciados, lo que aumenta el peligro de la manipulación de datos si llega a filtrarse ese dato en alguna base de datos.
	return 0;
}
