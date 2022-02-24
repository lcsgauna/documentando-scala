# If / Else

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

Sobre o exemplo acima, diferente de outras linguagens, Scala não precisa de um operador ternário ele utiliza a programação orientada a expressões.

Uma estrutura If/else quando não retorna um resultado:

```Scala
if(a == b) facaAlgo()
println("Olá")
```

Quando uma linha de código em Scala não retornar um resultado igual ao exemplo anterior ele é chamado de `side effects`. No exemplo o método `facaAlgo()` é um *side effects* quando `a` for igual a `b`, a segunda linha é utilizada como side effects para escrever um String utilizando o STDOUT.
