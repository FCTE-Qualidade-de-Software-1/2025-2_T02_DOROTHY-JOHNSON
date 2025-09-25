# Execução da Fase 1 - Avaliação de Software

## 1. Propósito da avaliação

### Requisitante e partes interessadas
<!-- *(comprador, fornecedor, desenvolvedor, operador, etc.)* -->

<!-- Descrever aqui quem está solicitando a avaliação e todas as partes interessadas envolvidas no processo -->

O requisitante principal do Krita é a comunidade de usuários finais, composta por artistas digitais, ilustradores, quadrinistas, animadores e designers que buscam uma solução acessível e completa para criação de artes digitais [[1]](#REF1). A demanda por melhorias e novas funcionalidades parte majoritariamente desses usuários, por meio de fóruns, enquetes, relatórios de erros e sugestões de recursos.

As partes interessadas envolvidas no processo também incluem [[1]](#REF1) [[2]](#REF2):

- Os desenvolvedores voluntários e colaboradores, responsáveis pela implementação de recursos, correções de falhas e manutenção do código aberto;

- Mantenedores do projeto, que coordenam a evolução do software, definem prioridades e integram as contribuições enviadas;

- Testadores e demais membros da comunidade que validam versões, reportam problemas e sugerem ajustes;

- Distribuidores e mantenedores de pacotes, como repositórios Linux e lojas de aplicativos, que asseguram que o software esteja acessível e atualizado em diferentes plataformas;

- A poiadores financeiros, como doadores, patrocinadores e iniciativas de financiamento coletivo;

- Os operadores, em que se destacam-se artistas, estúdios independentes e instituições de ensino, que utilizam o Krita em seus fluxos de trabalho e ajudam na sua difusão.


### Propósito da avaliação e uso pretendido dos resultados

<!-- Explicar o objetivo da avaliação e como os resultados serão utilizados -->

### Escopo, profundidade e objetos de avaliação
*(incluindo relação com avaliações anteriores ou futuras, quando aplicável)*

<!-- Definir o escopo da avaliação, qual será a profundidade da análise e quais objetos serão avaliados -->

### ODS relacionados e metas associadas ao software
*(com breve justificativa do vínculo)*

<!-- Identificar os Objetivos de Desenvolvimento Sustentável (ODS) relacionados ao software e justificar a conexão -->

---

## 2. Identificação do tipo de produto

### Descrição estruturada do software selecionado para avaliação

<!-- Fornecer uma descrição detalhada e estruturada do software que será avaliado -->

### 2.2. Classificação do tipo de produto

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

## 3. Especificação inicial do modelo de qualidade

### Modelo de qualidade com descrição e representação gráfica

<!-- Apresentar o modelo de qualidade que será utilizado, incluindo descrição textual e representação visual -->

### Adaptação do modelo de qualidade
*(refletindo ausência/presença de componentes relevantes ao software avaliado)*

<!-- Explicar como o modelo de qualidade foi adaptado para o software específico sendo avaliado -->

### Lista das características escolhidas (exceto usabilidade)
*(com critérios de priorização adotados e sua aplicação)*

<!-- Listar as características de qualidade selecionadas e explicar os critérios de priorização -->

#### Critérios de priorização e aplicação

- **O propósito e o tipo de produto devem orientar a seleção das características e o escopo**
- **Relação das características de qualidade priorizadas com o propósito declarado**

<!-- Explicar como as características escolhidas se relacionam com o propósito da avaliação -->

## Referências Bibliográficas

<a href="REF1">1.</a> Krita. Krita Foundation [S.l.]. Disponível em: https://krita.org/pt-pt/about/krita-foundation/
. Acesso em: 25 set. 2025.


<a href="REF2">2.</a> Krita. Licença de Utilização 4[S.l.]. Disponível em: https://krita.org/pt-pt/about/license
. Acesso em: 25 set. 2025.

