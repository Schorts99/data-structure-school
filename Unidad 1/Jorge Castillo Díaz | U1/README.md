# Turtle y Ngon modificado

### Proposito del proyecto:

Agregar nuevos métodos a la clase Turtle y Ngon para mejorar su funcionalidad

### Versión del proyecto: 0.0.2

### Áutores: Jorge Castillo Díaz

### Instrucciones:

1. Compilar y ejecutar:
	* Windows:
		* Ejecutar run.bat, el script compilara y posteriormente ejecutara la clase Prueba y sus dependencias
	* Linux/Mac:
		1. Dar permisos de ejecucución a run.sh ejecutando en la terminal estando previamente en la carpeta del proyecto
		2. Ejecutar run.sh
2. Ingresar el método de pintado:
	* Métodos disponibles:
		* normal
		* normal colorido
		* invertido
		* invertido colorido
		* reversa
		* reversa colorido
		* reversa musical
3. Ingresa el número de lados de la figura deseada

```bash
$ sudo chmod+x run.sh
$ ./run.sh
```

## Métodos agregados

## Turtle

* turnRight:
  Este método le da la habilidad a la tortuga de girar a la derecha.
  * Parametros recibidos:
    * degrees: Los grados que girara a la derecha
```java
turnRight(double degrees)
```
---
* turnAround:
  * Este método le da la habilidad de dar media vuelta a la tortuga
```java
turnAround()
```
---
* goForwardWithColors:
  * Este método hace que la tortuga deje un rastro de colores al avanzar
  * Parametros recibidos:
    * steps: La cantidad de pasos a avanzar
```java
goForwardWithColors(double steps)
```
* steps: La cantidad de pasos a avanzar
* changeEvery: Cada cuantos pasos la tortuga cambiara su color
```java
goForwardWithColors(double steps, double changeEvery)
```
* steps: La cantidad de pasos a avanzar
* colors: Los colores que usara la tortuga para avanzar
```java
goForwardWithColors(double steps, Color[] colors)
```
* steps: La cantidad de pasos a avanzar
* colors: Los colores que usara la tortuga para avanzar
* changeEvery: Cada cuantos pasos la tortuga cambiara su color
```java
goForwardWithColors(double steps, Color[] colors, double changeEvery)
```
---
* goBackward:
  * Este método le da la habilidad a la tortuga de ir en reversa
```java
goBackward()
```
---
* goBackwardWithColors:
  * Este método hace que la tortuga deje un rastro de colores al retroceder
  * Parametros recibidos:
    * steps: La cantidad de pasos a retroceder
```java
goBackwardWithColors(double steps)
```
* steps: La cantidad de pasos a retroceder
* changeEvery: Cada cuantos pasos la tortuga cambiara su color
```java
goBackwardWithColors(double steps, double changeEvery)
```
* steps: La cantidad de pasos a retroceder
* colors: Los colores que usara la tortuga para avanzar
```java
goBackwardWithColors(double steps, Color[] colors)
```
* steps: La cantidad de pasos a retroceder
* colors: Los colores que usara la tortuga para avanzar
* changeEvery: Cada cuantos pasos la tortuga cambiara su color
```java
goBackwardWithColors(double steps, Color[] colors, double changeEvery)
```

## Ngon

* seleccionarMetodo:
	* Valida el método de entrada seleccionado para el pintado.
	* Parametros recibidos:
		*	método: Método seleccionado.
```java
seleccionarMetodo(String metodo)
```
---
* preguntarLados:
	* Valida la entrada del usuario y manda a llamar al método de pintado previamente seleccionado.
```java
preguntarLados()
```
---
* preguntarMetodo:
	* Maneja la entrada del usuario del método de pintado a utilizar.
```java
preguntarMetodo()
```
---
* normal:
	* Esté método hace el pintado normal implementando turnLeft de Turtle, inicialmente este era el método main.
	* Parametros recibidos:
		* lados: El número de lados de la figura a dibujar.
```java
normal(int lados)
```
---
* normalColorido:
	* Esté método hace el pintado normal implementando turnLeft de Turtle y dejando un rastro de colores a su paso.
	* Parametros recibidos:
		* lados: El número de lados de la figura a dibujar.
```java
normalColorido(int lados)
```
---
* invertido:
	* Esté método hace uso de turnRight de la clase Turtle.
	* Parametros recibidos:
		* lados: El número de lados de la figura a dibujar.
```java
invertido(int lados)
```
---
* invertidoColorido:
	* Esté método hace uso de turnRight de la clase Turtle y dejando un rastro de colores a su paso.
	* Parametros recibidos:
		* lados: El número de lados de la figura a dibujar.
```java
invertidoColorido(int lados)
```
---
* reversa:
	* Esté método hace uso de turnLeft y goBackward de la clase Turtle.
	* Parametros recibidos:
		* lados: El número de lados de la figura a dibujar.
```java
reversa(int lados)
```
---
* reversaColorido:
	* Esté método hace uso de turnLeft y goBackwardWithColors de la clase Turtle.
	* Parametros recibidos:
		* lados: El número de lados de la figura a dibujar.
```java
reversaColorido(int lados)
```

---

### Validaciones

* OpcionPintadoInvalida:
	* Se manejan 2 tipos de pintado:
		* Normal: Usando el método turnLeft de Turtle.
		* Invertido: Usando el método turnRight de Turtle.