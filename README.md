
**1. Código-fonte (.java) → 2. Bytecode (.class) → 3. JVM (Java Virtual Machine)**

Etapas

### 1. Código-fonte (arquivo `.java`)

É o código que o programador escreve usando a linguagem Java.

Exemplo:

```java
public class OlaMundo {
    public static void main(String[] args) {
        System.out.println("Olá, mundo!");
    }
}
```

Esse arquivo é salvo com a extensão **`.java`**.

---

### 2. Bytecode (arquivo `.class`)

O código-fonte não é executado diretamente pelo computador.

Primeiro, ele é **compilado** pelo compilador Java (`javac`), que transforma o arquivo `.java` em um arquivo `.class`, contendo **bytecode**.

Exemplo:

```bash
javac OlaMundo.java
```

Resultado:

```
OlaMundo.class
```

O **bytecode** é um código intermediário. Ele não depende do sistema operacional, por isso pode ser executado em diferentes plataformas.

---

### 3. JVM (Java Virtual Machine)

A **JVM** é a Máquina Virtual Java.

Ela é responsável por:

* Ler o bytecode (`.class`);
* Interpretar ou compilar esse bytecode para código de máquina;
* Executar o programa no computador.

Para executar o programa:

```bash
java OlaMundo
```

A JVM carrega o arquivo `.class` e executa suas instruções.

---

## Resumo da ordem

```
Programador
      │
      ▼
Código-fonte (.java)
      │
      │ javac (compilador)
      ▼
Bytecode (.class)
      │
      │ JVM
      ▼
Código de máquina
      │
      ▼
Programa executando
```



JDK (Java Development Kit)

O JDK é o kit de desenvolvimento Java.

Ele é usado por quem programa em Java.

O que ele contém?
✅ Compilador (javac)
✅ JRE
✅ Ferramentas de desenvolvimento (como javadoc, jar, jdb, entre outras)

Sua principal função é criar, compilar e executar programas Java.


JRE (Java Runtime Environment)

O JRE é o ambiente de execução Java.

Ele serve para executar programas Java, mas não permite compilá-los.

O que ele contém?
✅ JVM
✅ Bibliotecas necessárias para rodar programas Java

Se você só quer abrir um programa Java, o JRE é suficiente.




