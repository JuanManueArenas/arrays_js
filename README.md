# arrays_js

- Un array es una zona de almacenamiento continuo, donde se pueden introducir varios valores cada uno de ellos ubicados por la posicion que ocupa en el array
- Tambien son llamados como arreglos o vectores, y cuando son de dos dimensiones son llamados matrices.
- Los arrays nos brindan la capacidad de almacenar una coleccion de elementos y acceder a ellos de manera indivudual.
-Cada elemento se identifica mediante su posicion en el array denominada indice y estos **indices** son siempre secuenciales
- En javascript son altamente flexibles en terminos de los diferentes tipos de datos que podemos almacenar en cada posicion del array

## Crear un array 

1. Declarando un array con elementos en linea

```Javascript
let miArray = [1,2,3]:
console.log(miArray);
```

2. Declarando un array con la sintaxis **new Array()**

```Javascript
let miArray = new Array(1,2,3);
console.log(miArray);
```

3. Declarando un array con un tamaño especifico utilizando la sintaxis **new Array** y asignando valores despues:

```Javascript
let miArray = new Array(3);
miArray[0] = 1;
miArray[1] = 2;
miArray[2] = 3;
console.log(miArray);
```

4. Declarando un array con diferentes tipos de datos

```Javascript
let miArray4 = [1, "dos", tres, {nombre: "Juan", edad:30}];
console.log(miArray4);
```

## Accediendo a la informacion de un array

### propiedad length
- Devuelve la cantidad de elementos del array

### Operador [pos]
- Permite acceder para leer o modificar el elemento pos del array

### Metodo at(pos)
- Devuelve el elemento de la posicion pos. El parametro admite valores negativos, lo que significa que empiezan a contar por el final del array.

```Javascript   
const letters = ["A","B","C"];
console.log(letters.length);
console.log(letters[2]);
console.log(letters[5]);
```

## Añadir o eleminar elementos
- push(ele1, ele2): añade uno o varios elementos al final del array. Devuelve el tamaño del aray

```Javascript
let miArray = [1, 2, 3];
mi array.push(4); // Agrega el elemento 4 al final del array
console .log(miArray);
```

- pop(): devuelve el ultimo elemento del array y lo elimina 
```Javascript
let miArray = [1,2,3];
miArray.pop(); //Elimina el ultimo elemento del array
console.log(miAarray);
```

- unsihift(ele1, ele2): añade uno a varios elementos al inicio, devolviendo el tamaño del array despues de añadidos
```Javascript
let miArray = [1,2,3,];
miArray.unshift(0);// agrega el element 0 al inicio del array
console.log(miArray);
```

```
```

```Javascript
let miArry = [1,2,3];
miAray.unshift(0); // agrega el elemento cero al inicio del array
console.log(miArray);
```
- concat(ele1, ele2): concatenaa dos arrays

```Javascript
let miArry = [1,2,3];
miAray.shift(0); // agrega el elemento cero al inicio del array
console.log(miArray);
```

- split(separado): a partir de una cadena,crear un array y dividiendo dicha cadena en elementos delimitados por separador

```Javascript
let miString ="Hola, ¿como estas?";
let miArray = miString.split("");
console.log(miArray);
```

- join(separador): a partir de un array, crea una cadena 

```Javascript
let miArray =["Hola,", "¿como", "estas?"];
let miString = miArray.join(" ");
console.log(miString);
```
## Busqueda de elemetos en un array

- includes(elemento): devuelve true o false si el elemento existe o no dentro del array
- indexOf(elemento): decuelve la posicion dde la primera aparicion del elemento. si no existe, devuelve -1.
- lastIndexOf(elemento): devuelve la posicion de la ultima aparacion del elemento. Si no existe, devuelve -1.

## Modificar el array o crear fragmentos 
- slice(inicio, fin): devuelve un array con los elementos desde la posicion inicio hasta la posicion fin, ambos excluidos.

## Ordenar elementos de un array 
- reverse(): invierte el orden de los elementos del array
- sort(): Ordena el array fabeticamente
-sort(criterio): ordena el array con el criterio determinado por la funcion criterio.

## Borrar elementos de un array
- Se puede borrar el contenido de un elemento de un array poniendo su valor a nul o asignando una cadena vacia " ".
- Para eliminar completamente un elemento del array se utiliza el operador delete

## Recorrido de un array
1. Recorrer con un bucle clasico pasando por todos los elementos.
```Javascript
var dias = ["lunes","martes","miercoles","jueves","viernes","sabado","domingo"];
var i = 0
for(i=0;1<dias.length;1++)
{
    console.log(dias(i));i++;
}

```

2. Recorrer con un while clasico pasando por todos los elementos.
```Javascript
var dias = ["lunes","martes","miercoles","jueves","viernes","sabado","domingo"];
var i = 0
while(i<dias.length)
{
    console.log(dias(i));i++;
}

```
3. usando la sentencia for... in 
```Javascript
var dias = ["lunes","martes","miercoles","jueves","viernes","sabado","domingo"];
var i = 0
for(let inde in dias)
{
    console.log(dias(index));
}

```
## Arrays multidimensionales```

```Javascript
const matrix = [
    [1,2,3]
    [4,5,6]
    [7,8,9]
];
```
- Recorrer una matriz utilizando bucles anidados
```Javascript
var dias = ["lunes","martes","miercoles","jueves","viernes","sabado","domingo"];
var i = 0
for(let i = 0;i<matriz.length;i++)
{
   for(let j=0;matriz.length; j++)
   {
    console log(matriz[i][j]);
   }
}
```

# Ejercicios

1. Dada una lita de numeros separador por coma, calcular la suma, el mayor, el menor y la media de todos.

2. Introducir dos cadenas con elementos separados por coma, y con un boton la dos cadenas y mostrarlas en pantalla

3. Introducir uno a uno los elementos en un array a traves de un boton. Con el boton se va eliminado el ultimo elemento. Siempre que pulse alguno de los otros de debe mostrar el contenido del array

4. Introducir un conjunto de numeros separados por comas. CUando se pulsa el boton "Pares" Cargar una tabla con los numeros introducidos y luego crear otra que solo incluya los numeros pares y mostrarla.