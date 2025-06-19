# si
### 1. clasificador de triangulos
```javascript
let a = Number(prompt("Escribe el primer lado del triangulo"));
let b = Number(prompt("Escribe el segundo lado del triangulo"));
let c = Number(prompt("Escribe el tercer lado del triangulo"));

function clasificar(a,b,c) {
    if (a + b <= c || a + c <= b || b + c <= a) {
        console.log ("no es un triangulo");
    } 
   else if (a === c && b === c){
        console.log ("equilatero");
    }
    else if (a === b || a === c || b === c) {
        console.log ("isoceles");
    }
    else 
   console.log("escaleno"); 

    }
 
    clasificar(a,b,c)
```
---
Metodos de arrays
---
### 1. Quitar el primer elemento de un array de frutas
```javascript
let frutas = ["manzana", "banana", "pera"];
frutas.shift()
console.log(frutas)
```
---
### 2. agregar numero al final de array de numeros
```javascript
let numeros = [1,2,3];
numeros.push(4);
console.log(numeros);
```
---
### 3. Agregar un elemento al principio de un array de palabras
```javascript
let palabras = ["noche", "día"];
palabras.unshift("amanecer");
console.log(palabras);
```
---
### 4. Eliminar el último elemento de un array de colores
```javascript
let colores = ["rojo", "verde", "azul"];
colores.pop();
console.log(colores);
```
---
### 5. Sacar una parte del array sin modificar el original
```javascript
let original = [100, 200, 300, 400, 500];
let nuevo = original.slice(1, 4);
console.log(nuevo);
```
---
### 6. Cambiar un valor dentro del array
```javascript
let animales = ["perro", "gato", "conejo"];
animales[2] = "loro";
console.log(animales);
```
---
### 7. Unir todas las palabras en un solo string
```javascript
let palabras2 = ["Hola", "esto", "es", "JS"];
let frase = palabras2.join(" ");
console.log(frase);
```
---
### 8. Ordenar un array de nombres alfabéticamente
```javascript
let nombres = ["Zoe", "Ana", "Luis"];
nombres.sort();
console.log(nombres);
```
---
### 9.  Dar vuelta el orden de un array
```javascript
let numeros2 = [5, 6, 7];
numeros2.reverse();
console.log(numeros2);
```
---
### 10. Ver si un valor está dentro del array 
```javascript
let frutas2 = ["melón", "sandía", "kiwi"];
let tieneKiwi = frutas2.includes("kiwi");
console.log(tieneKiwi);
```
---
---

## 🔁 Ejercicios con `for`, `for...in` y `for...of`

### 🔹 Sin listas (solo números o strings)

#### 1. Imprimir los caracteres de una palabra

```javascript
let palabra = "Hola";
for (let letra of palabra) {
  console.log(letra);
}
```
---
### 2. Contar del 1 al 5 usando for clásico
```javascript
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```
---
### 3. Mostrar la posición de cada letra en una palabra usando for...in
```javascript
let palabra2 = "Mundo";
for (let i in palabra2) {
  console.log(`Índice: ${i}, Letra: ${palabra2[i]}`);
}
```
---
##  Con listas (arrays)
### 4. Recorrer una lista de nombres usando for...of
```javascript
let listaNombres = ["Ana", "Juan", "Sofía"];
for (let nombre of listaNombres) {
  console.log(`Hola, ${nombre}`);
}
```
---
### 5. Imprimir índices de una lista usando for...in
```javascript
let listaColores = ["rojo", "azul", "verde"];
for (let i in listaColores) {
  console.log(i);
}
```
---
### 6. Imprimir índice y valor de cada número en un array 
```javascript
let listaNumeros = [10, 20, 30];
for (let i in listaNumeros) {
  console.log(`Índice: ${i}, Valor: ${listaNumeros[i]}`);
}
```
----
## 🧑‍💻 Ejercicios de Objetos
### 1. Crear un objeto persona con propiedades: nombre, edad y ciudad
```javascript
let persona = {
  nombre: "Carlos",
  edad: 30,
  ciudad: "Bogotá"
};
```
---
### 2. Mostrar el valor de una propiedad específica
```javascript
let libro = { titulo: "1984", autor: "Orwell" };
libro.titulo = "Rebelión en la granja";
```
---
### 3. Modificar una propiedad de un objeto libro
```javascript
let libro = { titulo: "1984", autor: "Orwell" };
libro.titulo = "Rebelión en la granja";
```
---
### 4. Agregar una nueva propiedad a un objeto auto
```javascript
let auto = { marca: "Toyota", modelo: "Corolla" };
auto.color = "rojo";
```
---
### 5. Recorrer un objeto estudiante con un bucle y mostrar claves y valores
```javascript
let estudiante = {
  nombre: "Lucía",
  edad: 22,
  carrera: "Ingeniería"
};

for (let clave in estudiante) {
  console.log(`${clave}: ${estudiante[clave]}`);
}
```
---