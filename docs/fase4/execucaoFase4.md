# Fase 4

## 1. Introdução

Esta fase representa a execução prática das avaliações de qualidade do Krita, baseadas nas métricas GQM definidas na [Fase 2](https://fcte-qualidade-de-software-1.github.io/2025-2_T02_DOROTHY-JOHNSON/fase2/execucaoFase2/) e nos instrumentos de medição planejados na [Fase 3](https://fcte-qualidade-de-software-1.github.io/2025-2_T02_DOROTHY-JOHNSON/fase3/execucaoFase3/). Aplicamos sistematicamente os procedimentos de coleta de dados para obter evidências objetivas sobre a Adequação Funcional e Portabilidade do software.

O objetivo é executar os testes definidos, coletar evidências através de gravações de tela e documentação sistemática, e analisar os resultados para responder às questões de pesquisa estabelecidas na metodologia GQM. Esta fase consolida todo o trabalho desenvolvido anteriormente, fornecendo dados concretos para avaliar se o Krita atende aos requisitos de qualidade no contexto de uso por artistas digitais em ambientes multiplataforma.

## 2. Aplicação do Plano de Avaliação

### 2.1. Instrumentos e Metodologia Aplicados

A execução dos testes seguiu rigorosamente os instrumentos de medição, ferramentas e protocolos definidos na **Fase 3**. Para detalhes completos sobre:

- **Ferramentas de captura** (OBS Studio)
- **Ambiente de teste controlado** (hardware padronizado, cronometragem)
- **Critérios de documentação** (nomenclatura, anotações)
- **Protocolo de execução** (setup, gravação, validação)

Consulte a documentação da [Fase 3](https://fcte-qualidade-de-software-1.github.io/2025-2_T02_DOROTHY-JOHNSON/fase3/execucaoFase3/), que estabeleceu todos os procedimentos metodológicos aplicados nesta fase de execução.

### 2.2. Contexto de Execução Realizada

**Período de Execução:** 11 a 12 de novembro de 2025

**Configuração dos Ambientes de Teste:**
- **Windows**: Versão _____, Krita ______ 
- **Linux**: Distribuição _____, Krita ______

**Equipe de Execução:**

Cada membro da equipe ficou responsável por testar **2 questões específicas** das 8 questões de pesquisa definidas na [Fase 2](https://fcte-qualidade-de-software-1.github.io/2025-2_T02_DOROTHY-JOHNSON/fase2/execucaoFase2/), garantindo cobertura completa e especialização na coleta de evidências:

| **Métrica** | **Membro(s)** |
|-------------|---------------|
| TCF | [Enzo Emir](https://github.com/EnzoEmir) |
| ICF | [Enzo Emir](https://github.com/EnzoEmir) |
| TCR | - |
| IAT | - |
| TAM | - |
| TMI | [Enzo Emir](https://github.com/EnzoEmir) |
| TSI | [Enzo Emir](https://github.com/EnzoEmir) |
| IPD | - |

## 3. Execução das Avaliações de Adequação Funcional

### 3.1. Teste de Completude Funcional (TCF)

#### 3.1.1. Objetivo da Medição
Avaliar o percentual de funcionalidades essenciais de pintura digital que estão implementadas e operacionais no Krita.

#### 3.1.2. Procedimento Executado
Baseado no checklist de funcionalidades essenciais derivado do workflow da [Fase 1](https://fcte-qualidade-de-software-1.github.io/2025-2_T02_DOROTHY-JOHNSON/fase1/execucaoFase1/#23-escopo-profundidade-e-objetos-de-avaliacao), foram testadas sistematicamente as seguintes funcionalidades:

**1. Preparação do Projeto e Esboço Inicial:**

- Criação de novo documento (definir dimensões, resolução, modelo de cor RGB, profundidade 8-bit)

- Configuração de Assistentes de Desenho (guias de perspectiva - 2 pontos de fuga)

- Ferramentas de esboço (pincéis similares a lápis, resposta à pressão, estabilizador de traço)

**2. Ferramentas de Pintura e Arte-final:**

- Pincéis de tinta para line art em nova camada

- Estabilizador de traço funcional

- Seletor de cores avançado/paletas

- Ferramenta de preenchimento (flood fill)

- Pincéis de pintura para colorização

**3. Sistema de Camadas e Gerenciamento:**

- Criação e organização de camadas

- Renomeação de camadas

- Criação de grupos de camadas

- Controle de opacidade por camada

- Modos de mesclagem (Multiply para sombras, Overlay para iluminação)

- Máscaras de camada básicas

**4. Exportação e Formatos:**

- Salvamento em formato nativo .kra (preservando camadas e metadados)

- Exportação para PNG (com transparência)

- Exportação para JPEG (com opções de compressão)

#### 3.1.3. Evidências Coletadas

<iframe width="560" height="315" src="https://www.youtube.com/embed/rRs5WbRCcIs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### 3.1.4. Análise dos Resultados

**Resultado TCF:** 100% (23 funcionalidades implementadas / 23 funcionalidades esperadas)

### 3.2. Teste de Cobertura Funcional (ICF)

#### 3.2.1. Objetivo da Medição
Medir o grau de correspondência entre as funcionalidades documentadas e as efetivamente disponíveis no software.

#### 3.2.2. Procedimento Executado
Verificação da correspondência entre funcionalidades documentadas na documentação oficial do Krita (docs.krita.org) e as implementadas no software:

**Método de Verificação:**
1. **Consulta à Documentação Oficial**: Levantamento de funcionalidades documentadas para pintura digital
2. **Teste de Disponibilidade**: Verificação da presença de cada funcionalidade documentada na interface

**Categorias Verificadas:**
Conforme as categorias de funcionalidades definidas no escopo da [Fase 1](https://fcte-qualidade-de-software-1.github.io/2025-2_T02_DOROTHY-JOHNSON/fase1/execucaoFase1/#23-escopo-profundidade-e-objetos-de-avaliacao):

- **Preparação do Projeto**: Criação de documentos, assistentes de desenho, ferramentas de esboço
- **Pintura e Arte-final**: Pincéis, estabilizador, seletor de cores, preenchimento
- **Sistema de Camadas**: Criação, organização, opacidade, modos de mesclagem, máscaras
- **Exportação e Formatos**: Salvamento .kra, exportação PNG/JPEG

#### 3.2.3. Evidências Coletadas

<iframe width="560" height="315" src="https://www.youtube.com/embed/rRs5WbRCcIs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/hHPGPiOO9zI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### 3.2.4. Análise dos Resultados

**Resultado ICF:** ___% (__ funcionalidades documentadas implementadas / __ funcionalidades documentadas)


### 3.3. Teste de Correção Funcional (TCR)

#### 3.3.1. Objetivo da Medição
Avaliar a proporção de funcionalidades que operam conforme especificado durante o workflow de criação artística.

#### 3.3.2. Procedimento Executado
Execução de casos de teste baseados no workflow da Fase 1:

**Cenário de Teste:** Criação de ilustração completa
1. **Preparação e Esboço Inicial**
2. **Pintura, Arte-final e Gerenciamento de Camadas**
3. **Exportação e Validação**

#### 3.3.3. Evidências Coletadas

#### 3.3.4. Análise dos Resultados

**Resultado TCR:** ___% (__ funcionalidades operando corretamente / __ funcionalidades testadas)

### 3.4. Teste de Adequação às Tarefas (IAT)

#### 3.4.1. Objetivo da Medição
Medir o grau de alinhamento entre as funcionalidades oferecidas e as necessidades específicas dos workflows artísticos.

#### 3.4.2. Procedimento Executado
Execução do workflow completo de ilustração dividido em 3 tarefas macro:
1. **Preparação e Esboço Inicial**
2. **Pintura, Arte-final e Gerenciamento de Camadas**
3. **Exportação e Validação**

#### 3.4.3. Evidências Coletadas

#### 3.4.4. Análise dos Resultados

**Resultado IAT:** ___% (__ tarefas completadas com sucesso / __ tarefas tentadas)

## 4. Execução das Avaliações de Portabilidade

### 4.1. Teste de Adaptabilidade Multiplataforma (TAM)

#### 4.1.1. Objetivo da Medição
Medir a capacidade do software de funcionar consistentemente em diferentes sistemas operacionais (Windows, Linux, Android).

#### 4.1.2. Procedimento Executado
Execução das funcionalidades essenciais nas 3 plataformas de desktop:

**Funcionalidades Testadas por Plataforma:**
Para cada sistema operacional, foi executado o workflow completo de ilustração e verificada a consistência de:

1. **Interface e Menus**: Layout, tradução, ícones e organização
2. **Ferramentas Core**: Pincéis, seletor de cores, camadas, exportação
3. **Performance**: Responsividade das ferramentas de pintura
4. **Shortcuts**: Funcionamento dos atalhos de teclado padrão
5. **Arquivos**: Salvamento/abertura de .kra entre plataformas
6. **Configurações**: Persistência de preferências e layouts

#### 4.1.3. Evidências Coletadas

#### 4.1.4. Análise dos Resultados

**Resultado TAM:** ___% (__ funcionalidades idênticas em todas as plataformas / __ funcionalidades testadas)

### 4.2. Teste de Instalabilidade 

#### 4.2.1. Objetivo da Medição
Cronometrar o processo de instalação e medir a taxa de sucesso em diferentes plataformas.

#### 4.2.2. Procedimento Executado

**Tempo Médio de Instalação (TMI):**
Cronometragem completa do processo de instalação em cada plataforma, desde o download até a primeira execução bem-sucedida:

**Etapas Cronometradas:**
1. **Instalação**: Execução do instalador até conclusão
2. **Primeiro Boot**: Tempo até abertura completa da interface

**Taxa de Sucesso de Instalação (TSI):**
Múltiplas tentativas de instalação em ambientes controlados:

**Cenários de Teste:**
- Instalação em sistemas "limpos" (VMs ou fresh installs)

**Critérios de Sucesso:**
- Instalação sem erros críticos
- Software inicia corretamente

#### 4.2.3. Evidências Coletadas

**TMI - Evidências Coletadas:**

<iframe width="560" height="315" src="https://www.youtube.com/embed/3jl9uRlkoNI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/JnTXEBkEHm0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

- Windows: ___ minutos (download: ___min, instalação: ___min, primeiro boot: ___min)
- Linux: ___ minutos (download: ___min, instalação: ___min, primeiro boot: ___min)  
- Android: ___ minutos (download: ___min, instalação: ___min, primeiro boot: ___min)

**TSI - Evidências Coletadas:**

<iframe width="560" height="315" src="https://www.youtube.com/embed/3jl9uRlkoNI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

- Windows: ___/2 tentativas bem-sucedidas

- Linux: ___/2 tentativas bem-sucedidas  

- Android: ___/2 tentativas bem-sucedidas


#### 4.2.4. Análise dos Resultados

**Resultado TMI:** ___ minutos (média aritmética das três plataformas)

**Resultado TSI:** ___% (__ instalações bem-sucedidas / __ tentativas totais)


### 4.3. Teste de Preservação de Dados (IPD)

#### 4.3.1. Objetivo da Medição
Medir a capacidade do software de manter integridade de arquivos e configurações entre diferentes sistemas operacionais.

#### 4.3.2. Procedimento Executado
Execução do "Teste de Consistência Multiplataforma" conforme definido na [Fase 1](https://fcte-qualidade-de-software-1.github.io/2025-2_T02_DOROTHY-JOHNSON/fase1/execucaoFase1/#23-escopo-profundidade-e-objetos-de-avaliacao):

**Protocolo de Teste:**
1. **Criação no SO 1**: Criar ilustração completa no Windows
2. **Migração para SO 2**: Transferir arquivo .kra para Linux e abrir
3. **Migração para SO 3**: Transferir mesmo arquivo para Android e abrir
4. **Verificação de Integridade**: Comparar visual e estruturalmente os projetos

**Aspectos Verificados:**
- Preservação de camadas e hierarquia
- Integridade de cores 
- Consistência de assistentes e guias
- Configurações de pincéis e texturas

#### 4.3.3. Evidências Coletadas

#### 4.3.4. Análise dos Resultados

**Resultado IPD:** ___% (__ projetos com integridade completa / __ projetos testados)

## 5. Síntese dos Resultados

### 5.1. Resumo das Métricas Obtidas

| **Métrica** | **Resultado** | **Nível** | **Hipótese** | **Status** |
|-------------|---------------|-----------|--------------|------------|
| TCF | ___% | ___ | H1: > 85% |  |
| ICF | ___% | ___ | H2: > 90% |  |
| TCR | ___% | ___ | H3: > 90% |  |
| IAT | ___% | ___ | H4: > 80% |  |
| TAM | ___% | ___ | H5: > 85% |  |
| TMI | ___ min | ___ | H6: < 15 min |  |
| TSI | ___% | ___ | H7: > 95% |  |
| IPD | ___% | ___ | H8: > 90% |  |

### 5.2. Análise Geral dos Resultados

#### 5.2.1. Adequação Funcional

#### 5.2.2. Portabilidade


## 6. Conclusões

### 6.1. Resposta à Pergunta Central
Com base nos resultados obtidos, em que medida o Krita atende aos requisitos de **Adequação Funcional** e de **Portabilidade** no contexto de tarefas típicas de pintura digital em **Windows, Linux, Android**?

## 7. Uso de IA

Durante o desenvolvimento desta fase, foi utilizada o ChatGPT como ferramenta de apoio para:

- **Revisão gramatical**: Correção de erros ortográficos e gramaticais
- **Padronização de formato**: Adequação às normas de documentação acadêmica

A IA foi empregada exclusivamente como ferramenta auxiliar, sendo todo o conteúdo técnico, métricas e análises desenvolvidos pela equipe com base nas referências bibliográficas citadas.

## Histórico de Versão

| Versão | Data | Descrição | Autor | Revisor |
| -- | -- | -- | -- | -- |
| 0.1 | 11/11/2025 | Criação da página | [Danielle Soares](https://github.com/danielle-soaress), [Enzo Emir](https://github.com/EnzoEmir), [Leticia Arisa](https://github.com/Leticia-Arisa-K-Higa), [Marcelo Makoto](https://github.com/MM4k), [Pedro Luciano](https://github.com/PedroALuciano), [Victor Pontual](https://github.com/VictorPontual) | - |

## Referências Bibliográficas

