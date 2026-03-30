[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/byyi1sDv)
# Recuperacao-banco de dados
**Tarefa de Recuperação: Gerenciamento de Inventário com SQLite3

Nesta atividade, você vai reforçar seus conhecimentos em SQL criando um banco de dados para gerenciar um pequeno estoque de produtos, garantindo a persistência dos dados no seu repositório GitHub.

Objetivo

Criar um banco de dados relacional com uma tabela de  **produtos**, inserir itens e realizar o envio (push) do arquivo final para o seu repositório.

🛠️ Passo a Passo

1. Criar o Banco de Dados

No terminal do seu Codespace, crie o arquivo do banco de dados de inventário utilizando seu nome para identificação:

Terminal

```
sqlite3 inventario_seu_nome.db
```

2. Criar a Tabela

Dentro do prompt do SQLite (`sqlite>`), crie a tabela  `produtos`  com a seguinte estrutura:

-   **id**: Inteiro, Chave Primária e Auto Incremento.
-   **nome**: Texto (obrigatório).
-   **quantidade**: Inteiro (não pode ser nulo).
-   **preco**: Real (valor decimal).

**Comando:**

sql

```
CREATE TABLE produtos (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    nome TEXT NOT NULL,
    quantidade INTEGER NOT NULL,
    preco REAL
);
```

3. Inserir Registros

Insira  **pelo menos 5 produtos**  diferentes. Exemplo de comando:

Terminal

```
INSERT INTO produtos (nome, quantidade, preco) VALUES ('Teclado Mecânico', 10, 250.50);
```

Use o código com cuidado.

4. Validar e Sair

Verifique se os dados foram salvos corretamente:

-   Digite  `SELECT * FROM produtos;`  e veja se a lista aparece.
-   Saia do SQLite digitando  `.exit`.

----------

Entrega (Git)

Envie o novo arquivo  `.db`  para o seu repositório com os comandos:

Terminal

```
git add inventario_seu_nome.db
git commit -m "Recuperação SQLite: Criado inventário de produtos"
git push
```

Use o código com cuidado.

----------

Dicas para os alunos:

-   **Errou o comando?**  Se o terminal mostrar  `...>` , é porque você esqueceu o ponto e vírgula (`;`). Digite  `;`  e dê Enter.
-   **Cuidado com o Nome:**  Certifique-se de substituir  `seu_nome`  pelo seu nome real no arquivo  `.db`.**
