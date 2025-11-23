# Fase 4

## 1. Introdução

Esta fase representa a execução prática das avaliações de qualidade do Krita, baseadas nas métricas GQM definidas na [Fase 2](https://fcte-qualidade-de-software-1.github.io/2025-2_T02_DOROTHY-JOHNSON/fase2/execucaoFase2/) e nos instrumentos de medição planejados na [Fase 3](https://fcte-qualidade-de-software-1.github.io/2025-2_T02_DOROTHY-JOHNSON/fase3/execucaoFase3/). Aplicamos sistematicamente os procedimentos de coleta de dados para obter evidências objetivas sobre a Adequação Funcional e Portabilidade do software.

O objetivo é executar os testes definidos, coletar evidências através de gravações de tela e documentação sistemática, e analisar os resultados para responder às questões de pesquisa estabelecidas na metodologia GQM. Esta fase consolida todo o trabalho desenvolvido anteriormente, fornecendo dados concretos para avaliar se o Krita atende aos requisitos de qualidade no contexto de uso por artistas digitais em ambientes multiplataforma.

## 2. Aplicação do Plano de Avaliação

### 2.1. Instrumentos e Metodologia Aplicados

A execução dos testes seguiu rigorosamente os instrumentos de medição, ferramentas e protocolos definidos na **Fase 3**. Para detalhes completos sobre:

- Ferramentas de captura (OBS Studio)
- Ambiente de teste controlado (hardware padronizado, cronometragem)
- Critérios de documentação (nomenclatura, anotações)
- Protocolo de execução (setup, gravação, validação)

Consulte a documentação da [Fase 3](https://fcte-qualidade-de-software-1.github.io/2025-2_T02_DOROTHY-JOHNSON/fase3/execucaoFase3/), que estabeleceu todos os procedimentos metodológicos aplicados nesta fase de execução.

### 2.2. Contexto de Execução Realizada

**Período de Execução:** 11 a 17 de novembro de 2025

**Configuração dos Ambientes de Teste:**
- **Windows**: Versão _____, Krita ______ 
- **Linux**: Distribuição _____, Krita ______

**Equipe de Execução:**

Cada membro da equipe ficou responsável por testar **2 questões específicas** das 8 questões de pesquisa definidas na [Fase 2](https://fcte-qualidade-de-software-1.github.io/2025-2_T02_DOROTHY-JOHNSON/fase2/execucaoFase2/), garantindo cobertura completa e especialização na coleta de evidências:

| **Métrica** | **Membro(s)** |
|-------------|---------------|
| TCF | [Enzo Emir](https://github.com/EnzoEmir), [Marcelo Makoto](https://github.com/MM4k) |
| ICF | [Enzo Emir](https://github.com/EnzoEmir), [Marcelo Makoto](https://github.com/MM4k) |
| TCR | [Danielle Soares](https://github.com/danielle-soaress), [Marcelo Makoto](https://github.com/MM4k), [Leticia Arisa](https://github.com/Leticia-Arisa-K-Higa) |
| IAT | - |
| TAM | - |
| TMI | [Enzo Emir](https://github.com/EnzoEmir), [Danielle Soares](https://github.com/danielle-soaress) |
| TSI | [Enzo Emir](https://github.com/EnzoEmir), [Danielle Soares](https://github.com/danielle-soaress) |
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

<iframe width="560" height="315" src="https://youtube.com/embed/pOrDbv29W5c" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### 3.1.4. Análise dos Resultados

**Resultado TCF (vídeo 1):** 100% (23 funcionalidades implementadas / 23 funcionalidades esperadas)

**Resultado TCF (vídeo 2):** 100% (33 funcionalidades testadas / 33 funcionalidades operando corretamente)

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

<iframe width="560" height="315" src="https://youtube.com/embed/pOrDbv29W5c" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://youtube.com/embed/7uKomi9D6nA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### 3.2.4. Análise dos Resultados

**Resultado ICF:** 100% (23 funcionalidades documentadas / 23 funcionalidades documentadas implementadas no software)


### 3.3. Teste de Correção Funcional (TCR)

#### 3.3.1. Objetivo da Medição
Avaliar a proporção de funcionalidades que operam conforme especificado durante o workflow de criação artística.

#### 3.3.2. Procedimento Executado
Execução de casos de teste baseados no workflow da Fase 1:

**Cenário de Teste:** Criação de ilustração completa

1. Preparação e Esboço Inicial

2. Pintura, Arte-final e Gerenciamento de Camadas

3. Exportação e Validação

#### 3.3.3. Evidências Coletadas

**Teste em um Tablet Android:**

<iframe width="560" height="315" src="https://www.youtube.com/embed/pIW6QDWi6CI?si=0HKBsAVc64Uvc17J" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

| Funcionalidade Utilizada          | Funciona? OK / INCONSISTENTE |
|-----------------------------------|--------------------------------------|
| Pincel Basic 1                    |                OK                    |
| Pincel WaterC Basic Round-Grunge  |                OK                     |
| Pincel Charcoal Pencil Large      |                OK                     |
| Pincel Marker Details             |               OK                     |
| Pincel Wet Paint Plus             |               OK                    |
| Borracha Eraser Circle            |               OK                     |
| Pick Colors                       | INCONSISTENTE – não pegou as cores desejadas |
| Paleta de Cores                   |                OK                     |
| Ferramenta de Camadas             |                 OK                   |
| Opacidade de Pincéis              |                OK                    |
| Tamanho de Pincéis                |                OK                    |
| Zoom                              |               OK                      |
| Rotate Canvas                     |              OK                     |
| Desfazer                          | INCONSISTENTE – difícil manuseio, não funcionou sempre     |
| Fazer                             | INCONSISTENTE – difícil manuseio, não funcionou sempre    |

!!! info "Resultado Consolidado"
    **TCR:** 73,33%  
    **Funcionalidades Testadas:** 15  
    **Operando Corretamente:** 11  


**Teste em um Desktop Windows:**

<iframe width="560" height="315" src="https://www.youtube.com/embed/LXjZK_MJfPA?si=sk9MIklQU79cxYlp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


| Funcionalidade Utilizada                 | Funciona? OK / INCONSISTENTE |
|------------------------------------------|--------------------------------------|
| Pincel Basic 1                           |            OK              |
| Pincel Marker Medium                     |            OK                  |
| Pincel Basic 5 Size                      |     OK             |
| Pincel Basic 4 Flow Opacity              |   OK         |
| Pincel WaterC Spread WideArea            |    OK         |
| Pincel WaterC Basic Round-Fringe 02      |    OK         |
| Pincel WaterC Spread Pattern             |        OK       |
| Pincel Texture Impressionism             |        OK         |
| Pincel WaterColor Texture                |   OK      |
| Pincel WaterColor Fringe                 |      OK  |
| Pincel Blender Blur                      | OK        |
| Pincel Stamp Leaves                      | OK        |
| Pincel Stamp Stylised Tree               | OK        |
| Pincel Stamp Herbals                     | OK        |
| Ferramenta de Pick Colors                | OK        |
| Ferramenta de Paleta de Cores            | OK        |
| Ferramenta de Camadas                    | OK        |
| Ferramenta de Opacidade de Pincéis       | OK        |
| Ferramenta de Tamanho de Pincéis         | OK        |
| Zoom                                     |      OK             |
| Rotate Canvas                            |        OK               |
| Desfazer                                 |         OK             |
| Fazer                                    |          OK        |
| Exportar (PNG e .kra)                     |             OK         |


!!! info "Resultado Consolidado"
    **TCR:** 100%  
    **Funcionalidades Testadas:** 24  
    **Operando Corretamente:** 24  

<iframe width="560" height="315" src="https://youtube.com/embed/pOrDbv29W5c" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

| Funcionalidade Utilizada                 | Funciona? OK / INCONSISTENTE |
|------------------------------------------|--------------------------------------|
| Airbrush Soft                           |            OK              |
| Pincel Basic 1                     |            OK                  |
| Eraser Circle                      |     OK             |
| Pincel Basic 5 Size              |   OK         |
| Charcoal Rock Soft            |    OK         |
| Water C Special Splats      |    OK         |
| RGBA 06 Rock             |        OK       |
| Texture Large Splat             |        OK         |
| Texture Random Particles                |   OK      |
| Texture Spines                 |      OK  |
| Texture Splats                      | OK        |
| Texture Spray                      | OK        |
| Texture Starfield               | OK        |
| Texture Wood Fiber                     | OK        |
| Stamp Bokeh                | OK        |
| Stamp Floor            | OK        |
| Stamp Grass                    | OK        |
| Stamp Grass Patch       | OK        |
| Stamp Herbals         | OK        |
| Stamp Leaves         | OK        |
| Stamp Mountains Distant         | OK        |
| Stamp Shoujo Bubbles         | OK        |
| Stamp Sparkles         | OK        |
| Stamp Stylised Tree         | OK        |
| Adicionar Camadas         | OK        |
| Ocultar Camadas         | OK        |
| Selecionar Camada         | OK        |
| Selecionar Cores         | OK        |
| Alterar Opacidade         | OK        |
| Alterar Tamanho de Pincéis         | OK        |
| Zoom                                     |      OK             |
| Desfazer                                 |         OK             |
| Exportar (PNG e .kra)                     |             OK         |


!!! info "Resultado Consolidado"
    **TCR:** 100%  
    **Funcionalidades Testadas:** 33  
    **Operando Corretamente:** 33  


<iframe width="560" height="315" src="https://www.youtube.com/embed/qzcHjYInLIg?si=do5hPVPjhpUjZuZZ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

| Funcionalidade Utilizada                 | Funciona? OK / INCONSISTENTE |
|------------------------------------------|--------------------------------------|
| Definir Dimensões do Documento           | OK                                   |
| Selecionar Camada                        | OK                                   |
| Organizar Camada                         | OK                                   |
| Selecionar Cores                         | OK                                   |
| Alterar Opacidade                        | OK                                   |
| Alterar Tamanho de Pincéis               | OK                                   |
| Zoom                                     | OK                                   |
| Desfazer                                 | OK                                   |
| Exportar (PNG e .kra)                    | OK                                   |
| Draw a Gradient                          | OK                                   |
| Pencil-1 Hard                            | OK                                   |
| Polyline                                 | OK                                   |
| Eraser Circle                            | OK                                   |
| Bristles - 4 Glaze                       | OK                                   |
| Fill                                     | OK                                   |
| Adjuste Color                            | OK                                   |
| Stamp Grass                              | OK                                   |
| Stamp Vegetal                            | OK                                   |
| Bristles - 5 Flat                        | OK                                   |
| Texture Starfield                        | OK                                   |
| Stamp Sparkles                           | OK                                   |
| Ellipse                                  | OK                                   |
| Basic - 6 Details                        | OK                                   |
| Adjuste Overlay Burn                     | OK                                   |
| Stamp Leaves                             | OK                                   |
| Basic - 5 Opacity                        | OK                                   |


!!! info "Resultado Consolidado"
    **TCR:** 100%  
    **Funcionalidades Testadas:** 25
    **Operando Corretamente:** 25


<iframe width="560" height="315" src="https://www.youtube.com/embed/tHBhAd5j6Ao?si=D-tQk2Kdl2Aiv82i" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


| Funcionalidade Utilizada                 | Funciona? OK / INCONSISTENTE |
|------------------------------------------|--------------------------------------|
| Definir dimensões do documento           | OK                                   | 
| Assistente de Desenho                    | OK                                   | 
| Pencil-1 Hard                            | INCONSISTENTE                        |
| Polyline                                 | OK                                   | 
| Free Hand Path                           | OK                                   | 
| Eraser Circle                            | OK                                   | 
| Eraser Small                             | OK                                   | 
| Pencil-5 Tilted                          | OK                                   | 
| Selecionar Camada                        | OK                                   | 
| Organizar Camada                         | OK                                   | 
| Selecionar Cores                         | OK                                   | 
| Alterar Opacidade                        | OK                                   | 
| Alterar Tamanho de Pincéis               | OK                                   | 
| Zoom                                     | OK                                   | 
| Desfazer                                 | OK                                   | 
| Exportar (PNG e .kra)                    | OK                                   | 
| Dry Roller                               | OK                                   | 
| Basic - 6 Details                        | OK                                   | 
| Bristles - 5 Flat                        | OK                                   | 
| Stamp Leaves                             | OK                                   | 
| Stamp Grass Patch                        | OK                                   | 
| Stamp Grass                              | OK                                   | 
| Texture Big                              | OK                                   | 
| Dry Bristles                             | OK                                   | 
| Blender Blur                             | OK                                   | 
| Dry Bristles Eroded                      | OK                                   | 
| Dry Textured Creases                     | OK                                   | 
| Stamp Herbals                            | OK                                   |
| Ellipse                                  | OK                                   | 
| Adjuste Overlay Burn                     | OK                                   | 
| Line                                     | OK                                   | 


!!! info "Resultado Consolidado"
    **TCR:** 100%  
    **Funcionalidades Testadas:** 31
    **Operando Corretamente:** 31

#### 3.3.4. Análise dos Resultados

Considerando os testes realizados em diferentes plataformas, dispositivos e estilos de desenho, a consolidação dos resultados é calculada pela soma de todas as funcionalidades testadas e de todas as funcionalidades que apresentaram funcionamento correto.

**Resultado TCR:** ___% (__ funcionalidades operando corretamente / __ funcionalidades testadas)

## 3.4. Teste de Adequação às Tarefas (IAT)

### 3.4.1. Objetivo da Medição

Medir o grau de alinhamento entre as funcionalidades oferecidas pelo Krita e as necessidades específicas do workflow artístico.
O IAT avalia se as ferramentas disponíveis permitem executar integralmente o ciclo de criação de uma ilustração digital, considerando fluidez, continuidade do processo e ausência de impedimentos funcionais.

### 3.4.2. Procedimento Executado

O workflow completo de produção artística foi executado em três tarefas macro:

1. Preparação e Esboço Inicial: criação do documento, configuração do ambiente de trabalho, ajuste e uso de pincéis para sketch, manipulação de camadas e definição da composição inicial.

2. Pintura, Arte-final e Gerenciamento de Camadas: construção de lineart, aplicação de pintura base, ajustes visuais e organização de camadas durante o processo criativo.

3. Exportação e Validação: revisão visual da arte final, conferência de dimensões e resolução, exportação do projeto e verificação de compatibilidade.

Todas as etapas foram aplicadas de forma prática ao longo de diferentes cenários de teste.

### 3.4.3. Evidências Coletadas

Vídeos de execução do workflow:

<iframe width="560" height="315" src="https://www.youtube.com/embed/cc9QCvoG0vU?si=FveR5SiwMNXvjbri" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Durante a execução dos fluxos, foi possível observar que as ferramentas essenciais permitiram o desenvolvimento completo das tarefas previstas, desde a construção do sketch e manipulação de pincéis até a finalização e exportação do artefato.

### 3.4.4. Análise dos Resultados

O fluxo artístico completo foi concluído sem barreiras funcionais. As ferramentas de desenho, camadas, navegação, edição e exportação suportaram integralmente as necessidades das tarefas macro executadas.

O resultado foi calculado pela relação entre tarefas concluídas e tarefas tentadas:

**IAT = (Tarefas macro concluídas / Tarefas macro tentadas) × 100**

Foram tentadas 3 tarefas macro e todas foram concluídas com sucesso:

**IAT = (3 / 3) × 100 = 100%**

### Resultado IAT

**100% (3 tarefas concluídas / 3 tarefas tentadas)**

O Krita demonstrou adequação total às necessidades práticas de criação artística digital dentro do workflow analisado, permitindo a execução contínua e completa desde o início da ilustração até sua exportação final.


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

**Teste em um Desktop Windows:**

<iframe width="560" height="315" src="https://www.youtube.com/embed/cQSAtqY1CCg?si=ZnPgSON2SL_rB1RE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

| Funcionalidade Testada                 | Funciona? Sucesso / Falha |
|------------------------------------------|--------------------------------------|
| Layout                                   | Sucesso                              |
| Tradução                                 | Sucesso                              |
| Ícones                                   | Sucesso                              |
| Organização                              | Sucesso                              |
| Pincéis                                  | Sucesso                              |
| Seletor de Cores                         | Sucesso                              |
| Camadas                                  | Sucesso                              |
| Exportação                               | Sucesso                              |
| Responsividade                           | Sucesso                              |
| Atalhos                                  | Sucesso                              |
| Salvamento do arquivo                    | Sucesso                              |
| Abertura do arquivo                      | Sucesso                              |
| Persistência                             | Sucesso                              |


!!! info "Resultado Consolidado"
    **TAM:** 100%  
    **Funcionalidades Testadas:** 13
    **Operando Identicamente:** 13


**Teste em um Desktop Linux:**

<iframe width="560" height="315" src="https://www.youtube.com/embed/LUd0esNwM5c?si=SBsccrrHYL3rlpTj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


| Funcionalidade Testada                 | Funciona? Sucesso / Falha |
|------------------------------------------|--------------------------------------|
| Layout                                   | Sucesso                              |
| Tradução                                 | Sucesso                              |
| Ícones                                   | Sucesso                              |
| Organização                              | Sucesso                              |
| Pincéis                                  | Sucesso                              |
| Seletor de Cores                         | Sucesso                              |
| Camadas                                  | Sucesso                              |
| Exportação                               | Sucesso                              |
| Responsividade                           | Sucesso                              |
| Atalhos                                  | Sucesso                              |
| Salvamento do arquivo                    | Sucesso                              |
| Abertura do arquivo                      | Sucesso                              |
| Persistência                             | Sucesso                              |


!!! info "Resultado Consolidado"
    **TAM:** 100%  
    **Funcionalidades Testadas:** 13
    **Operando Identicamente:** 13

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

#### Vídeos de Instalação

Android:

<iframe width="560" height="315" src="https://www.youtube.com/embed/1LrzdEJ75pA?si=Gqf1evNEkRG_aUhX" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Ubuntu (Linux):

<iframe width="560" height="315" src="https://www.youtube.com/embed/twd9sgbbIl0?si=0YZzZ_2EiiVGBqRJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Windows 10:

<iframe width="560" height="315" src="https://www.youtube.com/embed/GK9HIM5Qsp4?si=BO7fJ80Q0-sn1etT" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Windows 11:

<iframe width="560" height="315" src="https://www.youtube.com/embed/3jl9uRlkoNI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/JnTXEBkEHm0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


**TMI - Evidências Coletadas:**

- Windows: ___ minutos (download: ___min, instalação: ___min, primeiro boot: ___min)
- Linux: ___ minutos (download: ___min, instalação: ___min, primeiro boot: ___min)  
- Android: ___ minutos (download: ___min, instalação: ___min, primeiro boot: ___min)

**TSI - Evidências Coletadas:**

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

**Teste de Consistência Multiplataforma:**

O teste foi executado em 3 projetos distintos, cada um contendo ilustrações completas com múltiplas camadas, modos de mesclagem, assistentes de desenho e configurações avançadas de pincéis.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Oz1bROo37b4?si=S05FtJtyD-NOkUME" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/9WUxjhUjL3k?si=mWmvPVuq05MHaqNQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**Resultados da Verificação de Integridade:**

Para cada projeto testado, os seguintes aspectos foram verificados após migração entre plataformas (Windows → Linux → Android):

| Aspecto Verificado | Projeto 1 | Projeto 2 | Projeto 3 |
|-------------------|-----------|-----------|-----------|
| Preservação de camadas e hierarquia | Íntegro | Íntegro | Íntegro |
| Integridade de cores | Íntegro | Íntegro | Íntegro |
| Consistência de assistentes e guias | Íntegro | Íntegro | Íntegro |
| Configurações de pincéis e texturas | Íntegro | Íntegro | Íntegro |

Todos os três projetos mantiveram integridade completa ao serem transferidos entre as diferentes plataformas. As camadas permaneceram organizadas, as cores foram preservadas sem alterações, os assistentes de desenho continuaram funcionais e todas as configurações de pincéis foram mantidas.

#### 4.3.4. Análise dos Resultados

Os testes demonstraram que o formato nativo .kra do Krita é completamente portável entre diferentes sistemas operacionais. Todos os projetos testados mantiveram 100% de sua integridade estrutural e visual ao serem migrados entre Windows, Linux e Android.

O resultado foi calculado pela relação entre projetos que mantiveram integridade completa e o total de projetos testados:

**IPD = (Projetos com integridade completa / Projetos testados) × 100**

**IPD = (3 / 3) × 100 = 100%**

**Resultado IPD:** 100% (3 projetos com integridade completa / 3 projetos testados)

Este resultado confirma que o Krita garante total preservação de dados multiplataforma, permitindo que artistas trabalhem no mesmo projeto em diferentes sistemas operacionais sem perda de informações ou necessidade de conversões.

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
| IPD | 100% | 100% | H8: 100% > 90% | Aprovado |

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
| 0.2 | 11/11/2025 | Adição das evidências | [Enzo Emir](https://github.com/EnzoEmir)| - |
| 0.3 | 16/11/2025 | Adição de evidências para TCR, TMI e TSI, além de cálculos preliminares do TCR | [Danielle Soares](https://github.com/danielle-soaress)| - |
| 0.4 | 17/11/2025 | Adição de evidências para TCF, ICF e TCR | [Marcelo Makoto](https://github.com/MM4k)| - |
| 0.5 | 17/11/2025 | Adição de evidências para TCR | [Leticia Arisa](https://github.com/Leticia-Arisa-K-Higa)| - |
| 0.6 | 17/11/2025 | Adição de evidência para ICF | [Marcelo Makoto](https://github.com/MM4k)| - |

## Referências Bibliográficas

