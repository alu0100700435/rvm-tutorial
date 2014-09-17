Ruby y Git en Linux 
=========


*Rvm (Ruby Version Manager)* nos permite instalar y gestionar varios intérpretes *ruby* y conjuntos de gemas (gemsets). Por ello en este tutorial vamos a ver como instalarlo en linux, y como instalar las siguientes gemas:

  - *Bundler*
  - *Sinatra*
  - *Twitter*

Y también veremos que es *Git* y como instalarlo.


Instalación RVM
----

La instalación se llevará a cabo como un usuarios estándar, y para instarla debemos escribir en la linea de comandos de la terminal, lo siguiente:

```sh
$ \curl -#L https://get.rvm.io | bash -s stable --autolibs=3 --ruby
```
Como se puede ver en el siguiente ejemplo:

![instalacion de rvm](https://github.com/alu0100700435/rvm-tutorial/blob/gh-pages/img/1.png)

Una vez concluida la instalación, para cerciorarnos de que se ha instalado, hacemos lo siguiente en la linea de comandos:


```sh
rvm -v
```
Esto nos mostrara la version instalada de rvm. 
Para que siempre al iniciar se inicie rmv, escribimos lo siguiente:

```sh
source $HOME/.rvm/scripts/rvm
```
En mi caso en $HOME lo sustituí por */home/user*, y esto modificará el archivo *.profile*.



También podemos saber la versión de ruby instalada y que se esta utilizando de la siguiente manera:

```sh
ruby -v
```
##### Instalación de Gemas

Como ejemplo sólo vamos a instalar tres gemas, pero se puede instalar las que se desee o se necesiten (*[Ruby Gems]*). La manera de instalar una gema es la siguiente:

```sh
gem install [gemaainstalar]
```

Sustituyendo [gemaainstalar] por bundler, twitter o sinatra.


![instalacion de sinatra](https://github.com/alu0100700435/rvm-tutorial/blob/gh-pages/img/2.png)
![instalacion de twitter](https://github.com/alu0100700435/rvm-tutorial/blob/gh-pages/img/3.png)
![instalacion de bundler](https://github.com/alu0100700435/rvm-tutorial/blob/gh-pages/img/4.png)

##### Comprobación del funcionamiento de Bundler

Para poder comprobar el funcionamiento se crea un *Gemfile* en un proyecto, y una vez creado, se hace los siguiente:

```sh
bundle install
```

![funcionamiento bundler](https://github.com/alu0100700435/rvm-tutorial/blob/gh-pages/img/5.png)

*[Más información rvm]* 


Instalación Git
----
Git es una sistema de control de versiones, el cual registra los cambios realizados sobre un archivo o conjunto de archivos a lo largo del tiempo, de modo que puedas recuperar versiones específicas más adelante. Por ello resulta muy útil en la elaboración de proyectos de programación.

Yo ya lo tengo instalado en mi ordenador, pero instarlo es muy fácil, sólo se ha de hacer lo siguiente:

```sh
apt-get install git
```

Una plataforma recomendada para usar este controlador de versiones es *[GitHub]*. Y si quieres aprender más sobre git consulta esta [guía Git].




[Más información rvm]:http://rvm.io/
[Ruby Gems]:https://rubygems.org/
[GitHub]:https://github.com/
[guía git]:http://git-scm.com/book/es/Empezando
