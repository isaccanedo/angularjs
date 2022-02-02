# Introdução ao AngularJS

AngularJS é uma estrutura JavaScript. Ele pode ser adicionado a uma página HTML com uma tag <script>.

AngularJS estende atributos HTML com Diretivas e vincula dados a HTML com Expressões.

AngularJS é um framework JavaScript
AngularJS é um framework JavaScript escrito em JavaScript.

O AngularJS é distribuído como um arquivo JavaScript e pode ser adicionado a uma página da Web com uma tag de script:
  
  ```
  <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular.min.js"></script>
  ```
  
### AngularJS estende HTML
  
AngularJS estende HTML com diretivas ng.

A diretiva **ng-app** define um aplicativo AngularJS.

A diretiva **ng-model** vincula o valor dos controles HTML (input, select, textarea) aos dados do aplicativo.

A diretiva **ng-bind** vincula os dados do aplicativo à visualização HTML.
  
### Exemplo AngularJS
  
  ```
  <!DOCTYPE html>
<html>
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular.min.js"></script>
<body>

<div ng-app="">
  <p>Name: <input type="text" ng-model="name"></p>
  <p ng-bind="name"></p>
</div>

</body>
</html>
  ```
  
### Exemplo explicado:

O AngularJS é iniciado automaticamente quando a página da Web é carregada.

A diretiva **ng-app** diz ao AngularJS que o elemento <div> é o "proprietário" de um aplicativo AngularJS.

A diretiva **ng-model** vincula o valor do campo de entrada ao nome da variável do aplicativo.

A diretiva **ng-bind** vincula o conteúdo do elemento <p> ao nome da variável do aplicativo.
  
### Diretivas AngularJS
  
Como você já viu, as diretivas AngularJS são atributos HTML com um prefixo ng.

A diretiva ng-init inicializa as variáveis do aplicativo AngularJS.
  
```
<div ng-app="" ng-init="firstName='John'">

<p>The name is <span ng-bind="firstName"></span></p>

</div>
```

Alternativamente com HTML válido:
  
```
<div data-ng-app="" data-ng-init="firstName='John'">

<p>The name is <span data-ng-bind="firstName"></span></p>

</div>
```
  
Você pode usar data-ng-, em vez de ng-, se quiser tornar sua página HTML válida.

Você aprenderá muito mais sobre diretivas posteriormente neste tutorial.

### Expressões AngularJS
  
As expressões AngularJS são escritas entre chaves duplas: ```{{ expressão }}```.

O AngularJS "exibirá" os dados exatamente onde a expressão está escrita:
  
  ```
  <!DOCTYPE html>
<html>
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.6.9/angular.min.js"></script>
<body>

<div ng-app="">
  <p>My first expression: {{ 5 + 5 }}</p>
</div>

</body>
</html>
  ```
