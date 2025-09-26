# Fase 1

## 1. Aplicação Escolhida 

O software avaliado neste trabalho é o Krita, um aplicativo livre e de código aberto para pintura digital e ilustração mantido pela comunidade KDE/Krita Foundation. Trata-se de uma aplicação multiplataforma — com pacotes oficiais para Windows, Linux e macOS, além de versão para tablets Android — voltada a artistas, ilustradores e criadores de concept art, quadrinhos, texturas e matte painting. O repositório oficial está hospedado no [Krita](https://github.com/KDE/krita). 

Embora difundido amplamente, o Krita não é um produto comercial proprietário; é distribuído sob licença GPLv3, com desenvolvimento aberto e colaborativo. No enquadramento de aquisição e uso, ele se comporta como um software de prateleira (off-the-shelf) de código aberto, disponibilizado ao público em geral, sem personalizações específicas por cliente. 

O domínio de aplicação do Krita abrange a criação artística digital, educação em artes visuais e fluxos de trabalho de estúdios e profissionais independentes que necessitam de um estúdio de arte 2D completo, com suporte a camadas, pincéis avançados e formatos amplamente utilizados (ex.: PSD). 


## 2. Propósito da avaliação

### 2.1. Requisitante e partes interessadas
<!-- *(comprador, fornecedor, desenvolvedor, operador, etc.)* -->

<!-- Descrever aqui quem está solicitando a avaliação e todas as partes interessadas envolvidas no processo -->

O requisitante principal do Krita é a comunidade de usuários finais, composta por artistas digitais, ilustradores, quadrinistas, animadores e designers que buscam uma solução acessível e completa para criação de artes digitais [[1]](#REF1). A demanda por melhorias e novas funcionalidades parte majoritariamente desses usuários, por meio de fóruns, enquetes, relatórios de erros e sugestões de recursos.

As partes interessadas envolvidas no processo também incluem [[1]](#REF1) [[2]](#REF2):

- Os desenvolvedores voluntários e colaboradores, responsáveis pela implementação de recursos, correções de falhas e manutenção do código aberto;

- Mantenedores do projeto, que coordenam a evolução do software, definem prioridades e integram as contribuições enviadas;

- Testadores e demais membros da comunidade que validam versões, reportam problemas e sugerem ajustes;

- Distribuidores e mantenedores de pacotes, como repositórios Linux e lojas de aplicativos, que asseguram que o software esteja acessível e atualizado em diferentes plataformas;

- Apoiadores financeiros, como doadores, patrocinadores e iniciativas de financiamento coletivo;

- Os operadores, em que se destacam-se artistas, estúdios independentes e instituições de ensino, que utilizam o Krita em seus fluxos de trabalho e ajudam na sua difusão.


### 2.2. Propósito da avaliação e uso pretendido dos resultados

Este trabalho, desenvolvido na disciplina de Qualidade de Software, tem como propósito gerar evidências objetivas sobre a qualidade do Krita (projeto KDE) à luz do SQuaRE/ISO/IEC 25010 e transformá-las em decisões práticas para uso e melhoria do produto. Em termos simples: queremos saber o quão bem o Krita atende ao que promete e o quão bem ele se comporta entre plataformas.

**Pergunta central**  
> Em que medida o Krita atende aos requisitos de **Adequação Funcional** e de **Portabilidade** no contexto de tarefas típicas de pintura digital (camadas, pincéis, abertura/salvamento/exportação) em **Windows, Linux, macOS e Android**?

**Objetivos específicos**
1. **Identificar e priorizar** características de qualidade relevantes para o público-alvo.  
2. **Avaliar e medir** as subcaracterísticas selecionadas do ISO/IEC 25010:  
   - **Adequação Funcional**: *completude*, *correção* e *adequação às tarefas*.  
   - **Portabilidade**: *adaptabilidade*, *instalabilidade* e *substituibilidade*.  
3. **Propor recomendações** de melhoria contínua (curto e médio prazo).  
4. **Verificar aderência** a normas e boas práticas, registrando uma **linha de base** para reavaliações futuras.

**Escopo desta Fase 1**  
Foco nas duas características priorizadas (**Funcionalidade/Adequação Funcional** e **Portabilidade**), em **cenários multiplataforma** representativos do uso real do Krita, produzindo insumos claros para as fases seguintes do processo de avaliação.

### 2.3. Escopo, profundidade e objetos de avaliação
*(incluindo relação com avaliações anteriores ou futuras, quando aplicável)*

<!-- Definir o escopo da avaliação, qual será a profundidade da análise e quais objetos serão avaliados -->

### 2.4. ODS relacionados e metas associadas ao software
<!--*(com breve justificativa do vínculo)*-->

<!-- Identificar os Objetivos de Desenvolvimento Sustentável (ODS) relacionados ao software e justificar a conexão -->

<div align="center">
    <img width="100" src="../assets/ods/4.png"/>
    <img width="100"src="../assets/ods/9.png"/>
    <img width="100" src="../assets/ods/10.png"/>
</div>

#### ODS 4 – Educação de Qualidade

O Krita, por ser um software livre e gratuito, democratiza o acesso a ferramentas profissionais de criação digital, permitindo que estudantes, professores e instituições de ensino utilizem recursos avançados sem custos. Isso promove a inclusão educacional, especialmente em áreas como artes digitais, design e animação, favorecendo a aprendizagem criativa e a formação técnica em diferentes contextos.

#### ODS 9 – Indústria, Inovação e Infraestrutura

O desenvolvimento colaborativo e aberto do Krita incentiva a inovação tecnológica e a construção de infraestrutura digital acessível. Sua comunidade global de desenvolvedores e usuários contribui constantemente com melhorias, fortalecendo o ecossistema de software livre e estimulando soluções criativas para diferentes setores, como indústrias criativas, estúdios independentes e startups.

#### ODS 10 – Redução das Desigualdades
Por ser gratuito e de código aberto, o Krita elimina barreiras financeiras que limitam o acesso a softwares profissionais de criação digital. Isso possibilita que artistas de diferentes condições socioeconômicas, regiões e culturas possam desenvolver e compartilhar seu trabalho em igualdade de condições, reduzindo desigualdades no acesso à tecnologia criativa.

---

## 3. Identificação do tipo de produto

### Descrição estruturada do software selecionado para avaliação

<!-- Fornecer uma descrição detalhada e estruturada do software que será avaliado -->

### 3.2. Classificação do tipo de produto

**Nome:** Krita

**Tipo:** Aplicação Desktop Multiplataforma (Qt/C++)

**Repositório:** 
- Principal: https://invent.kde.org/graphics/krita.git (repositório principal KDE)

- Mirror: https://github.com/KDE/krita

**Framework/Backend:**

- **Framework Principal:** Qt Framework (Qt5/Qt6)

- **Linguagem:** C++ (padrão C++17)

- **Sistema de Build:** CMake (versão mínima 3.19.0)

- **Arquitetura:** Plugin-based com bibliotecas modulares

**Plataformas:**

- **Desktop:** Windows, Linux, macOS

- **Mobile:** Android (em desenvolvimento)

- **Distribuição:** AppImage (Linux), instaladores nativos

**Dependências Principais:**

- **Core:** Qt5/6, KDE Frameworks

- **Gráficos:** OpenGL, OpenColorIO (OCIO)

- **Processamento:** Eigen3 (matemática), FFTW3 (transformadas)

- **Formatos:** OpenEXR, LibRaw, OpenJPEG, WebP

- **Python:** PyQt para plugins e scripts

- **Multimídia:** MLT Framework, FFmpeg (para áudio/vídeo)

**Arquitetura Técnica:**

- **SIMD Optimization:** xsimd para processamento vetorial

- **Multi-threading:** Suporte nativo para múltiplos cores

- **Plugin System:** Extensível via plugins C++ e Python

- **Color Management:** Integração com Little CMS e OpenColorIO

- **Brush Engines:** Sistema modular de pincéis personalizáveis

**Características Especiais:**

- **Versão Atual:** 5.3.0-prealpha (branch master)

- **Versão Qt6:** 6.0.0-prealpha (experimental)

- **Licença:** GPL-3.0-only

- **Fundação:** Krita Foundation (organização responsável)

- **Documentação:** https://docs.krita.org/

- **Comunidade:** Krita Artists (https://krita-artists.org/)

---

## 4. Especificação inicial do modelo de qualidade

### Modelo de qualidade com descrição e representação gráfica

<!-- Apresentar o modelo de qualidade que será utilizado, incluindo descrição textual e representação visual -->

### Adaptação do modelo de qualidade
*(refletindo ausência/presença de componentes relevantes ao software avaliado)*

<!-- Explicar como o modelo de qualidade foi adaptado para o software específico sendo avaliado -->

### 3.3. Lista das Características de Qualidade Escolhidas (Método SQUARE)

#### 3.3.1. Adequação Funcional

**Motivação para Escolha:**

A Adequação Funcional foi selecionada para responder diretamente à pergunta central: "Em que medida o Krita atende aos requisitos funcionais em tarefas típicas de pintura digital?". Esta característica permite avaliar:

- **Completude:** Se o Krita oferece todas as funcionalidades necessárias (camadas, pincéis, abertura/salvamento/exportação)

- **Correção:** Se as funcionalidades funcionam conforme especificado

- **Adequação:** Se atende às necessidades do público-alvo (artistas digitais profissionais)

A arquitetura modular do código-fonte (libs/image/, libs/brush/, libs/color/) fornece evidências objetivas para esta avaliação.

#### 3.3.2. Portabilidade

**Motivação para Escolha:**

A Portabilidade foi escolhida para avaliar "o quão bem o Krita se comporta entre plataformas" (Windows, Linux, macOS e Android). As subcaracterísticas avaliadas são:

- **Adaptabilidade:** Funcionamento efetivo em diferentes ambientes

- **Instalabilidade:** Facilidade de instalação em diferentes sistemas

- **Substituibilidade:** Capacidade de substituir outros softwares de pintura digital

#### 3.3.3. Justificativa

Essas características foram priorizadas porque respondem diretamente aos objetivos do trabalho: verificar se o Krita "atende ao que promete" funcionalmente e "se comporta bem entre plataformas", gerando evidências práticas para decisões de uso e melhoria no contexto de pintura digital profissional.

**Critérios de priorização e aplicação:**

- **O propósito e o tipo de produto orientam a seleção das características e o escopo**
- **Relação das características de qualidade priorizadas com o propósito declarado:** Ambas as características escolhidas estão diretamente alinhadas com a pergunta central da avaliação e os objetivos específicos definidos na seção 1.2

## Referências Bibliográficas

<a href="REF1">1.</a> Krita. Krita Foundation [S.l.]. Disponível em: https://krita.org/pt-pt/about/krita-foundation/
. Acesso em: 25 set. 2025.


<a href="REF2">2.</a> Krita. Licença de Utilização 4[S.l.]. Disponível em: https://krita.org/pt-pt/about/license
. Acesso em: 25 set. 2025.

