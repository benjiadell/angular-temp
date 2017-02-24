
Angular 2: Getting Started - SnapShot 3
===================
En esta parte veremos estos contenidos del curso de Pluralshight:

 - Data Binding & Pipes


----------


### 1 - Data Binding


----------


En esta sección vamos a ver uno por uno cata tipo de binding que podemos aplicar en Angular2. Todos los tipos están ejemplificados en la siguiente imagen:


![enter image description here](https://i.imgur.com/aAYMGm0.png)


Gracias al motor de Angular cualquier modificación en ejecución de las propiedades del componente lanza el refresco de los bindings generados en la vista. 


.

 
#### Interpolation 


[Binding One-Way]


Con la interpolación lo que se consigue es poder renderizar en el HTML el valor de una propiedad o el valor de retorno de una función expuesta a través del componente.

En el momento en el que a la propiedad se le modifique el valor la vista se refrescará automáticamente.


.


#### Property Binding 


[Binding One-Way]


Con el property binding será posible bindar una propiedad a la vista pudiendo a su vez aplicar expresiones condicionales o Pipes como más adelante se verá. Sigue siendo un Binding OneWay


 - NOTA: Se puede incluso bindar estilos: **[style.width.px]='imageWitdh'**


![enter image description here](https://i.imgur.com/tes1f2h.jpg)


.


#### Event Binding


[Binding One-Way]


Con event binding podemos bindar un evento del DOM al componente TypeScript. 


Es posible generar un binding Two-way si se combina el Property Binding con el Event Binding. Podemos reaccionar a un evento del DOM y en el componente actualizar alguna propiedad que esté bindada a la vista.


 - $event: Con este binding tabién es posible enviar el payload del evento. Algo propio de javascript. Ejemplo: **(click)='metodo($event)'**


![enter image description here](https://i.imgur.com/YWzI30S.jpg)


.


#### Two-Way Binding


¿Cómo funciona el Two-Way binding? 


 - **ngModel**: es una propiedad pública de cualquier componente Angular


 - Angular por debajo crea una instancia de **FormControl**. 


 - La clase FormControl se enlazará a la propiedad **Value** del control **Input** y a su vez se enlazará a la propiedad **listFilter** del componente Angular. De esta forma FormControl no deja de ser un intermediario entre el control Input y la propiedad del componente y se encarga de propagar los cambios en ambos sentidos. [FormControl Class](https://angular.io/docs/ts/latest/api/forms/index/FormControl-class.html) 
 

- **NOTA**: Es más. Cuando se define un formulario completo en Angular con **ngForm** que se verá más adelante en este curso, en realidad lo que ocurre por debajo es que Angular está generando un **FormArray** de instancias de **FormControl** para todos los controles HTML del formulario.


- **Es necesario incluir en el componente el Módulo de Forms de Angular**: 


    import { FormsModule } from '@angular/forms'



![enter image description here](https://i.imgur.com/4gvl9Rp.jpg)


.


----------


### 2 - Pipes


----------






----------


### Práctica


----------


Para ello clonamos el **SnapShot 3** desde le primer commit:

    git clone https://github.com/tc-frontend/course_angular2_day1_snapshot3
    cd course_angular2_day1_snapshot3
    git checkout tag/init
    npm install
    code .
 
Seguimos los pasos detallados en el historial de commits:

    https://github.com/tc-frontend/tc-frontend-angular2_day1_snapshot3/commits/master   
  
Si queremos ver la App en nuestro browser

    npm start

Si queremos ver la solucion final de este SnapShot:

    git checkout master
    npm install
    npm start



