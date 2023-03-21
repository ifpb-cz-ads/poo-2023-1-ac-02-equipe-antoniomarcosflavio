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

#### 5. Mude o nome do método “main” para “start”, compile e execute. O que aconteceu?

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

#### 8. Experimente salvar o arquivo com um nome diferente do nome da classe, compile e execute. O que aconteceu?
