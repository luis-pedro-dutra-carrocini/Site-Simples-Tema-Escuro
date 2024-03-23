# Site Simples com Tema-Escuro

Site desenvolvido durante o curso de Criação de Site Simples usando HTML, CSS e JAVASCRIPT - Fundação Bradesco, servindo como uma breve introdução as linguagens citadas. Sua função é mudar o tema da página, para escuro ou para claro.


## 📄 Descrição

Para obter uma cópia basta baixar o arquivos contidos nesse repositório, executar o arquivo em um navagador (Chrome, Edge, FireFox, etc.).


## 🚀 [Link do Site](https://meusitetestefatec.000webhostapp.com/Site_Simples/index.html)


## 📦 Aparência

<img src="/prints/print1.png">
<img src="/prints/print2.png">


## ⚙️ Código Fonte

* HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <title>Site Simples</title>
 <link rel="stylesheet" href="main.css">
</head>

<body class="light-theme">
<h1>Taks List</h1>
<p id="msg">Current tasks:</p>
<ul>
 <li class="list">Add visual styles</li>
 <li class="list">Add light and themesstyles</li>
 <li>Eneble switching the theme</li>
</ul>
<div>
 <button class="btn">Dark</button>
</div>

<script src="app.js"></script>
<noscript>Você precisa ativar o JavaScript para vsisualizar todo o site.</noscript>
</body>
</html>
```

* css
```
:root {
 --green: #00FF00;
 --white: #ffffff;
 --black: #000000;
}

* {
 color: var(--fontColor);
 font-family: helvetica;
}

body {
 background: var(--bg);
}

ul {
 font-family: helvética;
}

li {
list-style: circle;
}

.list {
list-style: square;
}

.light-theme {
 --bg: var(--green);
 --fontColor: var(--black);
 --btnBg: var(--black);
 --btnFontColor: var(--white);
}

.dark-theme {
 --bg: var(--black);
 --fontColor: var(--green);
 --btnBg: var(--white);
 --btnFontColor: var(--black);
}

.btn {
 color: var(--btnFontColor);
 background-color: var(--btnBg);
}

.btn {
 position: absolute;
 top: 20px;
 left: 250px;
 height: 50px;
 width: 50px;
 border-radius: 50%;
 border: none;
 color: var(--btnFontColor);
 background-color: var(--btnBg);
}

.btn:focus { outline-style: none; }
```

* JAVASCRIPT
```
'use strict'

const switcher = document.querySelector('.btn');

switcher.addEventListener('click', function() {
 document.body.classList.toggle('dark-theme')

 var className = document.body.className;
 if(className == "light-theme") {
  this.textContent = "Dark";
 }
 else{
  this.textContent = "Light";
 }

 console.log('current class name: ' + className);
});
```

## 🛠️ Construído com

* Visual Studio Code - Editor de Código-Fonte;
* HTML5 - Linguagem de Marcação;
* CSS- Linguagem Web de Formatação;
* JAVASCRIPT- Linguagem de Programação;


## ✒️ Autor

* **Luís Pedro Dutra Carrocini** - *Desenvolvimento do Código-Fonte;*


## 🎁 Expressões de gratidão

* Conte a outras pessoas sobre este projeto 📢;
* [Inspiração](https://mattfarley.ca/](https://www.ev.org.br/cursos/crie-um-site-simples-usando-html-css-e-javascript)https://www.ev.org.br/cursos/crie-um-site-simples-usando-html-css-e-javascript); 
