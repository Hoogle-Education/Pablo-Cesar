# Revisão Java - Imperativa

## Saídas

```java
// sout // sysout
System.out.println("Hello World");
System.out.print("Hello World\n");
```

1. `%f` : float ou double
2. `%d` : int, short, ...
3. `%c` : caracteres
4. `%s` : strings

```java
double valor = 34.50; // float x 2

System.out.printf("O valor do produto é %.2f", valor);
```

```java
int a = 2;
int b = 3;
int soma = a + b;

System.out.printf("A soma de %d e %d é igual a %d", a, b, soma);
```

## Seleção (`if-else`)

### SE (`if`)

sintaxe:

```java
double a = 5.5;
double b = 3.4;
char operacao = '+';

// true(diferente de 0) ou false(0)
// boolean ehPraSomar = (operacao == '+')

if(operacao == '+') {
  double soma = a + b;
  System.out.pritln("A soma é" + soma );
}
```

### SE...SENÃO (`if...else`)

```java
if (/*condição*/) {
  /*executa se for true*/
} else {
  /*executa se for false*/
}
```

```java
if(operacao == '+') {
  double soma = a + b;
  System.out.pritln("A soma é" + soma );
} else {
  double produto = a + b;
  System.out.pritln("A produto é" + produto );
}
```

### SE...SENÃO SE...

```java
if(nota >= 7.0) {
  System.out.pritln("Aprovado");
} else if (nota >= 4.0) {
  System.out.pritln("Recuperação");
} else {
  System.out.pritln("Reprovado");
}
```

calculadora:

```java
if(op == '+') {
  //...
} else if (op == '-') {
  // ...
} else if (op == '*') {
  // ...
} else if (op == '/') {
  // ...
} else {
  System.out.pritln("Operação inválida");
}
```

### especiais de seleção

**if-braceless:**

Se tivermos apenas um comando dentro do `if`, não é necessário indicarmos seu escopo por chaves.

```java
double resultado;


if(op == '+') resultado = a + b;
else if (op == '-') resultado = a - b;
else if (op == '*') resultado = a * b;
else if (op == '/') resultado = a / b;
else
  System.out.pritln("Operação inválida");

```

**operador ternário**

sintaxe:

```java
resultado = (/*condição*/) ? (/*se for true*/) : (/*se for false*/);

resultado = (/*condição*/) ?
  (/*se for true*/) : (/*se for false*/);
```

## Operadores Aritméticos

1. `%`: módulo, calcula o resto entre dois números.

ex: 10 % 3 , resp = 1

2. `&&`: "e", permite que a gente verifique se ambas as condições são atendidas.

|    a    |    b    | `and` | result  |
| :-----: | :-----: | :---: | :-----: |
| `true`  | `true`  |   =   | `true`  |
| `true`  | `false` |   =   | `false` |
| `false` | `true`  |   =   | `false` |
| `false` | `false` |   =   | `false` |

3. `||`: "ou", permite que a gente verifique se ambas as condições são atendidas.

|    a    |    b    | `or` | result  |
| :-----: | :-----: | :--: | :-----: |
| `true`  | `true`  |  =   | `true`  |
| `true`  | `false` |  =   | `true`  |
| `false` | `true`  |  =   | `true`  |
| `false` | `false` |  =   | `false` |

4. `!`: "não", nega a expressão ou símbolo que está sendo avaliado.

## Entradas

```java
public class Program {
  public static void main(String[] args) {

    Scanner keyboard = new Scanner(System.in);

  }
}
```
