

Angular 2: Getting Started - SnapShot 2
===================

En esta sección cubriremos los siguientes puntos de Pluralsight:

 - Templates
 - Interpolation
 - Directives


----------


**1. Definición de templates**


----------


Las vistas o templates HTML de los componentes se pueden definir **Innine** o pueden crearse de forma separada en un fichero aparte.


La creación de un componente siempre implica:


1. Creación de un folder


2. Creación de un componente dentro del folder


3. Creación de una template dentro del folder
 
 
Ejemplo:
 
 
**- folder:** nombre_componente

**- componente:** nombre_componente.component.ts
 
**- template:** nombre_componente.component.html
 

En el momento de asociar el componente y la template definiremos en el **Decorator** la propiedad **templateUrl**:

![enter image description here](https://i.imgur.com/u60D6Nc.png)



----------


**2. Crear e importar un nuevo componente**


----------



Una vez tenemos definido un componente con una template externa tenemos que conocer la forma de importar componentes a nuestro componente **root**. 


Al exportarse el nuevo componente como **"pm-products"** tenemos la posibilidad de añadirlo directamente en la template del componente **root** de la aplicación.

![enter image description here](https://i.imgur.com/9QyfusT.png)



----------


**3. Registrar un nuevo componente**


----------


El siguiente paso será registrar el componente dentro del Módulo a fin de que el módulo cargue el componente y esté listo para su ejecución. Para ello bastará con:

1. Acceder al módulo principal.


2. Realizar un "imports" del componente.


3. Añadir el componente importado en la lista de "declarations"


![enter image description here](https://i.imgur.com/MhLBYjQ.png)



----------


**4. Interpolation**


----------


Angular mediante la interpolación permite mostrar propiedades y valores de retorno de funciones del componente dentro de las vistas HTML. 
Hay varias formas de realizar la interpolación:

![enter image description here](https://i.imgur.com/3cmzfnn.png)

![enter image description here](https://i.imgur.com/304izb3.png)



----------


**6. Directivas**


----------


Angular mediante la interpolación permite mostrar propiedades y valores de retorno de funciones del componente dentro de las vistas HTML. 
Hay varias formas de realizar la interpolación:
 

![enter image description here](https://i.imgur.com/s9MEtkg.png)



----------


**Práctica**


----------



![enter image description here](https://i.imgur.com/EW0hShu.png)


El objetivo es crear un componente que muestre una lista de productos. 
El componente tendra la plantilla en un html y tilizarelos 'templateUrl' para referenciarlo.
Dentro del comonente crearemos una propiedad que contenga un array de productos y utilizando directivas ngIf y ngFor dotaremos de logica a la plantilla. 
El resultad

Para ello clonamos el SnapShot 2 desde le primer commit de:

    git clone https://github.com/tc-frontend/course_angular2_day1_snapshot2
    cd course_angular2_day1_snapshot2
    git checkout tag/init
    npm install
    code .
 
Seguimos los pasos detallados en el historial de commits:

    https://github.com/tc-frontend/tc-frontend-angular2_day1_snapshot2/commits/master   
  
Si queremos ver la App en nuestro browser

    npm start

Si queremos ver la solucion final de este SnapShot:

    git checkout master
    npm install
    npm start



