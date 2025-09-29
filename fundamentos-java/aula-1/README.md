# JDK e JRE

## JDK Java Development Kit

O JDK é um pacote de software superconjunto do JRE. Ou seja, ele inclui o JRE inteiro e adiciona todas as ferramentas necessárias para desenvolver (compilar, depurar, documentar, empacotar) aplicações Java.

Para quem é?

    Desenvolvedores Java. Se você vai escrever código Java, você precisa do JDK.

O que ele contém? (Tudo que o JRE tem, MAIS...)

    Compilador Java (javac): A ferramenta mais importante. Ele pega o seu código fonte (arquivo .java) e o traduz para bytecode (arquivo .class) que a JVM pode entender.

    Ferramentas de Desenvolvimento:

        java: O carregador de aplicações. É usado para iniciar a JVM e executar a aplicação.

        jar: Utilitário para criar e manipular arquivos JAR (Java ARchive), que são pacotes que contêm todos os arquivos de uma aplicação.

        javadoc: Gera documentação automaticamente a partir dos comentários do código fonte.

        jdb: O depurador (debugger) para encontrar e corrigir erros no código.

        E muitas outras ferramentas para monitoramento e profiling (como jconsole, jstack, jstat).

Resumindo o JDK: É o "pacão" completo. Ele tem todas as ferramentas para criar um programa Java e o ambiente necessário para rodá-lo.

## JRE Java Runtime Environment

O JRE é um pacote de software que fornece as bibliotecas, a Java Virtual Machine (JVM) e outros componentes necessários para executar aplicações escritas em Java.

Para quem é?

    Usuários finais. Se você apenas quer rodar um programa feito em Java (como o Minecraft, por exemplo), você só precisa do JRE instalado na sua máquina.

O que ele contém?

    JVM (Java Virtual Machine): O coração da "escreva uma vez, execute em qualquer lugar" (Write Once, Run Anywhere - WORA). A JVM é responsável por interpretar o bytecode (o código compilado de Java, com extensão .class) e traduzi-lo para instruções que o sistema operacional da sua máquina entenda.

    Bibliotecas de Classes (Class Libraries): Um conjunto vasto de bibliotecas pré-construídas (como java.lang, java.util, java.io, etc.) que fornecem funcionalidades prontas para o programa usar (por exemplo, manipulação de strings, estruturas de dados, acesso a arquivos).

    Outros arquivos de suporte: Como arquivos de propriedades e recursos de interface gráfica.

Resumindo o JRE: Ele não contém ferramentas para desenvolver (como um compilador). Sua única função é rodar aplicações Java.

## Ecossistema OpenJDK e Código Aberto

### Status de Código Aberto


- OpenJDK é a implementação de referência oficial open source do Java

- Licença: GPLv2 + Classpath Exception

- Disponibilidade: Totalmente aberto desde 2007

### Arquitetura de Distribuição

```text
OpenJDK (Código-fonte)
        ↓
[Builds de Early Access]
        ↓
[Release Candidates]
        ↓
Distribuições JDK (Oracle, Eclipse, Amazon, Microsoft, etc.)
```

### Principais Distribuições Baseadas no OpenJDK

| Distribuição | Mantenedor | Características Principais |
|-------------|-------------|-------------|
| Eclipse Temurin | Eclipse Foundation | Build community mais popular|
| Oracle JDK | Oracle | Build comercial com suporte |
| Amazon Correto | AWS | Otimizado para cloud AWS |
| Microsoft JDK | Microsoft | Integração com Azure |
| Azul Zulu | Azul Systems | Foco em performance |



### Notas

- Classes iniciam sempre em letra maiuscula

- Comando para compilar arquivo em java:

```bash

> javac Hello.java

```

- Este comando gera um arquivo compilado .class, agora comando para rodar um programa java:

```bash
> java Hello

Ola mundo! Meu primeiro programa em Java 25!

```