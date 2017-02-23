

Angular 2: Getting Started - SnapShot 1
===================

# Objetivos del Curso


 - Aprender los principales conceptos de Angular2
 - Aplicar los conceptos a través de ejercicios guiados y basados en un curso de PluralSight
 - [Angular2: GettingStarted](https://app.pluralsight.com/library/courses/angular-2-getting-started-update/table-of-contents)

![enter image description here](https://i.imgur.com/S50z7av.png)	

# Introducción

----------

**Enlaces del curso**
 - [Introduction](https://app.pluralsight.com/player?course=angular-2-getting-started-update&author=deborah-kurata&name=angular-2-getting-started-update-m1&clip=0&mode=live)
 - [First Things First](https://app.pluralsight.com/player?course=angular-2-getting-started-update&author=deborah-kurata&name=angular-2-getting-started-update-m2&clip=0&mode=live)
 - [Introduction to Components](https://app.pluralsight.com/player?course=angular-2-getting-started-update&author=deborah-kurata&name=angular-2-getting-started-update-m3&clip=0&mode=live)
 
 
**Definición**: "*Es un framework de javascript para crear aplicaciones cliente utilizando HTML, CSS y Javascript*"


**Características**
 - HTML claro (If’s, foreach’s…)
 - Databinding (OneWay, TwoWay, eventos…)
 - Basado en Módulos (desacoplamiento y reutilización)
 - Soporte nativo de comunicación con el servidor.


**Mejoras en la versión 2**
 - Más rápido (renderizado, eventos y binding)
 - Actualizado a los últimos estándares de JS
 - API simplificada y orientado a productividad


# Arquitectura de una aplicación


Una aplicacion Angular 2 está compuesta por un conjunto de componentes

![enter image description here](https://i.imgur.com/Nzr6btH.jpg)

Cada componente se compone de:
 - Una Template HTML
 - Código javascript del componente
 - Metadatos asociados al componente


![enter image description here](https://i.imgur.com/po32QHz.jpg)

Una aplicación Angular 2 contiene un módulo principal o módulo Root pero se pueden añadir más módulos para agrupar las diversas funcionalidades de una aplicación compleja.

 ![enter image description here](https://i.imgur.com/V28Dzc3.jpg)

# First Things First

## Escojer el lenguaje

Angular 2 soporta gran variedad de lenguajes. Para el curso utilizaremos TypeScript como lenguaje de desarrollo.

 - ES5
 - ES6 (transpiled)
 - **TypeScript (transpiled)** : Aporta grandes funcionalidades como strong typing, orientación a clases y objetos y facilidad de interpretación de los editores y IDE's para ofrecer intellisense, navegación a definiciones y refactoring.
 - Dart

## Escojer el editor

Al desarrollar principalmente en JS y TypeScript podemos utilizar tanto editores como IDE's para el desarrollo de nuestras aplicaciones: Atom, Eclipse, VS. En este curso utilizaremos:
 - **Visual Studio Code (Windows, Mac y Linux)**


## Creamos y ejecutamos nuestra primera aplicación

    TODO: Explicar cómo crear una nueva app con angular cli.

 
El objetivo es construir una aplicación Angular 2 con un componente simple. 
Para ellos clonamos des del repositorio una aplicación con una estructura básica y un componente básico.

**Descargamos el código, restauramos las dependencias y abrimos el proyecto**

    git clone https://github.com/tc-frontend/course_angular2_day1_snapshot1.git
    cd course_angular2_day1_snapshot1
    git checkout tags/init
    npm install
    code .
  
    
**Descripción de los pasos**

 - **npm install**  -> Instala toda las dependencias 
 
![](https://i.imgur.com/YdRTnGy.jpg)

 - **code .** -> Abre el proyecto en Visual Studio Code

 

**Compilamos y ejecutamos la aplicación**

    npm start

 - **npm start** -> Transpila el código TypeScript, levanta un servidor y lanza la aplicación en un browser.

![](https://i.imgur.com/meUZzzD.jpg) 

Una vez transpilado el código tenemos que para cada componente TypeScript ***.ts** se generan ficheros ***.js** y ***.map**.

![enter image description here](https://i.imgur.com/jxjWNLs.png)

**¿Cómo se carga el módulo principal de Angular?**

 - Se navega a **index.html**
 - En la página se realiza la carga principal del módulo root de Angular que está dentro del folder **"app"**
 - Finalmente se ejecuta el código de **main.js**

![enter image description here](https://i.imgur.com/AYJfrVs.png)

**Modificar el proyecto en ejecución**

    TODO: Explicar el BrowserSync

 

## Diferencia entre módulos ES y Módulos en Angular

    TODO: Explicar las diferencias

## Acceder a la versión final 

Si queremos ver la solucion final 

    git checkout master
    npm install
    npm start

Los pasos detallados los podemos vr en:

    https://github.com/tc-frontend/tc-frontend-angular2_day1_snapshot1/commits/master


# Introduction to Components

## Estructura de un Componente

Angular 2 soporta gran variedad de lenguajes. Para el curso utilizaremos 
 ![enter image description here](https://i.imgur.com/BCR27MK.png)
![enter image description here](https://i.imgur.com/5o7WoBo.png)

## Desarrollo de un componente

Angular 2 soporta gran variedad de lenguajes. Para el curso utilizaremos 

![enter image description here](https://i.imgur.com/j2FoQFG.png)

## Carga de módulos de Angular


![enter image description here](https://i.imgur.com/r6tcVpc.png)


## Orden en la carga de los módulos

![enter image description here](https://i.imgur.com/A6rSYMa.png)
