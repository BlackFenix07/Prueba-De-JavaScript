# Test de JavaScript

¡Es hora de poner a prueba cuánto sabes sobre JavaScript!

Esta lectura es una prueba de JavaScript. A diferencia de un examen, nadie te obligará a nada. **Puedes hacer trampa y saltar a la siguiente clase**, ese es el camino fácil. Pero tengo mucha fe en ti, confío en que seguirás mis consejos y no avanzarás a la siguiente clase hasta superar esta prueba.

## Instrucciones para tomar esta prueba

- Evalúa muy críticamente tu conocimiento.
- Si logras resolver la prueba, no importa cuánto te cueste, puedo asegurarte que tienes todo para continuar a las siguientes clases y tomar el resto del curso.
- Si no lo logras, no te preocupes, absolutamente nadie puede juzgarte, solo tú. Vuelve al [Curso Básico de JavaScript](https://platzi.com/cursos/basico-javascript/), anota los temas clave donde puedes mejorar, ubica las clases donde puedes aprenderlos y estudia vigorosamente.
- Es completamente válido hacer búsquedas en Google, cursos y tutoriales de Platzi, incluso usar tu cuaderno de notas sin importar si es físico o virtual.

Recuerda que **el éxito no se mide por cuánto tiempo te toma aprender**, esa métrica es relativamente inútil. Mejor concéntrate en completar los cursos de tu ruta de aprendizaje profesional y desarrollar los proyectos que realmente demuestran que dominas cada tecnología.

¡Mucha suerte!


## Variables y operaciones

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una variable y para qué sirve?
    Las variables son espacios en memoria donde se puede guardar información dependiendo de los tipos y estructuras de datos que soporte nuestro lenguaje.

- ¿Cuál es la diferencia entre declarar e inicializar una variable?
    Declarar es cuando le decimos a JavaScript que vamos a crear una variable con x nombre mientras que inicializar o reinicializar es asignarle un valor a esa variable.

- ¿Cuál es la diferencia entre sumar números y concatenar strings?
- ¿Cuál operador me permite sumar o concatenar?
    El operador que permite sumar o concatenar es +. Este operador permite sumar números cuando lo usamos con números, pero cuando lo usamos con strings los concatena.

### 2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

- Nombre: string
- Apellido: string
- Nombre de usuario en Platzi: string
- Edad: number
- Correo electrónico: string
- Mayor de edad: boolean
- Dinero ahorrado: number
- Deudas: number

### 3️⃣ Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.

```js
let nombre = "Andrés";
let apellido = "Zapata";
let username = "BlackFenix";
let edad = 23;
let mail = "andresmauricio030400@gmail.com";
let esMayorDeEdad = true;
let dineroAhorrado = 1000;
let deudas = 100;
```

### 4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

```js
let nombreCompleto = nombre + " " + apellido;
let dineroReal = dineroAhorrado - deudas;
```

## Funciones

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una función?
    Las funciones permiten encapsular (guardar) bloques de código para reutilizarlos y ejecutarlos en el futuro.

- ¿Cuándo me sirve usar una función en mi código?
    Sirve cuando tenemos variables o bloques de código muy parecidos que podemos encapsular para reutilizar más de una vez en el futuro. También sirve para ordenar y mejorar la legibilidad de nuestro código.

- ¿Cuál es la diferencia entre parámetros y argumentos de una función?
    Las funciones reciben parámetros cuando las creamos y argumentos cuando las ejecutamos.

### 2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

```js
const name = "Andrés Mauricio";
const lastname = "Zapata Rico";
const completeName = name + lastname;
const nickname = "BlackFenix";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");
```


## Condicionales

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un condicional?
    Es la forma en la que ejecutamos un bloque de código u otro dependiendo de alguna condición o validación.
- ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
    If (else y else if) y Switch. El condicional if (else y else if) permite hacer validaciones completamente diferentes (si así queremos) en cada condicional o validación. En cambio, en el switch todos los cases se comparan con la misma variable o condición que definimos en el switch.

- ¿Puedo combinar funciones y condicionales?
    Sí. Las funciones pueden encapsular cualquier bloque de código incluyendo condicionales.

### 2️⃣ Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

```js
const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
   case "Free":
       console.log("Sólo puedes tomar los cursos gratis");
       break;
   case "Basic":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
       break;
   case "Expert":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
       break;
   case "ExpertDuo":
       console.log("Tú y alguien más pueden tomar todos los cursos de Platzi durante un año");
       break;
}
```

```js
const tipoDeSuscripcion = "Basic";

if (tipoDeSuscripcion === "Free") {
    console.log("Sólo puedes tomar los cursos gratis");
} else if (tipoDeSuscripcion === "Basic") {
    console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
} else if (tipoDeSuscripcion === "Expert") {
    console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
} else if (tipoDeSuscripcion === "ExpertDuo") {
    console.log("Tú y alguien más pueden tomar todos los cursos de Platzi durante un año");
} else {
    console.log("Ese tipo de suscripción no existe");
}
```

### 3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).

```js
function tipoDeSuscripcion(suscripcion) {
    if (suscripcion === "Free") {
        console.log("Sólo puedes tomar los cursos gratis");
        return;
    } 
    
    if (suscripcion === "Basic") {
        console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
        return;
    } 
    
    if (suscripcion === "Expert") {
        console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
        return;
    } 
    
    if (suscripcion === "ExpertDuo") {
        console.log("Tú y alguien más pueden tomar todos los cursos de Platzi durante un año");
        return;
    }
    console.warn ("Ese tipo de suscripción no existe");
}
console.log(tipoDeSuscripcion("Free"));
```

> 💡 Bonus: si ya eres una experta o experto en el lenguaje, te desafío a comentar cómo replicar este comportamiento con arrays u objetos y un solo condicional. 😏

```js
const tiposDeSuscripciones = {
    free: "Sólo puedes tomar los cursos gratis",
    basic: "Puedes tomar casi todos los cursos de Platzi durante un mes",
    expert: "Puedes tomar casi todos los cursos de Platzi durante un año",
    expertDuo: "Tú y alguien más pueden tomar todos los cursos de Platzi durante un año"
}

function conseguirTipoDeSuscripcion(suscripcion) {
    if (tiposDeSuscripciones[suscripcion]) {
        console.log(tiposDeSuscripciones[suscripcion]);
        return;
    }
    console.warn("Ese tipo de suscripción no existe");
}
```

## Ciclos

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un ciclo?
    Es la forma de ejecutar un bloque de código hasta que se cumpla cierta condición.
- ¿Qué tipos de ciclos existen en JavaScript?
    While, Do While y For.
- ¿Qué es un ciclo infinito y por qué es un problema?
    Es cuando la validación de nuestros condicionales nunca se cumple y esto es un problema ya que termina dañando la aplicación.
- ¿Puedo mezclar ciclos y condicionales?
    Sí. Aunque los ciclos son una especie de condicionales, nada impide agregar más condicionales dentro de ellos.

### 2️⃣ Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

```js
for (let i = 0; i < 5; i++) {
    console.log("El valor de i es: " + i);
}
```

```js
let i = 0;

while (i < 5) {
    console.log("El valor de i es: " + i);
    i++;
}
```

```js
for (let i = 10; i >= 2; i--) {
    console.log("El valor de i es: " + i);
}
```

```js
let i = 10;

while (i >= 2) {
    console.log("El valor de i es: " + i);
    i--;
}
```

### 3️⃣ Escribe un código en JavaScript que le pregunte a los usuarios cuánto es `2 + 2`. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

> 💡 Pista: puedes usar la función prompt de JavaScript.

```js
let respuesta = prompt("Cuánto es 2 + 2?");

while (respuesta != "4") {
    let pregunta = prompt("Cuánto es 2 + 2?");
    respuesta = pregunta;
}
```

## Listas

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un array?
    Es una lista de elementos.

- ¿Qué es un objeto?
    Es una lista de elementos pero cada elemento tiene un nombre clave.

- ¿Cuándo es mejor usar arrays u objetos?
    Arrays cuando lo que haremos en un elemento es lo mismo que en todos los demás (la regla se puede incumplir). Mientras que objetos cuando los nombres de cada elemento son importantes para nuestro algoritmo.

- ¿Puedo mezclar arrays con objetos o incluso objetos con arrays?
    Sí. Los arrays pueden guardar objetos y los objetos pueden guardar arrays en sus propiedades.

### 2️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

```js
function imprimirPrimerElementoArray(arr) {
        console.log(arr[i]);
    }
```

### 3️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

```js
const arr = ["Andrés", "Zapata", 23, "Ajiaco"];
console.log(arr);

function imprimirElementoPorElemento(arr) {
    for (let i = 0; i < arr.length; i++) {
        console.log(arr[i]);
    }
}
console.log(imprimirElementoPorElemento(arr));
```

### 4️⃣ Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).

```js
const obj = {
    nombre: "Andrés",
    apellido: "Zapata",
    edad: 23,
    comidaFavorita: "Ajiaco"
}
console.log(Object.values(obj));

function imprimirElementoPorElementoObjeto(obj) {
    const arr = Object.values(obj);
    for (let i = 0; i < arr.length; i++) {
        console.log(arr[i]);
    }
}
console.log(imprimirElementoPorElementoObjeto(obj));
```

## ¿Cómo te fue? 🏆

**¡Felicidades por completar la prueba de JavaScript!** Confío en que hayas completado cada paso y hayas pausado para repasar los temas de los ejercicios que se te complicaron.

Ahora sí, continúa a la siguiente clase, pero recuerda que **ya no puedes abandonar el curso**, debes completarlo hasta el final. No importa cuánto tiempo te tome. **Yo sé que tú puedes. Y tú deberías de saberlo también.**

¡Te espero en la siguiente clase para comenzar!