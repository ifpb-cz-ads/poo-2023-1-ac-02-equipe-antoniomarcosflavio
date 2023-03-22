#### 1. Explique qual a função da Máquina Virtual Java (JVM)
A JVM permite que o código Java seja executado em diferentes plataformas, independentemente do sistema operacional. A principal função da JVM é interpretar o código compilado em bytecode Java e executá-lo em tempo de execução.

#### 2. Qual a diferença entre JRE e JDK?
O JRE trata-se de uma sigla para Java Runtime Environment que, como o proprio nome sugere, é o “Ambiente de execução Java” e contém tudo aquilo que um usuário comum precisa para executar uma aplicação Java, provendo uma JVM e alguns pacotes básicos do Java.  
Já o JDK é o Java Development Kit, composto pelo JRE e um conjunto de ferramentas úteis ao desenvolvedor Java, tais como o compilador, interpretador, debugador, dentre outras.

#### 3. Crie um programa Java que imprima o seguinte texto “Terminei a primeira aula com um programa Java!”
```java
public class Main {
        public static void main(String[] args) {
            System.out.println("Terminei a primeira aula com um programa Java!");
        }
   }
```

#### 4. Compile o programa desenvolvido no exercício anterior. A seguir apague o arquivo .class gerado e tente executar o programa. O que aconteceu?
Ao tentar executar o programa sem o arquivo .class, ocorre um erro em que a classe não foi encontrada.  
A saída no terminal foi a seguinte:
```zsh
❯ java Main
Erro: Não foi possível localizar nem carregar a classe principal Main
Causada por: java.lang.ClassNotFoundException: Main
```
No entanto, ao se chamar o comando java passando o arquivo .java como argumento, mesmo sem compilar o programa e gerar o arquivo .class, o programa executa normalmente, sem gerar o arquivo bytecode.  
A exemplo no terminal foi o seguinte:
```zsh
❯ java Main.java
Terminei a primeira aula com um programa Java!
```
#### 5. Mude o nome do método “main” para “start”, compile e execute. O que aconteceu?
O programa foi compilado com sucesso, no entanto, ocorreu um erro na execução do programa porque o método main não foi encontrado na classe.

#### 6. Crie um programa Java para imprimir duas linhas de texto usando duas linhas de código “System.out”, onde aparecerá o seu nome na primeira linha e na segunda linha aparecerá o time para o qual você torce.
```java
public class ImprimeNomeETime {
    public static void main(String[] args) {
        String nome = "Antonio Marcos";
        String time = "Fluminense";
        System.out.println(nome);
        System.out.println(time);
    }
}
```

#### 7. Experimente escrever todo o programa anterior em maiúsculo, compile e execute. O que aconteceu?
Houve erro de sintáxe no compilador Java, porque ele não foi capaz de reconhecer os nomes das classes e métodos.

#### 8. Experimente salvar o arquivo com um nome diferente do nome da classe, compile e execute. O que aconteceu?
O código não chegou a ser compilado, uma vez que a classe é renomeada para Time, o compilador informa que ela deve ser declarada num arquivo de mesmo nome, no caso em tela, o arquivo teria de ser renomeado para o mesmo nome da classe: Time.java.  
A saída no terminal foi a seguinte:
```zsh
❯ javac ImprimeNomeETime.java
ImprimeNomeETime.java:1: error: class Time is public, should be declared in a file named Time.java
public class Time {
       ^
1 error
```
