# 📊 Cofiex Data Insights
### Dashboard e Análise de Projetos COFIEX

---

## 🌍 Visão Geral
Este projeto apresenta uma análise estruturada dos projetos financiados por organismos multilaterais e bilaterais, explorando como os recursos são distribuídos entre setores, regiões e fases do ciclo de aprovação.  
O objetivo é transformar dados públicos em insights claros, apoiando decisões e aumentando a transparência.

---

## 📥 1. Coleta de Dados
A base foi obtida em fontes públicas oficiais sobre financiamentos externos da administração pública federal.

O dataset inclui:  
- Nome e código do projeto  
- Setor e região  
- Fonte financiadora  
- Valores financiados e contrapartidas  
- Fases do projeto (análise, tramitação, assinatura, execução)

**Arquivos:**  
- `dados_2025-02-05.xlsx`  
- `dados_final.csv`

---

## 🧹 2. Limpeza e Preparação dos Dados
Processo realizado em Python (Google Colab) utilizando **pandas**, incluindo:

- Conversão e padronização de datas  
- Remoção de nulos e ajustes estruturais  
- Padronização de colunas  
- Criação de variáveis analíticas:  
  - `dias_ate_assinatura`  
  - `dias_ate_ultimo_desembolso`  
  - `fase_tipo`  
  - `projeto_assinado`  
  - `projeto_multi_fonte`

Dataset final conectado ao Looker Studio.

---

## 🎯 3. Hipóteses Analisadas

- **H1:** Projetos nacionais concentram mais recursos  
- **H2:** Regiões Sudeste e Sul possuem maior volume de propostas  
- **H3:** Projetos com múltiplas fontes levam mais tempo até assinatura  
- **H4:** Setores complexos têm ciclos de aprovação mais longos  

---

## 🔎 4. Análise Exploratória (EDA)

Foram explorados padrões, tendências e relações relevantes, com visualizações no Python e no Looker Studio:

- Distribuição de projetos por região  
- Evolução de projetos recebidos vs. assinados  
- Comparativos financeiros (financiamento x contrapartida)  
- Tempo médio até assinatura  
- Participação por setor  
- Maiores financiamentos  

---

## 📊 5. Dashboard Interativo

Dashboard no Looker Studio organizado em 5 páginas:

1. **Visão Geral**  
2. **Setores e Status**  
3. **Tabela Dinâmica (Filtros)**  
4. **Eficiência e Contrapartidas**  
5. **Principais Insights**

**🔗 Acesse o Dashboard:**  
https://lookerstudio.google.com/reporting/b5e212b4-9d2b-44c1-90cf-665ba42feb4a

---

## ❓ 6. Principais Perguntas Respondidas

**• Quais setores concentram os maiores investimentos?**  
Infraestrutura, Energia, Desenvolvimento Social e Transportes.

**• Quanto tempo um projeto leva até ser assinado?**  
Cerca de **10 anos**, indicando um ciclo longo e burocrático.

**• Projetos multi-fonte são mais lentos?**  
Sim, apresentam ciclos maiores.

**• Quais regiões apresentam mais projetos?**  
Nacional e Sudeste lideram o volume.

---

## 💡 7. Principais Insights

- Projetos nacionais representam quase metade do volume financeiro.  
- O ciclo de aprovação é longo: média de **10 anos**.  
- Contrapartidas equivalem a **33,3%** dos valores totais.  
- A partir de 2018 houve aumento nas assinaturas.  
- Infraestrutura e Energia concentram os maiores valores.  

---

## ⚠️ 8. Limitações dos Dados

- Datas ausentes ou incompletas em alguns registros  
- Diferenças entre anos e versões das bases oficiais  
- Possível defasagem em atualizações  
- Ausência de dados de execução física  

Essas limitações foram consideradas na análise.

---

## 🚀 9. Próximos Passos (Possíveis Extensões)

- Previsão do tempo de assinatura  
- Clusterização por características (setor, fonte, região)  
- Análise financeira aprofundada de contrapartidas  
- Integração com séries históricas de execução orçamentária  

---

## 🛠 Tecnologias Utilizadas

- Python (pandas, numpy, matplotlib)  
- Google Colab  
- Google Sheets  
- Looker Studio  
- GitHub  

---

## 📁 Estrutura do Projeto

Projeto-COFIEX
│
├── data
│ ├── dados_2025-02-05.xlsx
│ └── dados_final.csv
│
├── notebook
│ └── analise_cofiex.ipynb
│
├── dashboard
│ └── link_looker_studio.txt
│
├── README.md
└── relatorio_insights.pdf


---

## 🏁 Conclusão

O projeto demonstra como a análise de dados pode aprimorar a gestão pública, oferecendo transparência e suporte à tomada de decisões sobre financiamentos internacionais.  
As visualizações destacam gargalos, tendências e oportunidades de melhoria no processo de aprovação.


