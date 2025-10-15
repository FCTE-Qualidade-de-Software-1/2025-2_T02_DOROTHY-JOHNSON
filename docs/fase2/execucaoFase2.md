# Fase 2

## Introdução

Nesta etapa do projeto, aplicamos a metodologia Goal-Question-Metric (GQM) para avaliar objetivamente a qualidade do Krita. Esta abordagem foi escolhida por permitir a conversão de objetivos de qualidade em métricas concretas e mensuráveis, sendo especialmente útil para um software multiplataforma como o Krita.

Com base nas características priorizadas na [Fase 1](https://fcte-qualidade-de-software-1.github.io/2025-2_T02_DOROTHY-JOHNSON/fase1/execucaoFase1/), definimos questões específicas e métricas correspondentes para avaliar a Adequação Funcional e Portabilidade do software. O objetivo é quantificar o desempenho do Krita em cenários reais de uso por artistas digitais.

## Explicando GQM

A metodologia **Goal-Question-Metric (GQM)** é uma abordagem sistemática para definição e interpretação de métricas de software. Esta metodologia segue uma estrutura hierárquica descendente que conecta objetivos organizacionais a medições específicas.

### Estrutura da Metodologia GQM

**Goal (Objetivo)**: Define o propósito da medição de forma conceitual, especificando:

- **Objeto de análise**: O que será analisado 
- **Propósito**: Por que medir 
- **Característica de qualidade**: O foco da análise 
- **Sob o Ponto de Vista**: De qual ponto de vista está sendo analisado
- **Contexto**: Ambiente da medição 

**Question (Questão)**: Operacionaliza o objetivo através de questões específicas que caracterizam o objeto de estudo em relação ao propósito estabelecido.

**Metric (Métrica)**: Fornece dados quantitativos ou qualitativos para responder às questões de forma objetiva e mensurável.

<br>

# Adequação Funcional

## Descrição do Objetivo de Medição de Adequação Funcional

<font size="3"><p style="text-align: center">Tabela 1: Descrição do Objetivo de Medição de Adequação Funcional</p></font>

| **Elemento** | **Descrição** |
|--------------|---------------|
| **ANALISAR** | Krita |
| **PROPÓSITO** | Entender |
| **COM RESPEITO A:** | Adequação Funcional |
| **SOB O PONTO DE VISTA** | Artista Digital |
| **CONTEXTO** | Disciplina Qualidade de Software 1 |

<font size="3"><p style="text-align: center">Fonte: Adaptado de Basili e Weiss (1984).</p></font>

## Questões e Métricas

### Q1: Em que medida o Krita atende aos requisitos funcionais em tarefas típicas de pintura digital?

Para avaliar a completude funcional do Krita, utilizaremos a métrica de **Taxa de Completude Funcional (TCF)**, que mede o percentual de funcionalidades essenciais de pintura digital que estão implementadas e operacionais.

> **Fórmula:**
>
> TCF(%) = (Número de funcionalidades implementadas corretamente ÷ Total de funcionalidades esperadas) × 100

#### Hipótese

**H1:** O Krita apresenta uma Taxa de Completude Funcional superior a 85% para tarefas essenciais de pintura digital (camadas, pincéis, exportação).

### Q2: Quais funcionalidades essenciais do Krita apresentam comportamento incorreto ou inadequado durante o workflow de criação artística?

Para medir a correção funcional, utilizaremos a **Taxa de Correção Funcional (TCR)**, que avalia a proporção de funcionalidades que operam conforme especificado.

> **Fórmula:**
>
> TCR(%) = (Número de funcionalidades que operam corretamente ÷ Total de funcionalidades testadas) × 100

#### Hipótese

**H2:** A Taxa de Correção Funcional do Krita é superior a 90% para funcionalidades core, demonstrando alta confiabilidade operacional.

### Q3: Como a completude funcional do Krita se compara às necessidades específicas de diferentes estilos e técnicas de arte digital?

Para avaliar a adequação funcional, utilizaremos o **Índice de Adequação às Tarefas (IAT)**, que mede o grau de alinhamento entre as funcionalidades oferecidas e as necessidades específicas dos workflows artísticos.

> **Fórmula:**
>
> IAT(%) = (Tarefas artísticas completadas com sucesso ÷ Total de tarefas artísticas tentadas) × 100

#### Hipótese

**H3:** O Índice de Adequação às Tarefas do Krita é superior a 80% para workflows de ilustração.

# Portabilidade

## Descrição do Objetivo de Medição de Portabilidade

<font size="3"><p style="text-align: center">Tabela 2: Descrição do Objetivo de Medição de Portabilidade</p></font>

| **Elemento** | **Descrição** |
|--------------|---------------|
| **ANALISAR** | Krita |
| **PROPÓSITO** | Entender |
| **COM RESPEITO A:** | Portabilidade |
| **SOB O PONTO DE VISTA** | Artista Digital |
| **CONTEXTO** | Disciplina Qualidade de Software 1 |

<font size="3"><p style="text-align: center">Fonte: Adaptado de Basili e Weiss (1984).</p></font>

## Questões e Métricas

### Q1: Em quais aspectos de portabilidade o Krita apresenta limitações para artistas digitais?

Para avaliar a adaptabilidade, utilizaremos a **Taxa de Adaptabilidade Multiplataforma (TAM)**, que mede a capacidade do software de funcionar consistentemente em diferentes sistemas operacionais.

> **Fórmula:**
>
> TAM(%) = (Funcionalidades que operam identicamente em todas as plataformas ÷ Total de funcionalidades testadas) × 100

#### Hipótese

**H4:** A Taxa de Adaptabilidade Multiplataforma do Krita é superior a 85% entre Windows, Linux e macOS.

### Q2: Qual é o grau de adaptabilidade do Krita em diferentes sistemas operacionais e configurações de hardware?

Para medir a instalabilidade, utilizaremos o **Tempo Médio de Instalação (TMI)** e a **Taxa de Sucesso de Instalação (TSI)**.

> **Fórmula TMI:**
>
> TMI(minutos) = Σ(Tempo de instalação por plataforma) ÷ Número de plataformas testadas
>
> **Fórmula TSI:**
>
> TSI(%) = (Instalações bem-sucedidas ÷ Total de tentativas de instalação) × 100

#### Hipóteses

**H5:** O Tempo Médio de Instalação do Krita é inferior a 15 minutos em todas as plataformas suportadas.

**H6:** A Taxa de Sucesso de Instalação do Krita é superior a 95% em ambientes padrão.

### Q3: Como o Krita mantém a consistência de projetos e configurações ao migrar entre diferentes plataformas?

Para avaliar a consistência de dados, utilizaremos o **Índice de Preservação de Dados (IPD)**, que mede a capacidade do software de manter integridade de arquivos e configurações entre diferentes sistemas operacionais.

> **Fórmula:**
>
> IPD(%) = (Projetos que mantêm integridade completa após migração ÷ Total de projetos testados na migração) × 100

#### Hipótese

**H7:** O Índice de Preservação de Dados do Krita é superior a 90%, garantindo integridade de projetos e configurações durante migrações entre plataformas.


## Referências Bibliográficas

- **ISO/IEC 25010:2011 (BS ISO/IEC 25010:2011)**. Systems and software engineering — Systems and software Quality Requirements and Evaluation (SQuaRE) — System and software quality models. British Standards Institution, 2011.
- **UNIVERSIDADE FEDERAL DE PERNAMBUCO**. CENTRO DE INFORMÁTICA. GQM (Goal, Question, Metric). [2009]. Material de Seminário. Disponível em: https://www.cin.ufpe.br/~scbs/metricas/seminarios/GQM_texto.pdf. Acesso em: 14 out. 2025.
- **BASILI, Victor R.; WEISS, David M.** A Methodology for Collecting Valid Software Engineering Data. [1984]. Proceedings of the 2nd International Conference on Software Engineering. IEEE Computer Society Press. Disponível em: https://www.cs.umd.edu/users/basili/publications/proceedings/P131.pdf


## Uso de IA

Durante o desenvolvimento desta fase, foi utilizada Inteligência Artificial (IA) como ferramenta de apoio para:

- **Revisão gramatical**: Correção de erros ortográficos e gramaticais
- **Padronização de formato**: Adequação às normas de documentação acadêmica

A IA foi empregada exclusivamente como ferramenta auxiliar, sendo todo o conteúdo técnico, métricas e análises desenvolvidos pela equipe com base nas referências bibliográficas citadas.



## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| -- | -- | -- | -- | -- |
| 0.0 | 08/10/2025 | Criação da estrutura GQM inicial | [Danielle Soares](https://github.com/danielle-soaress), [Enzo Emir](https://github.com/EnzoEmir), [Leticia Arisa](https://github.com/Leticia-Arisa-K-Higa), [Marcelo Makoto](https://github.com/MM4k), [Pedro Luciano](https://github.com/PedroALuciano), [Victor Pontual](https://github.com/VictorPontual) | [Danielle Soares](https://github.com/danielle-soaress), [Enzo Emir](https://github.com/EnzoEmir), [Leticia Arisa](https://github.com/Leticia-Arisa-K-Higa), [Marcelo Makoto](https://github.com/MM4k), [Pedro Luciano](https://github.com/PedroALuciano), [Victor Pontual](https://github.com/VictorPontual) |
| 0.2 | 14/10/2025 | Adição das Questões, Métricas e Hipóteses | [Danielle Soares](https://github.com/danielle-soaress), [Enzo Emir](https://github.com/EnzoEmir), [Leticia Arisa](https://github.com/Leticia-Arisa-K-Higa), [Marcelo Makoto](https://github.com/MM4k), [Pedro Luciano](https://github.com/PedroALuciano), [Victor Pontual](https://github.com/VictorPontual) | [Danielle Soares](https://github.com/danielle-soaress), [Enzo Emir](https://github.com/EnzoEmir), [Leticia Arisa](https://github.com/Leticia-Arisa-K-Higa), [Marcelo Makoto](https://github.com/MM4k), [Pedro Luciano](https://github.com/PedroALuciano), [Victor Pontual](https://github.com/VictorPontual) |
| 0.3 | 14/10/2025 | Adição da Explicação do GQM | [Danielle Soares](https://github.com/danielle-soaress), [Enzo Emir](https://github.com/EnzoEmir), [Leticia Arisa](https://github.com/Leticia-Arisa-K-Higa), [Marcelo Makoto](https://github.com/MM4k), [Pedro Luciano](https://github.com/PedroALuciano), [Victor Pontual](https://github.com/VictorPontual) | [Danielle Soares](https://github.com/danielle-soaress), [Enzo Emir](https://github.com/EnzoEmir), [Leticia Arisa](https://github.com/Leticia-Arisa-K-Higa), [Marcelo Makoto](https://github.com/MM4k), [Pedro Luciano](https://github.com/PedroALuciano), [Victor Pontual](https://github.com/VictorPontual) |
| 0.4 | 14/10/2025 | Organizando Hipóteses | [Leticia Arisa](https://github.com/Leticia-Arisa-K-Higa), [Pedro Luciano](https://github.com/PedroALuciano), [Victor Pontual](https://github.com/VictorPontual) | [Danielle Soares](https://github.com/danielle-soaress), [Enzo Emir](https://github.com/EnzoEmir), [Leticia Arisa](https://github.com/Leticia-Arisa-K-Higa), [Marcelo Makoto](https://github.com/MM4k), [Pedro Luciano](https://github.com/PedroALuciano), [Victor Pontual](https://github.com/VictorPontual) |
| 0.5 | 14/10/2025 | Adição de Referência nas tabelas de GQM | [Enzo Emir](https://github.com/EnzoEmir), [Marcelo Makoto](https://github.com/MM4k) | [Danielle Soares](https://github.com/danielle-soaress), [Enzo Emir](https://github.com/EnzoEmir), [Leticia Arisa](https://github.com/Leticia-Arisa-K-Higa), [Marcelo Makoto](https://github.com/MM4k), [Pedro Luciano](https://github.com/PedroALuciano), [Victor Pontual](https://github.com/VictorPontual) |
