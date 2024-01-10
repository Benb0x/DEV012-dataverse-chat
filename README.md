# Dataverse Chat 
![image](https://github.com/Benb0x/DEV012-dataverse-chat/assets/144946997/57d8cd99-f33a-419c-adf4-e2e713e85fb6)


## Índice

* [1. INTRODUCCIÓN](#1-introducción)
* [2. RESUMEN DEL PROYECTO](#2-resumen-del-proyecto)
* [3. Consideraciones generales](#3-consideraciones-generales)
* [4. Funcionalidades](#4-funcionalidades)
* [5. Consideraciones técnicas](#5-consideraciones-técnicas)
* [6. Criterios de aceptación mínimos del proyecto](#6-criterios-de-aceptación-mínimos-del-proyecto)
* [7. Objetivos de aprendizaje](#7-objetivos-de-aprendizaje)
* [8. Pistas, tips y lecturas complementarias](#8-pistas-tips-y-lecturas-complementarias)
* [9. Consideraciones para pedir tu Project Feedback](#9-consideraciones-para-pedir-tu-project-feedback)

***

## 1. INTRODUCCIÓN

Bienvenido al emocionante mundo de la interacción con videojuegos a través de nuestro innovador proyecto desarrollado durante el Bootcamp de Laboratoria en Desarrollo Web. Esta fascinante Single Page Application (SPA) te sumergirá en el universo del gaming al permitirte explorar y conversar con personajes de tus juegos favoritos.

Imagina poder filtrar y ordenar los juegos por género y punto de vista, facilitándote la búsqueda del videojuego que se ajuste a tus preferencias.

Pero aquí viene la emocionante vuelta de tuerca: hemos llevado la interactividad al siguiente nivel. ¿Alguna vez soñaste con charlar con tus juegos favoritos? En nuestra aplicación, podrás acceder a una vista detallada de cada juego, con la increíble posibilidad de interactuar con ellos a través de un sistema de chat impulsado por la potente API de OpenAI.

Imagina charlar con el protagonista de tu videojuego favorito o tener una conversación intrigante con el villano maestro del juego. Esta experiencia única te permite explorar las profundidades de los personajes de una manera nunca antes vista.

En resumen, nuestro proyecto fusiona la magia de los videojuegos con la emocionante posibilidad de entablar conversaciones con los personajes de tu elección. ¡Sumérgete en esta experiencia única y descubre un nuevo nivel de conexión con el mundo de los juegos!

![image](https://github.com/Benb0x/DEV012-dataverse-chat/assets/144946997/29c0fd40-201b-4b53-9f89-8b4b83144956)


## 2. RESUMEN DEL PROYECTO

En este proyecto convertirás la aplicación desarrollada
en Dataverse en una
[Single Page Application (SPA)](https://es.wikipedia.org/wiki/Single-page_application),
manteniendo las funcionalidades de visualizar, filtrar, ordenar y
calcular alguna estadística, adicionando una nueva vista para
consultar información detallada de cada personaje/entidad y agregando
la posibilidad de interactuar con un personaje/entidad o todos ellos
a través de un sistema de chat impulsado por la
[API de OpenAI](https://openai.com/product).

### Los objetivos generales de este proyecto son los siguientes

* Desarrollar una [Single Page Application (SPA)](https://es.wikipedia.org/wiki/Single-page_application)
* Aplicar los conceptos de responsividad en el desarrollo de las vistas
* Implementar un router para la navegación entre las diferentes
  vistas de la aplicación
* Integrar una API externa
* Entender la asincronía en JavaScript
* Crear una suite de pruebas unitarias que permitan testear código asíncrono

## 3. PROTOTIPADO

Esta aplicación web se ha desarrollado a partir de un prototipo de alta fidelidad. Este ha sido diseñado cuidadosamente para incorporar requisitos esenciales, asegurando así una plataforma fácil de usar para cualquier usuario.

El prototipo de alta fidelidad fue diseñado utilizando la aplicación Figma. En este proceso, se establecieron elementos clave, como la paleta de colores, el estilo visual y el funcionamiento inicial. Este prototipo de alta fidelidad sirve como una representación avanzada y detallada de la visión conceptual.

![image](https://github.com/Benb0x/DEV012-dataverse-chat/assets/144946997/5e068998-c1fc-4886-a4f6-142b84f2b2e3)



## 4.FUNCIONALIDADES

### `Home`

La interfaz de la primera vista (HOME) está constituida por dos filtros que nos ayudan a seleccionar el género y POV de los juegos que se muestran. También encontramos una estadística que nos indica cuántos juegos existen actualmente en la página. Contamos con un
botón para limpiar nuestros filtros y así mostrar nuestra data original. En nuestro home, encontramos un botón que nos lleva a una vista para introducir nuestra API key y poder empezar a interactuar con nuestros juegos favoritos. Por último, nos encontramos con
nuestras tarjetas, donde se muestran nuestros videojuegos con una foto y una breve descripción de cada uno.

![image](https://github.com/Benb0x/DEV012-dataverse-chat/assets/144946997/63985d35-90e8-4a36-aa19-3e2d358ff41d)

### `Detalle`

La vista de detalle ofrece una descripción detallada del juego seleccionado, proporcionando información interesante, junto con una imagen de alguno de los protagonistas. Además, cuenta con un chat que incorpora una inteligencia artificial (IA), permitiendo a los usuarios entablar conversaciones en tiempo real con los personajes del videojuego.

![image](https://github.com/Benb0x/DEV012-dataverse-chat/assets/144946997/b31faafd-e928-466c-b132-497c2330fe56)

### `ApiKey`

En la vista de la ApiKey se visualiza un campo al que deberán ingresar nuestra clave proporcionada por el sitio de OpenAI, lo que permitirá habilitar las funcionalidades de cada uno de los chats. 

![image](https://github.com/Benb0x/DEV012-dataverse-chat/assets/144946997/44a85b3c-fdfe-43da-bc8a-86e82607d62c)

### `Error`

Finalmente, al intentar acceder a un URL inválido se despliega una vista de erorr con una breve descripción y un botón que redirige nuevamente a home.

![image](https://github.com/Benb0x/DEV012-dataverse-chat/assets/144946997/70fd8c7e-482d-4272-9958-a8792d0d1169)




## 5. Consideraciones técnicas
La lógica del proyecto está implementada completamente en JavaScript (ES6), HTML y CSS.

F:\Laboratoria\DEV012-dataverse-chat\src
