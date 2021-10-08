# Instalação

## 1. Verificar JDK na máquina

Antes de instalar o `Scala` é necessário ter instalado `Java JDK 8` ou `Java JDK 11` instalado na máquina

Para verficar, abra o terminal e digite:
`java -version`, deve ser mostrado a versão do Java informado(1.8 ou 11), caso não apareça ou tenha uma versão diferente recomendo que baixe uma destas duas versões:

* [Oracle JDK 8](https://www.oracle.com/java/technologies/javase-jdk8-downloads.html)

* [Oracle JDK 11](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html)

## 2. Modos de instalar Scala

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
