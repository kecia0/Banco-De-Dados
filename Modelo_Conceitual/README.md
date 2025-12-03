# MODELAGEM CONCEITUAL

![Banner](https://capsule-render.vercel.app/api?type=waving&color=007bff&height=220&section=header&text=Modelagem%20de%20Dados&fontSize=60&fontColor=ffffff&desc=Sistema%20de%20Gest%C3%A3o%20de%20Transporte&descAlignY=60&descAlign=50)

> **"Conectando pessoas aos seus destinos através de dados estruturados."**

## 🗺️ Sobre o Projeto
Este repositório apresenta a modelagem conceitual de um banco de dados robusto desenvolvido para gerenciar um ecossistema de transporte urbano. O sistema integra usuários, frotas de veículos, rotas inteligentes e múltiplos meios de pagamento.

---


## 🧩 Entidades e Regras de Negócio

O sistema foi arquitetado em módulos principais para garantir a integridade das operações:

| Módulo | Descrição Funcional | Entidades Relacionadas |
| :--- | :--- | :--- |
| **👤 Gestão de Usuários** | Controle de dados cadastrais e histórico de interações. | `Usuario`, `Bilhete_Unico` |
| **💳 Financeiro** | Processamento de recargas, pagamentos e tipos de transação. | `Recarga`, `Tipo_Pagamento`, `Paga` |
| **🚌 Frota & Rotas** | Logística de veículos, definição de trajetos e paradas estratégicas. | `Veiculos`, `Rota`, `Parada_Rota` |
| **🚲 Serviços** | Gestão de aluguéis (ex: bikes/patinetes) e uso do transporte. | `Aluguel`, `Faz_Trajeto` |

---

## 🛠️ Stack Utilizada
*   **Modelagem:** brModelo / Conceitual
*   **Paradigma:** Relacional
*   **Normalização:** 3FN (Terceira Forma Normal)

