# Execução da Fase 1 - Avaliação de Software

## 1. Propósito da avaliação

### Requisitante e partes interessadas
*(comprador, fornecedor, desenvolvedor, operador, etc.)*

<!-- Descrever aqui quem está solicitando a avaliação e todas as partes interessadas envolvidas no processo -->

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
