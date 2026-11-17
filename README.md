##  ObservatórioRemuneraSP

## Dinâmicas Remuneratórias no Setor Público: uma análise em Ciência de Dados das assimetrias salariais no Estado de São Paulo

---

**Sobre o Projeto**

  Criação e adição do Projeto Integrador num site, para aquisição de métricas e dados, com isso o projeto contempla uma boa parte do artigo em desenvolvimento e um pouco mais. A respeito do trabalho: Estudo quantitativo de abordagem descritivo-comparativa desenvolvido na **Fatec Rubens Lara (Santos/SP)**, com o objetivo de investigar simetrias e assimetrias salariais entre servidores públicos ativos, aposentados e pensionistas do Estado de São Paulo, utilizando dados abertos do Portal da Transparência referentes ao período de **junho de 2023 a junho de 2026** (37 competências mensais, totalizando mais de 8 GB em arquivos brutos).

*Aviso: Este projeto possui finalidade exclusivamente educacional e acadêmica, não representando órgão governamental ou serviço oficial.*

---

<!--

## Arquitetura e Pipeline de Dados (ETL)

Para processar e consolidar dezenas de milhões de registros sem perda de desempenho, foi estruturado o seguinte fluxo de engenharia e análise de dados:

1. **Extração (Extract):** Coleta das 37 bases mensais (`2023_06` a `2026_06`) no Portal da Transparência do Estado de São Paulo.
2. **Pré-tratamento e Padronização (Transform):**
   * Inspeção inicial e agrupamento de **75 órgãos** em grandes setores administrativos via **Microsoft Excel** e **LibreOffice Calc**.
   * Limpeza de colunas, remoção de duplicidades e conversão de arquivos `.txt`/`.csv` para o formato colunar compactado **Parquet** via **ExploreMyData**.
3. **Consolidação em Larga Escala (Load):**
   * Unificação de toda a série histórica via **DuckDB** e **SQL** (`read_parquet` com `union_by_name=true` e extração automática de `MES_COMPETENCIA` via expressão regular), gerando uma base única consolidada (`Remuneracao_Consolidada_Com_Mes.parquet`).
4. **Visualização e Análise Exploratória:** Modelagem analítica e construção de dashboards interativos no **Microsoft Power BI Desktop**.

---

## Principais Achados (Jun/2023 – Jun/2026)

* **Simetria entre grupos vs. Assimetria interna:** A média salarial líquida entre **ativos** (R$ 5,97 mil) e **aposentados** (R$ 5,58 mil) difere em apenas R$ 390. As grandes disparidades ocorrem internamente entre cargos e carreiras (variando de R$ 0 a mais de R$ 100 mil).
* **Retração do quadro ativo e razão previdenciária:** O número de servidores ativos caiu **8,8%** no período (de 548 mil para 500 mil), enquanto aposentados e pensionistas se mantiveram estáveis (~528 mil). A razão passou de 96 para **106 inativos para cada 100 ativos**.
* **Sazonalidade na Educação:** A Secretaria da Educação concentra a maior parte da retração de ativos, com quedas recorrentes nos meses de janeiro (como a redução de 45,7 mil vínculos entre dez/2023 e jan/2024) seguidas de reposição parcial a partir de março.
* **Efeito Coorte (Gerações de Ingresso):** Embora as gerações ingressantes entre 2000 e 2025 superem numericamente as antigas, a remuneração média de entrada caiu de **R$ 11 mil – R$ 17,5 mil** (coortes dos anos 1970) para menos de **R$ 4 mil** nos ingressos de 2025–2026.
* **Impacto do Teto Constitucional:** O volume de registros sujeitos ao redutor salarial (abate-teto) cresceu continuamente no período, concentrado principalmente no setor de Previdência e Benefícios (avançando de ~7 mil para 11,5 mil registros mensais).

---

-->

## Autores

* **Amanda da Silva Gonçalves(@M1T0K0)** — Fatec Rubens Lara
* **Gustavo Franco Mendonça Vasques(@Fr4nco0-0)** — Fatec Rubens Lara 
* **Yuki Paschoal Spinola Pencov** — Fatec Rubens Lara

---

## Ferramentas

`Google Sites`

## Link para o site
https://fr4nco0-0.github.io/ObservatorioRemuneraSP/
