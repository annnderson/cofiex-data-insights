# cofiex-data-insights
Dashboard e análise de projetos COFIEX

# 🌍 Cofiex Data Insights – Análise de Projetos e Financiamentos Internacionais

## 🧭 Visão Geral  
Este projeto apresenta uma análise detalhada dos **projetos e programas do setor público brasileiro** que contam com **financiamento externo** de organismos **multilaterais e bilaterais**, sob a coordenação da **Comissão de Financiamentos Externos (COFIEX)**.  

O objetivo é compreender como os recursos são distribuídos entre setores, regiões e fases do ciclo de projeto — desde a análise até a execução —, utilizando **dados públicos** e **ferramentas de Business Intelligence** para transformar informações em insights estratégicos.  

---

🔗 [Acessar a fonte oficial dos dados](https://dados.gov.br/dados/conjuntos-dados/cofiex)

## 🧩 Estrutura do Projeto  

### 1️⃣  Coleta de Dados  
A base foi obtida a partir de **fontes públicas oficiais** sobre financiamentos externos da administração pública federal.  
O dataset inclui informações como:  
- Nome e código do projeto;  
- Setor e região de atuação;  
- Fonte financiadora;  
- Valor do financiamento e contrapartida;  
- Fases do projeto (análise, tramitação, assinatura e execução).  


📁 **Arquivo principal:** `dados_2025-02-05.xlsx`  
📄 **Versão final tratada:** `dados_final.csv`  

---

### 2️⃣  Limpeza e Preparação dos Dados  
Realizada em **Python (Google Colab)** com uso da biblioteca **pandas**, incluindo:  
- Conversão de datas e formatação no padrão brasileiro;  
- Padronização de colunas e remoção de valores nulos;  
- Criação de novas variáveis como:  
  - `dias_ate_assinatura`  
  - `dias_ate_ultimo_desembolso`  
  - `fase_tipo`  
  - `projeto_assinado`  
  - `projeto_multi_fonte`  

O arquivo final foi exportado para o **Google Drive** e integrado ao **Looker Studio** para visualização interativa.  

---

### 3️⃣  Análise Exploratória de Dados (EDA)  
A EDA teve como foco entender **padrões, correlações e distribuição de investimentos**.  
Foram criadas diferentes análises e visualizações:  

- **Distribuição de projetos por região e setor**  
- **Evolução de projetos recebidos vs. assinados por ano**  
- **Comparativo financeiro entre valores financiados e contrapartidas**  
- **Tempo médio até assinatura (eficiência administrativa)**  
- **Top setores e projetos com maiores financiamentos**  

---

### 4️⃣  Dashboard no Looker Studio  
O dashboard foi estruturado em **5 páginas interativas**, cada uma com um propósito analítico:  

#### 📌 Página 1 – *Análise Geral de Projetos e Financiamentos*  
Visão macro com indicadores principais, evolução temporal e distribuição por região.  

#### 📌 Página 2 – *Setores e Status dos Projetos*  
Análise comparativa por setor e fase dos projetos.  

#### 📌 Página 3 – *Análise Detalhada (Tabela Dinâmica)*  
Consulta interativa com filtros de **Setor, Região e Fase Tipo**, exibindo valores e detalhes de cada projeto.  

#### 📌 Página 4 – *Eficiência e Contrapartidas*  
Tempo médio até assinatura e proporção das contrapartidas em relação ao total financiado.  

#### 📌 Página 5 – *Conclusões e Principais Insights*  
Resumo visual com **métricas, top setores e média de investimentos**.  

---

## 💡 Principais Insights  

- **Projetos Nacionais representam quase metade do total de investimentos.**  
- O tempo médio entre recebimento e assinatura é de aproximadamente **10 anos**, evidenciando um longo ciclo de aprovação.  
- **Setores com maior financiamento:** Infraestrutura, Energia, Desenvolvimento Social e Transportes.  
- **Contrapartida média:** 33,3% do valor total dos projetos, indicando esforço conjunto entre governo e organismos financiadores.  
- **Crescimento contínuo** de assinaturas nos últimos anos, especialmente após 2018.  

---

## 🛠️ Tecnologias Utilizadas  
- **Python (pandas, numpy, matplotlib)** – Limpeza e EDA  
- **Google Colab** – Ambiente de análise  
- **Google Sheets** – Ajustes e exportação  
- **Looker Studio** – Visualização e dashboard  
- **GitHub** – Documentação e entrega final  

---

## 🧾 Estrutura de Pastas
📁 Projeto-COFIEX
┣ 📂 data
┃ ┣ dados_2025-02-05.xlsx
┃ ┗ dados_final.csv
┣ 📂 notebook
┃ ┗ analise_cofiex.ipynb
┣ 📂 dashboard
┃ ┗ link_looker_studio.txt
┣ 📄 README.md
┗ 📄 relatorio_insights.pdf


---

## 👤 Autor  
**Anderson Rodrigues dos Santos**  
📍 Taboão da Serra – SP  
📧 andersonr.create@gmail.com  
🔗 [Github](https://github.com/annnderson) 

---

## 📊 Link do Dashboard  
🔗 *(https://lookerstudio.google.com/reporting/b5e212b4-9d2b-44c1-90cf-665ba42feb4a)*  

---

## 🏁 Conclusão  
O projeto demonstra como a **análise de dados pode aprimorar a gestão pública**, oferecendo transparência e suporte à tomada de decisões estratégicas sobre **financiamentos internacionais**.  
As visualizações no Looker Studio permitiram identificar gargalos, tendências e oportunidades de melhoria no processo de execução e aprovação de projetos.  

---

🧠 *"Dados bem analisados transformam complexidade em clareza."*  


