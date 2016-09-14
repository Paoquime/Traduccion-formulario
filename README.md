# Traduccion-formulario

**Usando selectores, cambia los textos que aparecen por su traducción o equivalente a español, como se muestra en las imágenes:**

![Sin titulo](http://i68.tinypic.com/29c12x4.png)

![Sin titulo](http://i68.tinypic.com/mbh1sj.png)

Los archivos que nos son entregados son: 

* index.html
* main.js(vacio)
* signin.css

1. Revisamos en el index.html cuales son las etiquetas que contienen los valores que queremos modificar, si tienen "Id", "Class" o solo están definidos en etiquetas.

2. Una vez hecho esto podemos utilizar en nuestro main.js los selectores que corresponden a cada caso en particular.

+ Solución

**En el título**

 Ya que en el archivo Html la etiqueta H2 contiene un Id, utilizamos el seletor "getElementById" para poder llamar al elemento, agregamos el atributo "innerHTML" y le asignamos el nuevo valor que seria "Por favor inicia sesión".
 
  `document.getElementById("form-signin-heading").innerHTML = "Por favor inicia sesión";`
  
**En los Placeholders**
  
 Los inputs del Html contienen Id por lo que utilizamos el seletor "getElementById" para poder llamar al elemento, agregamos el atributo "innerHTML" y le asignamos los nuevos valores que serian "Correo Electrónico" y "Contraseña".
  
 `document.getElementById("inputEmail").placeholder="Correo Electrónico";`
 
 `document.getElementById("inputPassword").placeholder="Contraseña";`
 
 **En el Checkbox**
 
 Ya que en el archivo Html tenemos un solo "span" utilizamos el selector "document.querySelector" para poder llamar al elemento, agregamos el atributo "innerHTML" y le asignamos el nuevo valor que seria "Recordar datos".
  
  `document.querySelector("span").innerHTML = "Recordar datos";`
  
 **En el Button**
  
  Ya que en el archivo Html tenemos un solo "button"  utilizamos el selector "document.querySelector" para poder llamar al elemento, agregamos el atributo "innerHTML" y le asignamos el nuevo valor que seria "Iniciar Sesión".
  
  `document.querySelector("button").innerHTML = "Iniciar Sesión";`
  
