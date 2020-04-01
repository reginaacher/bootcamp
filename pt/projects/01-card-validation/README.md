# Cartão de Crédito Válido

## Índice

* [1. Preâmbulo](#1-preámbulo)
* [2. Resumo do projeto](#2-resumen-del-proyecto)
* [3. Objetivos de aprendizagem](#3-objetivos-de-aprendizaje)
* [4. Considerações gerais](#4-consideraciones-generales)
* [5. Critérios mínimos de aceitação do projeto](#5-criterios-de-aceptación-mínimos-del-proyecto)
* [6. Dicas, conselhos e leituras adicionais](#6-pistas-tips-y-lecturas-complementarias)

***

## 1. Preâmbulo

O [algoritmo de Luhn](https://es.wikipedia.org/wiki/Algoritmo_de_Luhn), também chamado de módulo 10, é um método de soma de verificação, usado para validar números de identificação, como o IMEI de telefones celulares, cartões de crédito etc.

Esse algoritmo é simples. Obtemos o inverso do número a ser verificado (que contém apenas dígitos [0-9]); todos os números que ocupam uma posição par devem ser multiplicados por dois; se esse número for maior ou igual a 10, devemos adicionar os dígitos do resultado; o número a verificar será válido se a soma de seus dígitos finais for um múltiplo de 10.

![gráfico do algoritmo de Luhn](https://www.101computing.net/wp/wp-content/uploads/Luhn-Algorithm.png)

## 2. Resumo do projeto

Neste projeto, você precisará criar um aplicativo da Web que permita ao usuário validar o número de um cartão de crédito.  Além disso, você precisará implementar a funcionalidade para ocultar todos os dígitos de um cartão, exceto os quatro últimos.

O tema é livre. Você deve pensar em quais situações da vida real um cartão de crédito precisaria ser validado e em como deveria ser a experiência do usuário (telas, explicações, mensagens, cores, marca?) etc.

## 3. Objetivos de aprendizagem

Trabalhando em pares, vocês aprenderão a criar um aplicativo Web que irá interagir com x usuárix final através do navegador, usando HTML, CSS e JavaScript como tecnologias.

Simplificando, você aprenderá a:

* Organizar seu tempo e priorizar tarefas em um ambiente de **alta insegurança**.
* Compreender as **necessidades do usuário** e como propor uma solução.
* Compreender a importância do processo de prototipagem durante a criação de um produto digital.
* Conhecer os princípios básicos do design visual.
* Usar tags de HTML semânticas e elementos de formulário.
* Mostrar elementos do formulário na tela usando **HTML** e **CSS**.
* Empregar diversos tipos de seletores em CSS: de elemento, de tipo, de ID.
* Empregar o modelo de caixa CSS (borda, margem, preenchimento).
* Determinar as regras de estilo em CSS.
* Permitir ao usuário que interaja com elementos do DOM e faça com que o aplicativo responda quando ocorrerem esses **eventos do DOM**.
* Manipular _**strings**_ (cadeias de texto).
* Empregar **controle de fluxo** (loops, condicionais, ...).
* Atualizar a tela com os resultados (**manipular o DOM**) mediante **innerHTML** ou **textContent**.
* ** Implementar funções**, dada uma descrição do seu comportamento.
* Verificar se suas funções realizam as tarefas para as quais foram criadas (**testes de unidade (</em>unit tests</1>) com [Jest](https://jestjs.io/es-ES/)**).
* Configurar sua conta git.
* Realizar _fork_ e _clonar_ o repositório do projeto.
* Manter atualizadas as alterações em seu repositório remoto (commit, pull, push).
* Implantar seu projeto nas [Páginas do GitHub](https://pages.github.com).

## 4. Considerações gerais

* A equipe de treinadores fornecerá a você sugestões de tempo e orientações sobre como trabalhar sozinho ou em equipe. Lembre-se que cada pessoa aprende em um ritmo diferente.
* O projeto será entregue carregando seu código no GitHub (commit/push) e a interface será implantada usando as páginas do GitHub. Caso desconheça o GitHub, não se preocupe, pois você vai aprender sobre ele ao longo do projeto.

## 5. Critérios mínimos de aceitação do projeto

Empregue apenas caracteres numéricos (dígitos) no cartão para validar [0-9].

### Definição do produto

No `README.md`, conte-nos como você pensou sobre os usuários e qual foi seu processo para definir o produto final a nível da experiência e da interface.

* Quem são os principais usuários do produto.
* Quais os objetivos destes usuários em relação a seu produto.
* Como você considera que o produto que está criando resolverá os problemas dos usuários.

### Interface do usuário (UI)

A interface deve permitir ao usuário:

* Inserir o número que desejamos validar.
* Constatar se o resultado é válido ou não.
* Ocultar todos os dígitos do número do cartão, excetuando os últimos 4 caracteres.
* Não deve poder inserir um campo vazio.

### UX (Design da experiência do usuário)

Antes de começar a codificar, você deve entender o problema que deseja resolver e como o aplicativo o resolve.

* Trabalhe seu primeiro protótipo com papel e lápis (preto e branco).
* Em seguida, valide esta solução com uma companheira (peça feedback).
* Use o aprendizado no momento de validar seu primeiro protótipo e desenvolva um novo protótipo empregando alguma ferramenta para design de protótipos ([Balsamiq](https://balsamiq.com/), [Figma](https://www.figma.com/), [Apresentações Google](https://www.google.com/intl/es/slides/about/) etc.) Esses pontos serão apresentados no `README.md`.

### Scripts / Arquivos

#### Geral

##### `README.md`

Ele deve conter o seguinte:

* Um título com o nome do seu projeto.
* Um resumo de 1 ou 2 linhas sobre o seu projeto.
* A imagem final do seu projeto.
* Pesquisa UX:
  1. Explicar quem irá usá-lo e os objetivos quanto ao produto.
  2. Explicar como o produto resolve os problemas/necessidades desses usuários.
  3. Em seguida, você colocará a foto do seu primeiro protótipo no papel.
  4. Adicionar um resumo do feedback recebido indicando as melhorias a serem feitas.
  5. Imagem do protótipo final.

#### Visualmente (HTML e CSS)

Você precisará definir exatamente o protótipo final que você criou na ferramenta de design de protótipos que você escolheu usando HTML e CSS. Nesse momento, você escolherá as cores, o tipo de fonte etc. que irá usar.

Abaixo, descrevemos os arquivos que você usará:

##### `src/index.html`

Este arquivo contém o conteúdo que será exibido ao usuário (esqueleto HTML). Você encontrará três marcadores iniciais que, se você quiser, poderá excluir e começar do zero:

* `<header>`: cabeçalho do seu projeto.
* `<main>`: conteúdo principal do seu projeto.
* `<footer>`: rodapé do seu projeto.

##### `src/style.css`

Este arquivo deve conter as regras de estilo. Queremos que você escreva suas próprias regras. Por isso, o uso de estruturas CSS (Bootstrap, materialize etc.) NÃO é permitido.

#### Funcionalmente (JavaScript - testes de unidade)

* A lógica do projeto deve ser totalmente implementada em JavaScript.
* NÃO é permitido usar bibliotecas ou frameworks neste projeto, apenas JavaScript puro, também conhecido como JavaScript Vanilla.
* A _pseudo variável_ `this` não deve ser utilizada.

Você terá 2 arquivos JavaScript que separam responsabilidades, eis o que você fará em cada arquivo:

##### `src/validator.js`

Aqui você escreverá as funções necessárias para que o usuário possa verificar o cartão de crédito e ocultar os dígitos do número do cartão. Esta função deve ser pura e independente do DOM.

Para isso, você deve implementar o **validador `de objeto`**, que já está _exportado_ no _boilerplate_. Este objeto (`validador`) contém dois métodos (`isValid` e `maskify`):

* **`validator.isValid(creditCardNumber)`**: `creditCardNumber` é um `string` com o número do cartão a ser verificado. Esta função deve retornar um `boolean`, dependendo de sua validade, de acordo com o [algoritmo Luhn](https://es.wikipedia.org/wiki/Algoritmo_de_Luhn).

* **`validator.maskify(creditCardNumber)`**: `creditCardNumber` é um `string` com o número do cartão e esta função deve retornar um `string` onde todos, exceto os últimos quatro caracteres, são substituídos por um número (`#`) ou 🐱. Essa função deve sempre manter os quatro últimos caracteres intactos, mesmo quando o `string` for mais curto.

    Exemplo de uso:

    ```js
    maskify('4556364607935616') === '############5616'
    maskify(     '64607935616') ===      '#######5616'
    maskify(               '1') ===                '1'
    maskify(               '')  ===                ''
    ```

##### `src/index.js
`

Aqui, você escreverá todo o código relacionado à interação do DOM (selecionar, atualizar e manipular elementos do DOM e eventos). Ou seja, nesse arquivo, você precisará ativar as funções `isValid` e `maskify` conforme seja necessário para atualizar o resultado na tela (UI).

##### `test/validator.spec.js`

Nesse arquivo, você deverá concluir os testes de unidade das funções `validator.isValid(creditCardNumber)` e `validator.maskify(creditCardNumber)` implementadas em `validator.js` usando [Jest](https://jestjs.io/es-ES/). Seus testes de unidade devem proporcionar 70% em _coverage_ (cobertura), _statements_ (instruções), _functions_ (funções) e _lines_ (linhas); e um mínimo de 50% de _branches_ (ramificações).

***

## 6. Dicas, conselhos e leituras adicionais

### Primeiros passos

1. Antes de tudo, verifique se você possui um :pencil: editor de texto em boa condição, algo como [Atom](https://atom.io/) ou [Code](https://code.visualstudio.com/).
2. Para executar os comandos abaixo, você precisará de um :shell: [Shell UNIX](https://github.com/Laboratoria/bootcamp/tree/master/topics/shell), que é um pequeno programa que interpreta linhas de comando (command-line interpreter), além de ter o [git](https://github.com/Laboratoria/bootcamp/tree/master/topics/scm/01-git) instalado. Se você usa um sistema operacional do tipo UNIX, como GNU/Linux ou MacOS, já possui um _shell_ (terminal) instalado por padrão (e provavelmente `git`) também. Se você usa o Windows, pode utilizar a versão completa do [Cmder](https://cmder.net/) que inclui [Git bash](https://git-scm.com/download/win) e, se tiver o Windows 10 ou superior, pode usar o [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10).
3. Uma das integrantes da equipe deve fazer um :fork_and_knife: [bifurcação](https://help.github.com/articles/fork-a-repo/) do repositório da sua coorte, seus _treinadores_ compartilharão um _link_ com você para um repositório e fornecerão acesso de leitura nesse repositório. A outra integrante da equipe deve fazer uma bifurcação **do repositório da sua companheira** e [configurar](https://gist.github.com/BCasal/026e4c7f5c71418485c1) um `remote` para ele.
4. :arrow_down: [Clone](https://help.github.com/articles/cloning-a-repository/) sua _bifurcação_ no seu computador (cópia local).
5. 📦 Instale as dependências do projeto com o comando `npm install`. Isso pressupõe que você instalou [Node.js](https://nodejs.org/) (que inclui [npm](https://docs.npmjs.com/)).
6. Se tudo correu bem, você poderá executar :traffic_light: testes de unidade (unit tests) com o comando `npm test`.
7. Para visualizar a interface do seu programa no navegador, use o comando `npm start` para iniciar o servidor da web e acesse `http://localhost:5000` no seu navegador.
8. Comece a programar! :rocket:

### Recursos e tópicos relacionados

Aqui está um vídeo de Michelle que mostra o algoritmo de Luhn e mais algumas coisas que você deve saber para realizar este projeto. Ouça com atenção e siga os conselhos dela! :)

[![dicas de cartão de crédito](https://img.youtube.com/vi/f0zL6Ot9y_w/0.jpg)](https://www.youtube.com/watch?v=f0zL6Ot9y_w)

[Link](https://www.youtube.com/watch?v=f0zL6Ot9y_w)

Terminal e shell de UNIX:

[![Lista de reprodução de terminal e shell do UNIX](https://img.youtube.com/vi/GB35Eyb-J4c/0.jpg)](https://www.youtube.com/playlist?list=PLiAEe0-R7u8nGH5TEHfSTeDNIvjZFe_Yd)

[Link](https://www.youtube.com/playlist?list=PLiAEe0-R7u8nGH5TEHfSTeDNIvjZFe_Yd)

Controle de versão e trabalho colaborativo com o Git e o GitHub:

[![Lista de reprodução de controle de versões e trabalho colaborativo ](https://img.youtube.com/vi/F1EoBbvhaqU/0.jpg)](https://www.youtube.com/playlist?list=PLiAEe0-R7u8k9o3PbT3_QdyoBW_RX8rnV)

[Link](https://www.youtube.com/playlist?list=PLiAEe0-R7u8k9o3PbT3_QdyoBW_RX8rnV)

Design da experiência do usuário (User Experience Design):

* Concepção
* Prototipagem (desenho)
* Testes e iteração

Desenvolvimento de front-end:

* Valores
* Tipos
* Variáveis
* Controle de fluxo
* Testes unitários
* [Documentação do NPM](https://docs.npmjs.com/)

Organização do trabalho:

* [Metodologias ágeis](https://www.youtube.com/watch?v=v3fLx7VHxGM)
* [Scrum em menos de 2 minutos](https://www.youtube.com/watch?v=TRcReyRYIMg)
* [Scrum em detalhe](https://www.youtube.com/watch?v=nOlwF3HRrAY&t=297s). Não esperamos que você faça tudo isso neste projeto. Vamos nos aprofundar gradualmente ao longo do -_bootcamp_.
* [Blog: como funciona o algoritmo de Luhn](http://www.quobit.mx/asi-funciona-el-algoritmo-de-luhn-para-generar-numeros-de-tarjetas-de-credito.html).
