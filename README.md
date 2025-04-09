# 💰 MGCash - Sistema de Gerenciamento de Pagamentos

Este projeto simula um sistema de folha de pagamento para uma empresa, utilizando **herança** e **polimorfismo** em Java.

---

## 📚 Objetivo

Aplicar os conceitos de programação orientada a objetos com:

- Classes abstratas
- Herança
- Polimorfismo
- Sobrescrita de métodos

---

## 🏗️ Estrutura do Projeto

O sistema é composto pelas seguintes classes:

### 🧱 Classes de Modelo

- **Empregado** (classe abstrata)
  - Atributos: `nome`, `salarioBase`
  - Métodos: `calcularSalario()`, `exibirDetalhes()`

- **EmpregadoHorista**
  - Atributos: `horasTrabalhadas`, `valorHora`
  - Calcula salário com base nas horas trabalhadas

- **EmpregadoComissionado**
  - Atributos: `vendas`, `percentualComissao`
  - Calcula salário com base no salário fixo + comissão

- **EmpregadoAssalariado**
  - Usa apenas o `salarioBase` como salário fixo

---

### 🧪 Classe de Teste

- **PagamentoTeste**
  - Cria 2 objetos de cada tipo de empregado
  - Exibe os detalhes dos funcionários
  - Gera um relatório com:
    - Nome
    - Tipo (Horista, Comissionado ou Assalariado)
    - Salário calculado
    - Total de salários pagos

---

## 💡 Como Executar

1. Compile todos os arquivos `.java`:
   ```bash
   javac *.java
