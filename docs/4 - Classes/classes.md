# Classes

Com o suporte a orientção à objetos, Scala utiliza o conceito de `class construct`, aonde, seus construtores são inseridos idênticos aos parâmetros de uma função e para diferenciá-los são inseridos `var` ou `val` antes de cada inserção de construtores.

Classe com construtor *read-write*

```Scala
class Pessoa (var nome: String, var sobrenome: String)
```

Classe com construtor *read only*

```Scala
class Pessoa (val nome: String, val sobrenome: String)
```
