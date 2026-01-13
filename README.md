<p align="center">
  <img src="https://img.shields.io/badge/Status-Concluído-brightgreen?style=flat-square">
  <img src="https://img.shields.io/badge/IA-Integrada-007acc?style=flat-square">
  <img src="https://img.shields.io/badge/CX-Inteligência_Ativa-f57c00?style=flat-square">
  <img src="https://img.shields.io/badge/PNL-Natural_Language_Processing-6a1b9a?style=flat-square">
</p>

# NLP Insights & CX Intelligence | Inteligência Artificial e PNL

## 🚀 Resultados e Impacto

Este projeto gerou ganhos concretos para a operação:

- 📈 **Recuperação de NPS**: O projeto provocou uma gestão real time de indicadores de satisfação ajudando o NPS sair de 35,77 em Julho/2025 para 61,32 em Setembro/2025
- ⚙️ **Automação de relatórios**: De semanal (terça-feira) para **Atualização diária**
- 🧠 **Adoção de IA** para detecção de padrões e alavancas de resultado
- 🔍 **Mapeamento automático de causa raiz** colaborando em melhoria contínua de jornada (antes manual)
- 🛡️ **Identificação preventiva** de situações de alto attrition capturadas pelo código

---

## 📊 Demonstração do Projeto

<table>
  <tr>
    <td><b>Página 1: Insights e Causa Raiz</b></td>
    <td><b>Página 2: IA e Propensão de Attrition</b></td>
  </tr>
  <tr>
    <td><img src="https://i.postimg.cc/YqYYGJGL/P-gina-1-Insights-geral.gif" width="100%"></td>
    <td><img src="https://i.postimg.cc/P5MDKYQz/P-gina-2-IA-e-Ant-atriction.gif" width="100%"></td>
  </tr>
  <tr>
    <td><b>Página 3: Análise de Volumetria</b></td>
    <td><b>Página 4: PNL Isolada</b></td>
  </tr>
  <tr>
    <td><img src="https://i.postimg.cc/HLsyNnSc/P-gina-3-Volumetria.gif" width="100%"></td>
    <td><img src="https://i.postimg.cc/t49Z17GW/P-gina-4-PNL-isolada.gif" width="100%"></td>
  </tr>
</table>

---

## 📌 Visão Geral

Este projeto integra dados de CRM próprio com metodologias avançadas de PNL e Inteligência Artificial. Utiliza um simulador de GPT e algoritmos de captura de strings via Speech e Text Analytics para transformar conversas brutas em insights acionáveis de experiência do cliente.

> **Nota de Confidencialidade:** Devido a políticas de LGPD, dados sensíveis e nomes de colunas reais foram omitidos ou mascarados. O foco deste repositório é demonstrar a arquitetura da solução e os resultados de negócio obtidos.

---

## 🧩 Arquitetura da Solução

A solução foi construída em camadas, desde a captura de dados brutos até a geração de ações preventivas em tempo real.

### 🔹 Camada 1 – Fontes de Dados

- **CRM próprio**
- **Speech Analytics** (áudio → texto)
- **Text Analytics** (texto de pesquisas, comentários, chats)

Essas fontes alimentam o pipeline com conversas e feedbacks brutos de clientes.

---

### 🔹 Camada 2 – Pipeline de IA & PNL

- **Ingestão & limpeza de texto**
- **Detecção de expressões chave e geração de WordCloud**
- **Pareto de motivos de reclamação**
- **Classificação de temas** (Processos, Pessoas, Negócio)
- **Cálculo de volumetria por canal, local e equipe**
- **Identificação de menções críticas e risco de attrition**

Aqui entram as regras de negócio, NLP e lógica de categorização que transformam texto em dados estruturados.

---

### 🔹 Camada 3 – Camada Analítica (Notebook)

- **Notebook principal:** `notebooks/pipeline_insights_cx.ipynb`
- Criação e tratamento de:
  - `Fato_Pesquisas`
  - `Fato_Respostas`
  - Tabelas de parâmetros de filtro
  - Tabelas de suporte estatístico (ex.: desvio padrão)

Essa camada consolida a saída do pipeline de IA & PNL e prepara o modelo tabular para consumo no BI.

---

### 🔹 Camada 4 – Modelo BI & DAX

- **Ferramenta:** Power BI
- **Lógica de negócio implementada via DAX**, incluindo:
  - Métricas de volumetria por canal
  - Propensão de attrition por tema, canal, local e equipe
  - NPS, rankings e paretos de motivos
  - Indicadores de produção e performance (carga, tempo de atualização, capacity)

Detalhes adicionais de métricas estão documentados em:
- `metrics/tabela_metricas_dax.md`
- `metrics/indicadores_utilizados.md`
- `metrics/exemplos_dax.txt`

---

### 🔹 Camada 5 – Camada de Consumo (Dashboards & IA)

- **Páginas do dashboard:**
  - Página 1: Insights & Causa Raiz
  - Página 2: IA & Propensão de Attrition
  - Página 3: Volumetria & Estatística
  - Página 4: PNL Isolada
- **Chat com IA** para:
  - Consultar volumetria
  - Gerar cenários
  - Tirar dúvidas sobre resultados
  - Sugerir ações

Essa camada conecta usuários de negócio diretamente aos insights gerados pela solução.

---

### 🔹 Camada 6 – Impacto e Ações

- **Recuperação de NPS** de 35,77 para 61,32 em 2 meses
- **Automação de relatórios**: de semanal para diário
- **Mapeamento automático de causa raiz** e motivos prioritários
- **Identificação preventiva de casos de alto attrition**

Essa arquitetura fecha o ciclo completo: dado bruto → inteligência de IA/PNL → decisão → resultado de negócio.

## 🛠️ Ferramentas Utilizadas

* **IA & NLP:** Speech/Text Analytics para captura de strings e análise de sentimento  
* **UX/UI Design:** Figma para prototipação de alta fidelidade  
* **Arquitetura:** SQL para manipulação e Discovery de Dados  
* **BI:** Power BI e DAX avançado para simulação de cenários  
* **Metodologia:** SCRUM, Lean Six Sigma (LSS) e Discovery de Negócios (Confluence)

---

## 📂 Estrutura do Repositório

* `/metrics`: Fórmulas DAX e lógica de predição de attrition  
* `/Notebooks`: Pipiline do projeto (camada final)
* `/results`: Resultados consolidados de reversão de KPIs
* `/visuals`: Capturas da interface e fluxos de NLP 
* `/documentation`: README, LICENSE 

---

## 👤 Autor

**Jessé Oliveira de Castro**  
* <a href="https://www.linkedin.com/in/jesse-oliveira-de-castro-88421536/" target="_blank">LinkedIn Profissional</a>  
* <a href="https://portfolio-jesseoliveiracastro.netlify.app/" target="_blank">Portfólio Profissional</a>
