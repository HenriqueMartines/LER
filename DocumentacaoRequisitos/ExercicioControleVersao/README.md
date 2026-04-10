# Sistema de Gerenciamento de Reservas de Hotel

## 1. Introdução 

### 1.1 Propósito

Este documento apresenta o versionamento e a evolução do requisito funcional de reservas (RF-010), garantindo a rastreabilidade e a análise de impacto diante das mudanças de negócio ocorridas entre janeiro e março de 2026.

### 1.2 Escopo

O documento abrange a definição e evolução das regras relacionadas à realização de reservas de quartos, incluindo restrições de antecedência e aplicação de tarifas conforme condições como urgência ou perfil do cliente.

### 1.3 Acrônimos - Definição

- **RF**: Requisito Funcional  
- **RNF**: Requisito Não-Funcional  
- **VIP**: Cliente com benefícios exclusivos  
- **NS**: Necessidade do Stakeholder  

### 1.4 Referências 

- IEEE 29148:2018 - Systems and software engineering  
- CMMI for Development, Version 2.0  

## 2. Descrição Geral

O sistema tem como objetivo gerenciar reservas de hotéis, permitindo validar regras de antecedência, aplicar políticas comerciais e integrar funcionalidades como autenticação de usuários e processamento de pagamentos.

## 3. Requisitos Específicos 

### 3.1 Requisito Funcional 

#### RF-010: Gestão de Prazos e Tarifas de Reserva

**Descrição**:  
O sistema deve permitir que usuários realizem reservas de quartos, validando os períodos de antecedência e aplicando tarifas conforme o nível de urgência da reserva ou o perfil do cliente.

**Prioridade**: Alta  
**Versão**: 1.0  
**Data**: 2026-03-20  
**Rastreabilidade**: Derivado das necessidades comerciais dos stakeholders NS-001 (Vendas) e NS-002 (Operações)

**Critérios de Aceitação**:

- [  ] Permitir reservas padrão com antecedência entre 24 horas e 6 meses.

- [  ] Permitir que usuários VIP reservem com até 1 ano (12 meses) de antecedência.

- [  ] Permitir reservas de "Última Hora" com menos de 2 horas de antecedência.

- [  ] Aplicar taxa adicional automática de 15% sobre o valor total em reservas de "Última Hora".

- [  ] Bloquear tentativas de reserva realizadas no intervalo de 2h a 24h de antecedência.

- [  ] Exibir o detalhamento da taxa de urgência no resumo do pagamento.

**Dependências**:  
RF-005 (Módulo de Autenticação/Status VIP)  
RF-020 (Módulo de Pagamentos)

## 4. Controle de Versão

### 4.1 Histórico de Alterações

| Versão | Data       | Autor                  | Modificação                |
|--------|------------|------------------------|----------------------------|
| 1.0    | 2026-01-15 | Analista de Requisitos | Versão inicial do documento |

## 5. Aprovação 

Matriz de Aprovação

| Alteração | Data       | Autor                  | Aprovador   |
|----------|------------|------------------------|-------------|
| 1.0      | 2026-03-15 | Analista de Requisitos | Stakeholder |