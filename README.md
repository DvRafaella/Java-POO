
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

### Exemplo completo

Você escreve:

```java
System.out.println("Olá!");
```

Depois acontece:

1. Você salva em um arquivo **`.java`**.
2. O compilador (`javac`) transforma o código em **bytecode** (`.class`).
3. A **JVM** lê esse bytecode.
4. A JVM converte as instruções para o código de máquina do seu computador e o programa é executado.




