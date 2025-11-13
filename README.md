Cofiex Data Insights – Dashboard e Análise de Projetos COFIEX

Análise dos projetos e programas do setor público brasileiro com financiamento externo, sob coordenação da Comissão de Financiamentos Externos (COFIEX).

Visão Geral

Este projeto apresenta uma análise estruturada dos projetos financiados por organismos multilaterais e bilaterais, explorando como os recursos são distribuídos entre setores, regiões e fases do ciclo de aprovação.
O objetivo é transformar dados públicos em insights claros, que apoiem decisões e aumentem a transparência.

1. Coleta de Dados

A base foi obtida a partir de fontes públicas oficiais sobre financiamentos externos da administração pública federal.

O dataset inclui:

Nome e código do projeto

Setor e região

Fonte financiadora

Valor financiado e contrapartida

Fases do projeto (análise, tramitação, assinatura, execução)

Arquivos:
• dados_2025-02-05.xlsx
• dados_final.csv

2. Limpeza e Preparação dos Dados

Processo realizado em Python (Google Colab) com pandas, incluindo:

Conversão e padronização de datas

Remoção de nulos e inconsistências

Normalização de colunas

Criação de novas variáveis analíticas:

dias_ate_assinatura

dias_ate_ultimo_desembolso

fase_tipo

projeto_assinado

projeto_multi_fonte

A versão final foi exportada e conectada ao Looker Studio.

3. Hipóteses Avaliadas

Para guiar a EDA, foram consideradas hipóteses simples, coerentes com o contexto:

H1: Projetos nacionais recebem mais recursos.

H2: Regiões Sul e Sudeste concentram mais propostas aprovadas.

H3: Projetos com múltiplas fontes de financiamento levam mais tempo para serem assinados.

H4: Setores de grande complexidade (infraestrutura, energia) possuem ciclos de aprovação mais longos.

Essas hipóteses ajudaram a direcionar perguntas e validações ao longo da análise.

4. Análise Exploratória (EDA)

A EDA explorou padrões, tendências e relações importantes.

Entre as visualizações e métricas criadas no Python e no Looker Studio estão:

Distribuição de projetos por região

Evolução de projetos recebidos vs. assinados

Comparativo financeiro (financiado vs contrapartida)

Tempo médio até assinatura

Participação e desempenho de setores

Identificação dos maiores financiamentos

5. Dashboard Interativo (Looker Studio)

Organizado em 5 páginas temáticas:

Visão Geral – indicadores principais e evolução

Setores e Status – comparativos e fases

Tabela Dinâmica – consulta detalhada com filtros

Eficiência e Contrapartidas – tempos médios e proporções

Insights – principais achados e conclusões

Link: (https://lookerstudio.google.com/reporting/b5e212b4-9d2b-44c1-90cf-665ba42feb4a
)

6. Perguntas de Negócio Respondidas

Algumas das principais perguntas analisadas:

• Quais setores concentram os maiores investimentos?
Infraestrutura, Energia, Desenvolvimento Social e Transportes.

• Quanto tempo um projeto leva, em média, para ser assinado?
Aproximadamente 10 anos, indicando um ciclo altamente burocrático.

• De onde vêm os maiores financiamentos?
Principalmente de organismos multilaterais, com destaque para bancos internacionais.

• Quais regiões possuem maior quantidade de projetos?
Predomínio de projetos nacionais e forte concentração no Sudeste.

• Projetos multi-fonte são mais lentos?
Sim. Geralmente apresentam tempos maiores de tramitação.

7. Principais Insights

Projetos nacionais representam quase metade do volume financeiro total.

O ciclo de aprovação é longo: cerca de 10 anos entre recebimento e assinatura.

Contrapartidas representam, em média, 33,3% dos valores totais.

Houve crescimento no número de assinaturas após 2018.

Setores estratégicos absorvem os maiores valores de financiamento.

8. Limitações dos Dados

Transparência é importante, e algumas limitações foram observadas:

Ausência de datas completas para todos os projetos

Diferenças no padrão das fases entre períodos diferentes

Possíveis atrasos na atualização das bases oficiais

Falta de informações sobre execução física dos projetos

Essas limitações foram consideradas na interpretação dos resultados.

9. Possíveis Próximos Passos

Ideias para evoluir o projeto futuramente:

Comparar valores aprovados vs valores efetivamente desembolsados

Criar um modelo simples de previsão do tempo de assinatura

Clusterizar projetos por características semelhantes

Integrar outras bases de dados de investimentos públicos

Tecnologias Utilizadas

Python (pandas, numpy, matplotlib)

Google Colab

Looker Studio

Google Sheets

GitHub

Estrutura de Pastas
Projeto-COFIEX
│
├── data
│   ├── dados_2025-02-05.xlsx
│   └── dados_final.csv
│
├── notebook
│   └── analise_cofiex.ipynb
│
├── dashboard
│   └── link_looker_studio.txt
│
├── README.md
└── relatorio_insights.pdf

Conclusão

O projeto demonstra como a análise de dados pode apoiar a gestão pública por meio de indicadores, visualizações e métricas de eficiência.
Os insights permitem identificar gargalos, tendências e oportunidades de melhoria no processo de aprovação de financiamentos internacionais.

