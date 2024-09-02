# Esse eu já li!

**"Esse eu já li!"** é um sistema simples de gamificação para leitores. Nele, os usuários podem marcar os livros que já leram, acumular pontos com base no número de páginas lidas, e conquistar troféus ao completar um certo número de livros de um mesmo estilo. O sistema também possui um ranking que exibe os 10 usuários com maior pontuação.

## Funcionalidades

- **Login de Usuário**: Usuários podem fazer login com email e senha.
- **Marcação de Livros Lidos**: Usuários podem selecionar e marcar livros que já leram, acumulando pontos.
- **Pontuação**: Pontos são atribuídos a cada livro lido, com pontos extras para livros mais longos.
- **Troféus**: Usuários ganham troféus ao lerem 5 livros do mesmo estilo.
- **Ranking**: Ranking dos 10 usuários com maior pontuação.

## Estrutura do Código

### Classes Principais

- **`Usuario`**: Gerencia as informações do usuário, livros lidos, pontuação, e troféus conquistados.
- **`Livro`**: Representa um livro com título, autor, número de páginas e estilo.
- **`Trofeu`**: Representa um troféu que pode ser concedido a um usuário ao ler um certo número de livros de um mesmo estilo.
- **`Ranking`**: Gera e exibe o ranking dos 10 usuários com maior pontuação.
- **`Program`**: Classe principal que gerencia a execução do sistema, incluindo login, marcação de livros como lidos e exibição de informações e ranking.

## Como Executar

### Pré-requisitos

- **Java Development Kit (JDK)**: Certifique-se de que o JDK está instalado no seu sistema. Você pode baixar a última versão [aqui](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html).

### Passos para Compilar e Executar

1. **Clone ou Baixe o Repositório**:
    ```bash
    git clone https://github.com/seu-usuario/seu-repositorio.git
    ```
    Ou faça o download como ZIP e extraia os arquivos.

2. **Compile o Código**:
    Navegue até o diretório do projeto e compile os arquivos `.java`:
    ```bash
    javac -d bin src/entities/*.java src/Program.java
    ```

3. **Execute o Programa**:
    Após a compilação, execute o programa a partir da pasta `bin`:
    ```bash
    java -cp bin Program
    ```

4. **Interaja com o Sistema**:
    - Insira seu email e senha para fazer login.
    - Selecione um livro da lista para marcar como lido.
    - Veja seus pontos e troféus acumulados.
    - Veja o ranking dos 10 melhores leitores.

## Estrutura de Diretórios

```plaintext
├── src
│   ├── entities
│   │   ├── Usuario.java
│   │   ├── Livro.java
│   │   ├── Trofeu.java
│   │   └── Ranking.java
│   └── Program.java
├── bin
│   └── (arquivos .class compilados)
└── README.md
