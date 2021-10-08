# Instalação

### **Importante**: Antes de instalar `Scala`, é necessário ter instalado `Java JDK 8` ou `Java JDK 11` na máquina

## 1. Verificar JDK na máquina

Para verficar, abra o terminal e digite:
`java -version`, deve ser mostrado a versão do Java informado(1.8 ou 11), caso não apareça ou tenha uma versão diferente recomendo que baixe uma destas duas versões:

* [Oracle JDK 8](https://www.oracle.com/java/technologies/javase-jdk8-downloads.html)

* [Oracle JDK 11](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html)

## 2. Maneiras de instalar Scala

* Instalando o plugin no IntelliJ

    Na aba plugin busque por `Scala` no marketplace e clique em instalar, caso não saiba [como baixar plugin IntelliJ](https://www.jetbrains.com/help/idea/managing-plugins.html)

* Instalando via SBT

    O sbt é o build tool do Scala (não tem nada a ver com Silvio Santos), recomendo que instale este build tool mesmo não sendo sua escolha de instalação do Scala,pois, muitos frameworks Scala o utilizam para instalar suas dependencias.

    [Windows](https://www.scala-sbt.org/1.x/docs/Installing-sbt-on-Windows.html),
    [Linux](https://www.scala-sbt.org/1.x/docs/Installing-sbt-on-Linux.html),
    [Mac](https://www.scala-sbt.org/1.x/docs/Installing-sbt-on-Mac.html)

    Após a instalação crie um projeto e adicione o arquivo `build.sbt`, este arquivo será o local aonde as bibliotecas e funcionalidades adicionadas no projeto serão reconhecidas pelo sbt e assim instaladas. Como estamos instalando Scala, iremos abrir este arquivo e adicionar:

    ````sbt
    libraryDependencies += "org.scala-lang.modules" %% "scala-parser-combinators" % "1.1.2"
    ````

* **Microsoft**: Instalador Scala

    [Instalador Scala 2.13](https://downloads.lightbend.com/scala/2.13.6/scala-2.13.6.msi)

* Utilizando SDKMAN!

    O SDKMAN! é um kit de gerenciamento de software que pode ser instalado no Linux, Mac e Windows, para instalar em sua máquina o SDKMAN!, [veja este passo a passo](https://sdkman.io/install).

    Após a instalação do gerenciador, utilize o comando `sdk install scala` ou caso preferir uma versão especifica `sdk install scala 2.13.6` para instalar Scala via sdkman.

* Utilizando Scala Online

    Utilizando o [Scatie](https://scastie.scala-lang.org/), você tem a possibilidade de executar arquivos diretamente e com a possibilidade de configurar as principais bibliotecas do Scala pelo Browser.
