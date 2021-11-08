# Estrutura de Controle
Estruturas de controle é uma parte importante de qualquer linguagem de programação,
em Scala não é diferente, em sua estrutura de controle possui o básico que você espera encontrar em uma linguagem de programação como:

* if  / then / else
* for loops
* try / catch / finally

E também possui estruturas de controle com formato exclusivos como:

* match expressions
* for expressions

## if / else 

Uma estrutura de `if` básica em Scala:

````Scala

if (a == b) facaAlgo()

ou 

if(a==b){
    facaAlgo()
}

````

Uma estrutura `if/else` básica em Scala:

````Scala

if(a==b){
    facaAlgo()
}else{
    facaOutraCoisa()
}

````

Uma estrutura `if\else-if\else` básica em Scala:

````Scala

if(teste1){
    facaX
}else if(teste2){
    facaY()
}else{
    facaZ()
}

````

If/else quando retorna um resultado

```Scala
val menorValor = if(a < b)a else b
```
Sobre o exemplo acima, diferentes de outras linguagens, Scala não precisa de um operador ternário ele utiliza a programação orientada a expressões.


If/else quando não retorna um resultado

```Scala
if(a == b) facaAlgo()
println("Olá")
```

Quando uma linha de código em Scala não retorna um resultado igual ao exemplo anterior ele é chamado de `side effects`. No exemplo o método `facaAlgo()` é um 
side effects quando `a` for igual a `b`, a segunda linha é utilizada como side effects
para escrever um String utilizando o STDOUT.


## For

Um loop em `for` é utilizado quando uma tarefa precisa ser realizada repetidas vezes
até que sua condicional boleana retorne `false`

Sintaxe básica de um loop `for` em Scala:

```Scala
for(receptor <- gerador){
    linhas de códigos
}
```

Quando: 
. *receptor*  é a variável que recebe valores enviadas pelo *gerador* a cada iteração
. *gerador* em casos normais são *Range*, *Collection* ou *Map* que enviam novos valores para o *receptor* a cada iteração.



