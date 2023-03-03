# Programação Orientada a Objetos

## motivação

```java
// alunos
String[] nome = new String[1000];
String[] CPF = new String[1000];
int[] idade = new int[1000];
double[] nota = new double[1000];
```

```java
int a = 2, b = 3;
int temp = a;
a = b;
b = temp;
```

problemas tentando trocar dois alunos:

- inconsistência do tipo aluno
- dificuldade de trocar alunos (falta de abstração)
- relacionamento incorreto dos dados (maior entre dados semelhantes do que entre dados de uma mesma entidade)

## Classe e Objeto

Classe é o molde.

Objeto é o fruto desse molde.

**Conteúdo de uma classe:**

- tem : **atributos**
- faz: **método**

```java

// modelagem de um aluno
class Aluno {
  String nome;
  String CPF;
  int idade;
  double nota;

  void fazerAniversario() {
    idade++;
  }

  double somar(double a, double b) {
    return a + b;
  }
}

public class Program {

  public static void main(String[] args){

    // instancia de um Aluno
    Aluno joao = new Aluno();
    Aluno[] turna = new Aluno[1000];

    // resolvendo problema motivador
    Aluno temp = turma[5];
    turma[5] = turma[0];
    turma[0] = temp;

    // atribuindo valor aos atributos
    joao.nome = "Joao Pedro da Silva";
    joao.CPF = "111.222.333-99";
    joao.idade = 20;
    joao.nota = 8.5;

    // acessando o valor dos atributos
    System.out.println("Nome: " + joao.nome);
  }

}
```
