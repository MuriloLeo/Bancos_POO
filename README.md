# Bancos - POO

**Sistema Bancário em Python**

Este projeto é um sistema bancário simples desenvolvido em Python, com foco nos princípios de POO (Programação Orientada a Objetos): abstração, herança, encapsulamento e polimorfismo.

**🚀 Objetivo**

*Simular um sistema bancário básico onde:*

- Um banco possui clientes e contas (poupança ou corrente).
- Os clientes podem realizar saques e depósitos.
- O banco é responsável por autenticar transações.

**🧱 Estrutura do Projeto**

*👤 Pessoa*

- Classe base que representa uma pessoa genérica.
- Atributos: nome, idade
- Utiliza encapsulamento com getters.

*👥 Cliente (herda de Pessoa)*

- Representa um cliente do banco.
- Agrega uma ou mais contas (corrente ou poupança).

*💳 Conta (Classe Abstrata)*

- Classe base para diferentes tipos de conta.
- Atributos: agência, número, saldo
- Método abstrato: sacar()
- Método concreto: depositar()

*➕ ContaCorrente (herda de Conta)*

- Possui um limite extra para saque além do saldo.
- Implementa o método sacar().

*💰 ContaPoupanca (herda de Conta)*

- Conta comum de poupança.
- Implementa o método sacar() sem limite extra.

*🏦 Banco*

- Agrega clientes e contas.
- Responsável por autenticar transações:
- Verifica se a agência, conta e cliente pertencem ao banco.
- Só permite saque se a autenticação for bem-sucedida.

*✅ Funcionalidades*

- Cadastro de clientes e contas.
- Depósitos em contas.
- Saques com verificação de saldo e autenticação.
- Suporte a múltiplas contas por cliente.
- Contas Corrente com limite extra de saque.

*🧠 Conceitos Aplicados*

- Abstração: Classe Conta com método abstrato sacar.
- Herança: Cliente herda de Pessoa; ContaCorrente e ContaPoupanca herdam de Conta.
- Encapsulamento: Atributos protegidos com acesso via métodos.
