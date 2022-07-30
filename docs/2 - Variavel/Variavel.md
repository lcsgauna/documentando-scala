# Variável

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

Tipos de dados e seus valores possíveis :

| Tipos de Dados | Valores |
:----------|:---------|
| Boolean | `True` ou `False`|
| Byte |  Números inteiros de `-128` a `127` de `8 bits`   |
| Short | Números inteiros de `32.768` a `32.767` de `16 bits` |
| Int | Números inteiros de `-2.147.483.648` a `2.147.483.647` de `32 bits` |
| Long |Números inteiros de `-9223372036854775808` to `9223372036854775807` de `64 bits`|
| Float | Números flutuantes de `1.40129846432481707e-45` a `3.40282346638528860e + 38` de `32 bits`|
| Double | Números flutuantes de `4.94065645841246544e-324d` a `1.79769313486231570e + 308` de `64 bits`|
| Char | Caractere `Unicode` de `0` a `65.535` de `16 bits`|
| String | Cadeia de caracteres|

Scala também conta com mais dois tipos de dados para números o `BigInt` e `BigDecimal` e ambos oferecem suporte aos operadores para usar com tipos numéricos.
