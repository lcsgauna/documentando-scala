# Estrutura de Controle

Estruturas de controle é um conceito importante para qualquer linguagem de programação,
em Scala não é diferente, sua estrutura de controle possui as condicionais básicas encontradas na maioria das linguagens de programação como:

* if  / then / else
* for loops
* try / catch / finally

E também possui estruturas de controle com formato exclusivos como:

* match expressions
* for expressions

## If / Else 

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

Uma estrutura `if/else-if/else` básica em Scala:

````Scala

if(teste1){
    facaX
}else if(teste2){
    facaY()
}else{
    facaZ()
}

````

Uma estrutura If/else quando retorna um resultado:

```Scala
val menorValor = if(a < b)a else b
```
Sobre o exemplo acima, diferentes de outras linguagens, Scala não precisa de um operador ternário ele utiliza a programação orientada a expressões.

Uma estrutura If/else quando não retorna um resultado:

```Scala
if(a == b) facaAlgo()
println("Olá")
```

Quando uma linha de código em Scala não retornar um resultado igual ao exemplo anterior ele é chamado de `side effects`. No exemplo o método `facaAlgo()` é um 
*side effects* quando `a` for igual a `b`, a segunda linha é utilizada como side effects
para escrever um String utilizando o STDOUT.

## For

Um loop em `for` é utilizado quando uma tarefa precisa ser realizada inúmeras vezes
até que sua condicional boleana retorne `false`. Em sua utilização na grande maioria ela é utilizada para iterar elementos dentro de uma `collection`(List,Set,Range,Map, etc).

Estrutura básica de um loop `for` em Scala:

```Scala
for(receptor <- gerador){
    linhas de códigos
}
```

Quando: 

* *receptor*  é a variável que recebe valores enviadas pelo *gerador* a cada iteração

* *gerador* em casos normais são *Range*, *Collection* ou *Map* que enviam novos valores para o *receptor* a cada iteração.

```Scala
val nums = Seq(1,2,3)
for( n <- nums) println(n)
```
No exemplo acima, foi criado uma variável `nums` utilizando a collection `Seq`, no loop `for` a variavel `nums` foi  utilizada como um *gerador* de valores para ser iterado a cada loop na variavel `n` que se torna o *receptor* destes valores. A cada interação é mostrado na tela os valores contidos em `num` até que a condicional retorne `false`, neste caso, até não ter mais valores em `num`.


