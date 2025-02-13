# 🚀 Desafio - Conta Banco

## 📌 Descrição
Este projeto faz parte do **Bootcamp Java Cloud Native** e tem como objetivo fixar conceitos fundamentais da **sintaxe Java**, incluindo:
- Declaração de **classes e métodos**
- Uso de **variáveis e tipos primitivos**
- Entrada de dados via **`Scanner`**
- Uso de **concatenação de Strings**

O programa simula a criação de uma **conta bancária** a partir dos dados fornecidos pelo usuário no terminal.

---

## 📂 Estrutura do Projeto
```
📦 ContaBanco
 ┣ 📂 src/main/java/com/seuprojeto/contabanco
 ┃ ┣ 📜 ContaTerminal.java
 ┣ 📜 README.md
 ┣ 📜 .gitignore
 ┗ 📜 pom.xml
```

---

## 📜 Implementação

### **1️⃣ Classe `ContaTerminal.java`**
```java
package com.seuprojeto.contabanco;

import java.util.Scanner;

public class ContaTerminal {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Solicitação de dados ao usuário
        System.out.println("Por favor, digite o número da Agência: ");
        String agencia = scanner.nextLine();
        
        System.out.println("Digite o número da conta: ");
        int numero = scanner.nextInt();
        scanner.nextLine(); // Consumir a quebra de linha
        
        System.out.println("Digite o nome do Cliente: ");
        String nomeCliente = scanner.nextLine();
        
        System.out.println("Digite o saldo inicial: ");
        double saldo = scanner.nextDouble();

        // Exibição da mensagem formatada
        System.out.println("Olá " + nomeCliente + ", obrigado por criar uma conta em nosso banco, " +
                "sua agência é " + agencia + ", conta " + numero + " e seu saldo " + saldo + " já está disponível para saque.");
        
        scanner.close();
    }
}
```

---

## 🎯 O que foi aplicado?
✔ **Uso do `Scanner`** para entrada de dados do usuário via terminal.
✔ **Tipos de variáveis**: `String`, `int`, `double`.
✔ **Concatenação de Strings** para exibir a mensagem formatada.
✔ **Estrutura de um programa Java** (`main`, `System.out.println()`, `scanner.nextLine()`, etc.).

---

## 🔥 Como Executar o Programa
1. **Clone o repositório:**
   ```bash
   git clone https://github.com/seuusuario/ContaBanco.git
   ```
2. **Acesse o diretório do projeto:**
   ```bash
   cd ContaBanco
   ```
3. **Compile e execute o programa:**
   ```bash
   javac src/main/java/com/seuprojeto/contabanco/ContaTerminal.java
   java -cp src/main/java com.seuprojeto.contabanco.ContaTerminal
   ```

---

## 📌 Exemplo de Entrada e Saída
**Entrada do Usuário:**
```
Por favor, digite o número da Agência:
067-8
Digite o número da conta:
1021
Digite o nome do Cliente:
MARIO ANDRADE
Digite o saldo inicial:
237.48
```

**Saída no Terminal:**
```
Olá MARIO ANDRADE, obrigado por criar uma conta em nosso banco, sua agência é 067-8, conta 1021 e seu saldo 237.48 já está disponível para saque.
```

---

## 🏆 Conclusão
Este desafio ajudou a fixar os conceitos básicos da **sintaxe Java**, **entrada de dados**, **tipos de variáveis** e **concatenação de Strings**.

🚀 **Agora é só testar, melhorar e adaptar para novos desafios!**

