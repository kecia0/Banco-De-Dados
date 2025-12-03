# Modelo Logico

![IoT](https://img.shields.io/badge/IoT-Sensors-blue?style=for-the-badge&logo=internetofthings&logoColor=white) ![Database](https://img.shields.io/badge/Database-SQL-orange?style=for-the-badge&logo=postgresql&logoColor=white) ![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

> **"Monitorando o pulso da cidade: veículos, rotas e eventos em tempo real."**

## 📡 Sobre o Projeto
Este repositório contém a modelagem de dados para o **UrbanPulse**, uma plataforma de gestão de mobilidade urbana. O sistema foi projetado para integrar dados de frotas de transporte com sensores IoT, permitindo o rastreamento de viagens, incidentes e tarifação dinâmica.

## 🧠 Arquitetura de Dados

O banco de dados orquestra três pilares principais:

### 1. 🚌 Frota e Logística
Gerenciamento físico dos ativos da cidade.
*   **`Veiculo`**: Rastreados individualmente por Placa e Status.
*   **`Rota`**: Definição de trajetos com cálculo de distância e tempo estimado.

### 2. 📡 Monitoramento IoT (Internet of Things)
Camada de inteligência em tempo real.
*   **`Sensor`**: Dispositivos acoplados aos veículos.
*   **`EventoMobilidade`**: Registra incidentes (trânsito, acidentes, falhas) detectados pelos sensores.

### 3. 👤 Usuários e Operação
Controle de acesso e tarifação.
*   **`Usuario`** & **`TipoUsuario`**: Sistema de tarifação segmentada (Estudante, Idoso, Comum) baseada na tabela de tarifas.
*   **`Viagem`**: O registro histórico de quem usou o que, quando e onde.

---
