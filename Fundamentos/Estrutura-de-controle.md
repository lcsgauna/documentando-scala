# Estrutura de Controles

Em Scala existe estrutura de controle básicas que você esperaria encontrar em uma linguagem de programação como:

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