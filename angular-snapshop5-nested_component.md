Angular 2: Getting Started - SnapShot 5
===================
En esta parte veremos estos contenidos del curso de Pluralshight:

 - Building Nested Components


----------


### 1 - Building Nested Components


----------


Un nested component es un componente que renderiza una pequeña parte visual de la pantalla y que puede ser reutilizado por varios componentes en varias vistas.


 - El ejemplo clásico de un Nested Component es aquell que se utiliza para ser renderizado en cada una de las filas de una lista o de una tabla.


 - Ejemplo: Mostrar una lista de Clientes: Se crea un nested component con el detalle del cliente en formato "row"


![enter image description here](https://i.imgur.com/lexsIP7.png)


.


----------


### 2 - Building & using a Nested Component


----------


Un nested component es un componente igual que los demás en Angular la diferencia radica en que dicho componente se crea para dividir las pantallas en vistas parciales o componentes pequeños e individuales y reutilizables.


En el ejemplo siguiente podemos ver la siguiente estructura de componentes:


**product-list.component.ts** : que se encarga de mostrar una lista de productos


**star.component.ts** : nested component que se utiliza en la lista de productos para mostrar el rating de cada uno de los productos.


![enter image description here](https://i.imgur.com/cCXekr0.jpg)


**No hay que olvidar registrar el componente en el módulo.**


![enter image description here](https://i.imgur.com/IRSuvZs.jpg)


.


----------


### 3 - Passing Data to Nested Component using @Input


----------


#### ¿Cómo publicamos propiedades des de nuestro nested component?


Con la directiva **@Input**. 


De esa forma conseguimos que la propiedad se pueda utilizar des de los **"componentes padre"**. El ejemplo a continuación:



![enter image description here](https://i.imgur.com/0DNcdIm.jpg)


.


----------


### 4 - Passing Data from Nested Component using @Output


----------


#### ¿Cómo podemos publicar eventos des de nuestro nested component?


Con la directiva **@Output**


Con la directiva estamos indicando que se tratará de un evento expuesto a través de nuestro componente y con el uso de la clase **EventEmmitter<>** que nos permitirá lanzar dicho evento cuando la lógica lo requiera.


![enter image description here](https://i.imgur.com/GGJkV4Y.jpg)


.


----------


### 5 - Práctica


----------

En esta seccion el objetio es crear un Nested Component, en concreto, a Star Component para las puntuaciones del producto.


![enter image description here](https://i.imgur.com/IPI3bLi.png)



Para ello clonamos el **SnapShot 5** desde le primer commit de:


    git clone https://github.com/tc-frontend/course_angular2_day1_snapshot5
    git checkout HEAD~1
    npm install
    code .

 
Seguimos los pasos detallados en el historial de commits:


    https://github.com/tc-frontend/tc-frontend-angular2_day1_snapshot5/commits/master   

  
Si queremos ver la App en nuestro browser


    npm start


Si queremos ver la solucion final de este SnapShot:


    git checkout master
    npm install
    npm start



