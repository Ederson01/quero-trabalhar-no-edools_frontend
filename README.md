AngularJS Exam
==============

# Ederson - AngularJS Exam Edools
## Objetivo da applica��o
A aplica��o se conecta com uma api do git hub e faz uma busca de todos os repositorios pelo nome e retorna em uma lista contendo informa��es sobre o repositorio.
� preciso digitar pelo menos 5 letrar para o sistema iniciar a busca.
Se o usuario clicar na linha daquele repositorio o sistema abrir� uma nova aba diretamente naquele repositorio do github
**a aplica��o est� disponivel [edersonangular.azurewebsites.net](http://edersonangular.azurewebsites.net/)**
## Arquitetura
A aplica��o web foi desenvolvida com angularJS, com o bower como gestor de dependencia e o gulp para automatizar as tarefas. O gulp tamb�m realiza alguns testes para ver se tem arquivos faltantes.
## Estrutura de diretorios
O sistema est� dividido nos seguintes diret�rios:
- app
  * css
  * js
  * views
- master
  * js
    * components
      * search
  * less
- vendor
### app
A pasta app contem os arquivos de distribui��o css, js (compactados e uglifyed) e views (html)
### master
A pasta master contem os arquivos "fontes" js e less.
Na pasta js tem os arquivos de inicializa��o e de roteamento e a aplica��o foi modularizada na pasta components e depois na pasta search que contem o controller e o services em angularjs.
### vendor
A pasta vendor contem arquivos externos como fontes awesome entre outros.

### Instala��o
Voc� precisa ter o NodeJs e NPM instalados

Voc� precisa instalar o gulp
```sh
$ npm install -g gulp
```
### Debug e Edi��o
Voc� precisa rodar o gulp
```sh
$ gulp
```
Com isso voc� pode editar os arquivos less e js que o gulp vai atualizar os arquivos js e css automaticamente na pasta app, onde o index.html est� apontando.

### Distribui��o
Voc� precisa rodar o gulp build para compactar e huglify os arquivos
```sh
$ gulp build
```
Para distribuir vc deve copiar somente a pasta app e o index.
