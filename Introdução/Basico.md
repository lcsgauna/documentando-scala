# Básico

## Olá Mundo

É uma tradição começar programação com um exemplo de **"Olá Mundo"** e para não decepcionar, crie um arquivo `HelloWorld.scala`

```scala
object HelloWorld extends App{
    println("Hello World")
}
```

Após salvar este arquivo, abra o terminal e digite na pasta do aonde está salvo este arquivo e execute com `scala HelloWorld.scala`

## REPL

O Scala REPL("Read-Evaluate-Print Loop") é um interpretador de linha de comando que você utiliza como uma área de "playground" para teste de código Scala

Para iniciar uma sessão REPL, digite `scala` no terminal do seu sistema operacional e você verá algo do assim:

```bash
$scala
Welcome to Scala 2.13.6 (Java HotSpot(TM) 64-Bit Server VM, Java 1.8.0_301).
Type in expressions for evaluation. Or try :help.
```

## Variável

Scala possui dois modos de variáveis:

* `val` é uma variável imutável
* `var` é uma variável mutável e só deve ser usada quando há um motivo específico para usá-la

Exemplos:

```scala
val x = 1 //imutável
var y = 2 //mutável
```

## Tipos de variáveis

Em Scala, você normalmente cria variáveis sem declarar seu tipo, pois, Scala consegue inferir o tipo de dados para você

```scala
val x = 1
val s = "Uma String"
val pokemon = new Pokemon("Gengar")
```

Conseguimos visualizar os tipos de dados inferidos utilizando REPL para isso:

```bash
$scala
Welcome to Scala 2.13.6 (Java HotSpot(TM) 64-Bit Server VM, Java 1.8.0_301).
Type in expressions for evaluation. Or try :help.

scala> val x = 1 
val x : Int = 1
scala> val y = "Uma frase aleatória em Scala para olhar abaixo que o tipo é uma String"
val y : String = Uma frase aleatória em Scala para olhar abaixo que o tipo é uma String

```
