# For

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
for(n <- nums) println(n)
```

No exemplo acima, foi criado uma variável `nums` utilizando a collection `Seq`, no loop `for` a variavel `nums` foi  utilizada como um *gerador* de valores para ser iterado a cada loop na variavel `n` que se torna o *receptor* destes valores. A cada interação é mostrado na tela os valores contidos em `num` até que a condicional retorne `false`, neste caso, até não ter mais valores em `num`.

## Foreach

## For Comprehensions

Além da utilização `for` comum em muitas linguagens, Scala também oferece uma versão mais simples de expressar uma sequência utilizando `for`.

Estrutura básica de `for comprehensions`:

```Scala
for (enumerador) yield resultado
```

Aonde:

* *enumerador* : É uma lista de enumeradores separados por ponto e vírgula. Ele é o gerador que pode introduzir novas variáveis ou um filtro.

* *yield* : Declaração para colher o resultado do enumerador em uma variavel, no caso da estrutura acima, na variavel resultado.

* *resultado* : Retorno do que é gerado dentro do enumerador.

```Scala
case class Usuario(nome:String, idade: Int)

val baseUsuario = List(
    Usuario("Ana", 28),
    Usuario("Laura",38),
    Usuario("Antonio", 3),
    Usuario("Alice", 1)
)

val buscarVinteTantosAnos = for( usuarios <- baseUsuario if usuario.idade >= 20 && usuario.idade < 30) yield usuario.nome

buscarVinteTantosAnos.foreach(println) // Ana
```

No exemplo acima, foi criado uma variável chamada `baseUsuario` que contém uma `List` alimentando uma case class `Usuario` com informações do tipo `String` e `Int`.
