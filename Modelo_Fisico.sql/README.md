# Modelo Fisico

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-Expert-orange?style=for-the-badge) ![Status](https://img.shields.io/badge/Status-Finalizado-success?style=for-the-badge)

> **"Integração total entre passageiros, frotas e pagamentos digitais."**

## 📋 Sobre o Projeto
Este repositório contém a implementação física (SQL) de um banco de dados relacional para cidades inteligentes. O sistema gerencia desde a **bilhetagem eletrônica** até o **monitoramento de frotas** e **aluguel de veículos leves**.

## 🗄️ Estrutura do Banco de Dados

O schema foi projetado para garantir a integridade e escalabilidade dos dados.

| Tabela | Função Principal | Destaque Técnico |
| :--- | :--- | :--- |
| **👤 Usuario** | Cadastro central de passageiros. | `Unique Email` |
| **💳 Recarga** | Histórico financeiro de créditos. | `Check (valor > 0)` |
| **🚌 Veiculos** | Gestão da frota (Ônibus, VLT, Bikes). | `Controle de Manutenção (1-5)` |
| **📍 Rota & Parada** | Logística de trajetos e distâncias. | `Cálculo de Distância (KM)` |
| **⏱️ Faz_Trajeto** | Monitoramento de horários. | `Tabela Associativa` |

---

## 🛠️ Regras de Negócio Implementadas (SQL)

O código SQL inclui restrições robustas para validar os dados diretamente no banco:
*   ✅ **Validação Financeira:** Não é permitido recargas com valor negativo ou zero.
*   ✅ **Qualidade da Frota:** O grau de manutenção dos veículos é restrito a uma escala de 1 a 5.
*   ✅ **Integridade Referencial:** Uso rigoroso de `Foreign Keys` conectando pagamentos, bilhetes e usuários.

## 🚀 Como Executar

1.  Certifique-se de ter o **PostgreSQL** instalado.
2.  Clone este repositório.
3.  Execute o script principal:
    ```sql
    -- O arquivo cria as tabelas e popula com dados de teste
    \i script_criacao_banco.sql
    ```
