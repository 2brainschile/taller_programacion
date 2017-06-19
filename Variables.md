# Variables en Javascript

## ¿Que es una Variable?
> Una forma de guardar algun tipo de informacion para despues usarla, y para obtener esta informacion es necesario referirse a la “Palabra” que describa esta información.

Otra forma de definir una variable es pensar en esta como un contenedor (o caja), la cual puede guardar diferentes valores.

Ej: 
```javascript
// Esto es un Comentario, No se interpreta código en esta linea

// Se define una variable con la keyword -> var
var nombreVariable = "Valor Variable"

var x = 5;
var y = 6;
var z = x + y;
```

- *Ojo: el nombre de una variable no puede llevar espacios, ni la letra Ñ, ni tampoco tildes*
- Se recomienda seguir la [convencion de nombres](https://es.wikipedia.org/wiki/Convenci%C3%B3n_de_nombres_(programaci%C3%B3n)#JavaScript) de JS que dice que las variables se tienen definir en **camelCase**, si quieres saber mas sobre convenciones de guias de estilos ver [link](https://www.w3schools.com/js/js_conventions.asp).


## Tipos de Variables
<p align="center">
  <img src="http://i.imgur.com/5eNDMI4.png" alt="Tipos de Variables"/>
</p>

### Numbers

```javascript
var variableNumEntero = 1123
var variableDecimal = 1123.1
var variableTipoNumber = 1e5
```

### Strings

```javascript
var variableTipoString = "Esta"
var variableCaracter = "E"
var variableTipoString4 = "Esta es un variable tipo String"
var variableTipoStringNumber = "123"
```

### Objects
Los Objectos son variables tambien, pero pueden contener muchos valores.


```javascript
var nombreObjeto = {}
var miObject = new Object()

// Ej de Objeto AUTO
var auto = {
    color: "rojo",
    modelo: "MARCA XXX"
}

// console
// Es un objeto que presenta varias funciones en la consola del Navegador
// la funcion que vamos a usar es -> log
// y lo que hace es mostrar una variable en la consola
// se llama asi

console.log() // muestra undefined, dado que no le pasamos ninguna variable

console.log(1) // muestra 1

console.log("Hola") // muestra HOLA

var miVariable = ":)"
console.log(miVariable) // muestra :)
```

### Functions
Las funciones son un tipo especial de Objetos, lo que hacer es entregar un resultado en base algunos parametros.

- *Las funciones en JS se definen con la palabra `function`*
```javascript

function nombreFuncion(){
    // Código que realice alguna acción.
}

// EJ: 
// FUNCION SIN PARAMETROS
function imprimirUno(){
    console.log(1)
}

// Para llamar a una función es necesario poner el nombre de la funcion seguido de parentesis

// ejecutar funcion imprimirUno
imprimirUno() // muestra 1

//FUNCION CON PARAMETROS
function imprimir(parametro){
    console.log(parametro)
}

imprimir(2) // Muestra 2
imprimir("letra") // Muestra letra
imprimir(false) // Muestra false

```

### Actividad IVA
```javascript

// CALCULAR IVA
var valorNeto = 1000
function calcularIVA(){
    var valorIVA = valorNeto * 0.19;
    console.log(valorIVA)
}

calcularIVA()

valorNeto = 200
calcularIVA()


function calcularIVAconParametro(parametro){
    var valorIVA = parametro * 0.19;
    console.log(valorIVA)
}

calcularIVAconParametro(1000)
calcularIVAconParametro(200)
```