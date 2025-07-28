# 💰 Sistema Bancário em Python

Este projeto é um **sistema bancário de linha de comando** desenvolvido em Python, com foco na **modularização de funções**, **cadastro de usuários** e **criação de contas correntes**. Ele foi construído como um exercício prático para reforçar conceitos de **funções, listas, dicionários, controle de fluxo e boas práticas em Python**.

---

## 📋 Funcionalidades

* Criar usuários com nome, CPF e endereço completo.
* Criar contas bancárias associadas a um usuário existente.
* Realizar **depósitos** e **saques** com validações.
* Emitir o **extrato bancário** com saldo e histórico de transações.
* Controlar **limite de valor e quantidade de saques** diários.

---

## 🛠 Tecnologias Utilizadas

* **Python 3.x**
* Terminal / Console
* Programação procedural com funções reutilizáveis
* Argumentos `positional-only` e `keyword-only`

---

## ⚙️ Como funciona

### 📁 Estrutura

```python
menu()           # Interface principal do sistema
deposito()       # Função para depósitos (somente argumentos por posição)
saque()          # Função para saques (somente argumentos nomeados)
exibir_extrato() # Função para exibir o extrato da conta
criar_usuario()  # Cadastro de novos clientes (evita CPF duplicado)
criar_conta()    # Criação de contas bancárias vinculadas a usuários
filtrar_usuario()# Função de apoio para buscar CPF na lista de usuários
```

---

## ✅ Regras de Negócio

* Um **CPF não pode ser duplicado**.
* Um **usuário pode ter várias contas**, mas uma **conta só pertence a um usuário**.
* O número da agência é fixo: `0001`.
* O **número da conta é sequencial**, começando em 1.
* Só é possível realizar **três saques por dia**, com limite de R\$500 por saque.
* O extrato exibe todas as movimentações e o saldo atual.

---

## ▶️ Como executar

1. Tenha o Python instalado (`python --version`)
2. Clone o repositório:

   ```bash
   git clone https://github.com/seu-usuario/sistema-bancario-python.git
   cd sistema-bancario-python
   ```
3. Execute o script:

   ```bash
   python sistema_bancario.py
   ```

---

## ✍️ Autor

Desenvolvido por \ Jheyson Silva Siqueira  🧠
Projeto de estudo baseado nos desafios da [DIO - Digital Innovation One](https://www.dio.me)

