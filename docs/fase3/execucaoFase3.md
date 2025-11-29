# Fase 3

## 1. Introdução

Nesta etapa do projeto, vamos  especificar como iremos implementar e executar as métricas definidas na metodologia Goal-Question-Metric (GQM) da [Fase 2](https://fcte-qualidade-de-software-1.github.io/2025-2_T02_DOROTHY-JOHNSON/fase2/execucaoFase2/) para avaliar objetivamente a **Adequação Funcional** e **Portabilidade** do Krita. Esta abordagem foi escolhida por permitir a conversão de objetivos de qualidade em métricas concretas e mensuráveis, sendo especialmente útil para um software multiplataforma como o Krita.

O processo de coleta e análise seguirá utilizando ferramentas do Krita, de capturas de telas para evidenciar o que estará sendo testado e calculos das fórmulas para analisar os dados garantindo a rastreabilidade e reprodutibilidade dos resultados obtidos.

### 1.1. Métricas a Serem Implementadas

Com base no planejamento da Fase 2, serão coletados dados para as seguintes métricas:

**Adequação Funcional:**

- Taxa de Completude Funcional (TCF)

- Índice de Cobertura Funcional (ICF)  

- Taxa de Correção Funcional (TCR)

- Índice de Adequação às Tarefas (IAT)

**Portabilidade:**

- Taxa de Adaptabilidade Multiplataforma (TAM)

- Tempo Médio de Instalação (TMI)

- Taxa de Sucesso de Instalação (TSI)

- Índice de Preservação de Dados (IPD)

### 1.2. Ferramentas e Métodos de Coleta

#### 1.2.1. Ambiente de Teste

- **Sistemas Operacionais:** Windows 11 ou 10, Ubuntu 24.04.3 LTS, Android

- **Hardware de Teste:** Configurações padronizadas com pelo menos 8GB RAM, processador Intel i5/AMD Ryzen 5 ou equivalente

- **Versão do Krita:** Versão mais recente estável disponível no site oficial (5.2.13)

#### 1.2.2. Instrumentos de Medição

Para Adequação Funcional:

- **Checklist de Funcionalidades:** Documento estruturado baseado no escopo da Fase 1, contendo todas as funcionalidades essenciais a serem testadas

- **Cronômetro:** Para medição de tempos de execução das tarefas

- **Registro de Tela:** Software de captura (OBS Studio) para documentar a execução dos testes

Para Portabilidade:

- **Cronômetro de Precisão:** Para medição dos tempos de instalação

- **Máquinas Virtuais:** VirtualBox/VMware para testes em múltiplas plataformas de forma controlada

- **Arquivos de Teste Padronizados:** Projetos .kra com diferentes níveis de complexidade para teste de migração entre plataformas

#### 1.2.3. Processo de Coleta Passo a Passo

1. **Preparação do Ambiente**
      - Instalação limpa dos sistemas operacionais de teste
      - Configuração das máquinas virtuais com especificações padronizadas
      - Download da versão oficial do Krita para cada plataforma

2. **Execução das Medições de Adequação Funcional**
      - Execução sequencial do checklist de funcionalidades em cada plataforma
      - Registro detalhado dos resultados (sucesso/falha) para cada funcionalidade
      - Documentação de comportamentos inesperados ou erros encontrados
      - Cronometragem das tarefas do workflow artístico completo

3. **Execução das Medições de Portabilidade**
      - Cronometragem do processo de instalação completo em cada plataforma
      - Migração de projetos entre diferentes sistemas operacionais
      - Verificação da integridade de dados após migração

4. **Consolidação dos Dados**
      - Compilação dos resultados em um único documento
      - Cálculo das métricas definidas na Fase 2
      - Análise estatística descritiva dos resultados obtidos

### 1.3. Localização dos Dados de Avaliação

Os dados coletados serão organizados e armazenados na seguinte estrutura:

- **`/docs/fase4/execucaoFase4/`**: Diretório principal para todos os dados da avaliação
  - **`adequacao_funcional/`**: Resultados das métricas de adequação funcional
    - `Checklist Funcionalidades`: Dados do TCF e ICF
    - `Testes Correção`: Dados do TCR  
    - `Workflow Tarefas`: Dados do IAT
  - **`portabilidade/`**: Resultados das métricas de portabilidade
    - `Adaptabilidade em Multiplataforma`: Dados do TAM
    - `Instalação de Sistemas`: Dados do TMI e TSI
    - `Migração de projetos`: Dados do IPD
  - **`evidencias/`**: Capturas de tela, vídeos e logs dos testes realizados
  - **`analise/`**: Análises estatísticas e relatórios consolidados

Esta estrutura permitirá a rastreabilidade completa dos dados coletados e facilitará a análise posterior dos resultados obtidos.