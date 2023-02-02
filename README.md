# Cifrador-alura
Programa para crear encriptador web
HTML CSS JV
# Encriptador de Texto | Challenge ONE - Oracle Next Education


---

Este es el primer Challenge del programa ONE - Oracle Next Education, donde se nos solicitó hacer un encriptador de texto, donde se podrá intercambiar mensajes secretos con otras personas que sepan el secreto de la encriptación utilizada.

---

Las "llaves" de encriptación que se utilizaron son las siguiente:  
  
  - La letra "e" es convertida para `"enter"`
  - La letra "i" es convertida para `"imes"`
  - La letra "a" es convertida para `"ai"`
  - La letra "o" es convertida para `"ober"`
  - La letra "u" es convertida para `"ufat"`

---

**Requisitos:**  
  - Debe funcionar solo con letras minúsculas.
  - No deben ser utilizados letras con acentos ni caracteres especiales.
  - Debe ser posible convertir una palabra para la versión encriptada también devolver una palabra encriptada para su versión original.  

**Por ejemplo:** `"gato" => "gaitober"` `"gaitober" => "gato"`

---

**Tecnologías utilizadas:**  
<img src="https://img.icons8.com/color/344/html-5--v1.png" alt="html" width="50"/>
<img src="https://img.icons8.com/color/344/css3.png" alt="css" width="50"/>
<img src="https://img.icons8.com/color/344/javascript--v1.png" alt="JavaScript" width="50"/>

---



---


---

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Challenge Alura - Cifrador</title>
    <!--======LINK CSS======-->
    <link rel="stylesheet" href="./assets/css/style.css" />
    <link rel="icon" href="./assets/img/favicon-32x32.png" />
    <!--======REMIX ICON CDN======-->
    <link
      href="https://cdn.jsdelivr.net/npm/remixicon@2.5.0/fonts/remixicon.css"
      rel="stylesheet"
    />
  </head>
  <body>
    <div class="container">
      <div class="logo">
        <img
          class="logo-img"
          src="./assets/img/logo-alura.png"
          alt="Logo Alura Latam"
        />
      </div>
      <div class="left">
        <input
          id="text-input"
          class="text-input"
          type="text"
          placeholder="Ingrese el texto aquí"
        />
      </div>
      <div class="right">
        <img
          id="right-image"
          src="./assets/img/muneco-alura.png"
          alt="Imagen muñeco Alura"
        />
        <h2 id="text-error">Ningún mensaje fue encontrado</h2>
        <textarea name="text-encrypt" id="text-encrypt" cols="30" rows="7" readonly>Ingresa el texto que desees encriptar o desencriptar.</textarea>
        <button type="button" name="button" id="copy" onclick="copy()">Copiar</button>
      </div>
      <div class="left-button">
        <p><i class="ri-error-warning-fill"></i> Solo minusculas y sin acentos</p>
        <button type="button" id="btn-encrypt" onclick="encrypt()">Encriptar</button>
        <button type="button" id="btn-decrypt" onclick="decrypt()">Desencriptar</button>
      </div>
    </div>

    <!--======SWEETALERT CDN======-->
    <script src="//cdn.jsdelivr.net/npm/sweetalert2@11"></script>
    <!--======LINK JS======-->
    <script src="./assets/js/main.js"></script>
  </body>
</html>
