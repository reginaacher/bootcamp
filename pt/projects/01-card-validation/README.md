# Cartão de Crédito Válido

## Índice

* [1. Preâmbulo](#1-preámbulo)
* [2. Resumo do Projeto](#2-resumen-del-proyecto)
* [3. Objetivos de aprendizagem](#3-objetivos-de-aprendizaje)
* [4. Considerações Gerais](#4-consideraciones-generales)
* [5. Critérios mínimos de aceitação do projeto](#5-criterios-de-aceptación-mínimos-del-proyecto)
* [6. Dicas e leituras adicionais](#6-pistas-tips-y-lecturas-complementarias)

***

## 1. Preâmbulo

O algoritmo de Luhn, também chamado de módulo 10, é um método de soma de verificação, usado para validar números de identificação; como o IMEI de telefones celulares, cartões de crédito etc.

Este algoritmo es simple. Obtenemos la reversa del número a verificar (que solamente contiene dígitos [0-9]); a todos los números que ocupan una posición par se les debe multiplicar por dos, si este número es mayor o igual a 10, debemos sumar los dígitos del resultado; el número a verificar será válido si la suma de sus dígitos finales es un múltiplo de 10.

![gráfica de algoritmo de Luhn](https://www.101computing.net/wp/wp-content/uploads/Luhn-Algorithm.png)

## 2. Resumo do Projeto

Neste projeto, você precisará criar um aplicativo da Web que permita ao usuário validar o número de um cartão de crédito.  Além disso, você precisará implementar a funcionalidade para ocultar todos os dígitos de um cartão, exceto os quatro últimos.

O tema é livre. Você deve pensar em quais situações da vida real um cartão de crédito precisaria ser validado e em como deveria ser a experiência do usuário (telas, explicações, mensagens, cores, marca?) Etc.

## 3. Objetivos de Aprendizagem

Trabalhando em pares, eles aprenderão a criar um aplicativo Web que irá interagir com o usuário final através do navegador, usando HTML, CSS e JavaScript como tecnologias.

Simplificando, você aprenderá a:

* Organizar seu tempo e priorizar tarefas em um ambiente de alta insegurança.
* Compreender as necessidades do usuário e como propor uma solução.
* Compreendr a importância do processo de prototipagem durante a criação de um produto digital.
* Conhecer os princípios básicos do design visual.
* Usar tags HTML semânticas e os elementos de formulário.
* Mostrar elementos do formulário na tela usando **HTML** e **CSS**.
* Empregar diversos tipos de seletores em CSS: de elemento, de tipo, de ID.
* Empregar o modelo de caixa CSS (borda, margem, preenchimento).
* Determinar as regras de estilo em CSS.
* Permitir ao usuário interagir com elementos do DOM e fazer com que o aplicativo responda quando ocorrerem esses **eventos do DOM**.
* Manipular _**strings**_ (cadeias de texto).
* Empregar controle de fluxo (loops, condicionais, ...).
* Atualizar a tela com os resultados (manipular o DOM) mediante **innerHTML** o **textContent**.
* ** Implementar funções **, dada uma descrição do seu comportamento.
* Verificar se suas funções realizam as coisas para as quais foram criadas (** testes de unidade </em>) com [ Jest ](https://jestjs.io/es-ES/) **).
* Configure sua conta git.
* Realizar _ bifurque _ e _ clonar _ o repositório do projeto.
* Manter atualizadas as alterações em seu repositório remoto (commit, pull, push).
* Implantar seu projeto nas [ Páginas do GitHub ](https://pages.github.com).

## 4. Considerações Gerais

* A equipe de treinadores fornecerá a você sugestões de horários e orientações sobre como trabalhar sozinho ou em equipe. Lembre-se que cada pessoa aprende em um ritmo diferente.
* O projeto será entregue carregando seu código no GitHub (commit / push) e a interface será implantada usando as páginas do GitHub. Caso desconheça o GitHub não se preocupe, o conhecerá ao longo do projeto.

## 5. Critérios mínimos de aceitação do projeto

Empregue apenas caracteres numéricos (dígitos) no cartão para validar [0-9].

### Definição do Produto

No ` README.md `, conte-nos como você pensou sobre os usuários e qual foi seu processo para definir o produto final a nível da experiência e da interface.

* Quem são os principais usuários do produto.
* Quais os objetivos de estes usuários em relação a seu produto.
* Como você acha que o produto que está criando resolverá os problemas deles.

### Interface do usuário (UI)

A interface deve permitir ao usuário:

* Inserir o número que desejamos validar.
* Constatar se o resultado é válido ou não.
* Oculte todos os dígitos do número do cartão menos os últimos 4 caracteres.
* Não deve poder inserir um campo vazio.

### UX (Design da experiência do usuário)

Antes de começar a codificar, você deve entender o problema que deseja resolver e como o aplicativo o resolve.

* Trabalhe seu primeiro protótipo com papel e lápis (preto e branco).
* Em seguida, valide esta solução com um companheiro (peça feedback).
* Use o aprendizado no momento de validar seu primeiro protótipo e desenvolva um novo protótipo empregando alguma ferramenta para desing de protótipos([ Balsamiq ](https://balsamiq.com/), [ Figma ](https://www.figma.com/), [ Slides do Google ](https://www.google.com/intl/es/slides/about/), etc.) Esses pontos serão apresentados no ` README.md `.

### Scripts / Arquivos

#### Geral

##### `README.md`

Ele deve conter o seguinte:

* Um título com o nome do seu projeto.
* Um resumo de 1 ou 2 linhas sobre o seu projeto.
* A imagem final do seu projeto.
* Pesquisa UX:
  1. Explicar quem irá usá-lo e os objetivos quanto ao produto.
  2. Explicar como o produto resolve os problemas / necessidades desses usuários.
  3. Em seguida, você colocará a foto do seu primeiro protótipo no papel.
  4. Adicione um resumo do feedback recebido indicando as melhorias a serem feitas.
  5. Imagem do protótipo final.

#### Visualmente (HTML e CSS)

Você precisará definir exatamente o protótipo final que você criou na ferramenta de design, de protótipo que você escolheu usando HTML e CSS. Nesse momento, você escolherá as cores, o tipo de fonte etc. que irá usar.

Abaixo, descrevemos os arquivos que você usará:

##### `src/index.html`

Este arquivo contém o conteúdo que será mostrado ao usuário (esqueleto HTML). Você encontrará três marcadores iniciais que, se você quiser, pode excluir e começar do zero:

* `<header>`: cabeçalho do seu projeto.
* `<main>`: conteúdo principal do seu projeto.
* `<footer>`: rodapé do seu projeto.

##### `src/style.css`

Este arquivo deve conter as regras de estilo. Queremos que você escreva suas próprias regras, é por isso que o uso de estruturas CSS (Bootstrap, materialize etc.) NÃO é permitido.

#### Funcionalmente (JavaScript - testes de unidade)

* A lógica do projeto deve ser totalmente implementada em JavaScript.
* NÃO é permitido usar bibliotecas ou estruturas neste projeto, apenas JavaScript puro, também conhecido como JavaScript Vanilla.
* A pseudo variável `this`  não se deve ser utilizada.

Você terá 2 arquivos JavaScript que separam responsabilidades, eis o que você fará em cada arquivo:

##### `src/validator.js`

Aqui você escreverá as funções necessárias para que o usuário possa verificar o cartão de crédito e ocultar os dígitos do número do cartão. Esta função deve ser pura e independente do DOM.

Para isso, você deve implementar o ** validador de objeto ` ` **, que já está _ exportado _ no _ padrão _. Este objeto (`validator`) contiene dos métodos (`isValid` y `maskify`):

* **`validator.isValid(creditCardNumber)`**: `creditCardNumber` es un `string` con el número de tarjeta que se va a verificar. Esta función debe retornar un `boolean` dependiendo si es válida de acuerdo al [algoritmo de Luhn](https://es.wikipedia.org/wiki/Algoritmo_de_Luhn).

* **`validator.maskify(creditCardNumber)`**: `creditCardNumber` es un `string` con el número de tarjeta y esta función debe retornar un `string` donde todos menos los últimos cuatro caracteres sean reemplazados por un numeral (`#`) o 🐱. Esta función deberá siempre mantener los últimos cuatro caracteres intactos, aún cuando el `string` sea de menor longitud.

    Ejemplo de uso

    ```js
    maskify('4556364607935616') === '############5616'
    maskify(     '64607935616') ===      '#######5616'
    maskify(               '1') ===                '1'
    maskify(               '')  ===                ''
    ```

##### `src/index.js`

Acá escribirás todo el código que tenga que ver con la interacción del DOM (seleccionar, actualizar y manipular elementos del DOM y eventos). Es decir, en este archivo deberás invocar las funciones `isValid` y `maskify` según sea necesario para actualizar el resultado en la pantalla (UI).

##### `test/validator.spec.js`

En este archivo tendrás que completar las pruebas unitarias de las funciones `validator.isValid(creditCardNumber)` y `validator.maskify(creditCardNumber)` implementadas en `validator.js` utilizando [Jest](https://jestjs.io/es-ES/). Tus pruebas unitarias deben dar un 70% en _coverage_ (cobertura), _statements_ (sentencias), _functions_ (funciones) y _lines_ (líneas); y un mínimo del 50% de _branches_ (ramas).

***

## 6. Pistas, tips y lecturas complementarias

### Primeros pasos

1. Antes que nada, asegúrate de tener un :pencil: editor de texto en condiciones, algo como [Atom](https://atom.io/) o [Code](https://code.visualstudio.com/).
2. Para ejecutar los comandos a continuación necesitarás una :shell: [UNIX Shell](https://github.com/Laboratoria/bootcamp/tree/master/topics/shell), que es un programita que interpreta líneas de comando (command-line interpreter) así como tener [git](https://github.com/Laboratoria/bootcamp/tree/master/topics/scm/01-git) instalado. Si usas un sistema operativo "UNIX-like", como GNU/Linux o MacOS, ya tienes una _shell_ (terminal) instalada por defecto (y probablemente `git` también). Si usas Windows puedes usar la versión completa de [Cmder](https://cmder.net/) que incluye [Git bash](https://git-scm.com/download/win) y si tienes Windows 10 o superior puedes usar [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10).
3. Una de las integrantes del equipo debe realizar un :fork_and_knife: [fork](https://help.github.com/articles/fork-a-repo/) del repo de tu cohort, tus _coaches_ te compartirán un _link_ a un repo y te darán acceso de lectura en ese repo. La otra integrante del equipo deber hacer un fork **del repositorio de su compañera** y [configurar](https://gist.github.com/BCasal/026e4c7f5c71418485c1) un `remote` hacia el mismo.
4. :arrow_down: [Clona](https://help.github.com/articles/cloning-a-repository/) tu _fork_ a tu computadora (copia local).
5. 📦 Instala las dependencias del proyecto con el comando `npm install`. Esto asume que has instalado [Node.js](https://nodejs.org/) (que incluye [npm](https://docs.npmjs.com/)).
6. Si todo ha ido bien, deberías poder ejecutar las :traffic_light: pruebas unitarias (unit tests) con el comando `npm test`.
7. Para ver la interfaz de tu programa en el navegador, usa el comando `npm start` para arrancar el servidor web y dirígete a `http://localhost:5000` en tu navegador.
8. A codear se ha dicho! :rocket:

### Recursos y temas relacionados

A continuación un video de Michelle que te lleva a través del algoritmo de Luhn y un par de cosas más que debes saber para resolver este proyecto. ¡Escúchala con detenimiento y sigue sus consejos! :)

[![tips credit card](https://img.youtube.com/vi/f0zL6Ot9y_w/0.jpg)](https://www.youtube.com/watch?v=f0zL6Ot9y_w)

[Link](https://www.youtube.com/watch?v=f0zL6Ot9y_w)

Terminal y shell de UNIX:

[![Playlist de Terminal y shell de UNIX](https://img.youtube.com/vi/GB35Eyb-J4c/0.jpg)](https://www.youtube.com/playlist?list=PLiAEe0-R7u8nGH5TEHfSTeDNIvjZFe_Yd)

[Link](https://www.youtube.com/playlist?list=PLiAEe0-R7u8nGH5TEHfSTeDNIvjZFe_Yd)

Control de versiones y trabajo colaborativo con Git y GitHub:

[![Playlist de control de versiones y trabajo colaborativo](https://img.youtube.com/vi/F1EoBbvhaqU/0.jpg)](https://www.youtube.com/playlist?list=PLiAEe0-R7u8k9o3PbT3_QdyoBW_RX8rnV)

[Link](https://www.youtube.com/playlist?list=PLiAEe0-R7u8k9o3PbT3_QdyoBW_RX8rnV)

Diseño de experiencia de usuario (User Experience Design):

* Ideación
* Prototipado (sketching)
* Testeo e Iteración

Desarrollo Front-end:

* Valores
* Tipos
* Variables
* Control de flujo
* Tests unitarios
* [Documentación de NPM](https://docs.npmjs.com/)

Organización del Trabajo:

* [Metodologías Ágiles](https://www.youtube.com/watch?v=v3fLx7VHxGM)
* [Scrum en menos de 2 minutos](https://www.youtube.com/watch?v=TRcReyRYIMg)
* [Scrum en Detalle](https://www.youtube.com/watch?v=nOlwF3HRrAY&t=297s). No esperamos que hagas todo eso desde este proyecto. Iremos profundizando poco a poco a lo largo del -_bootcamp_.
* [Blog: cómo funciona el algoritmo de Luhn](http://www.quobit.mx/asi-funciona-el-algoritmo-de-luhn-para-generar-numeros-de-tarjetas-de-credito.html).
