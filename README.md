# ⚽ Perfil Estatístico dos Jogadores da Seleção Brasileira (Ciclo Copa 2026)

Este projeto apresenta uma **Análise Exploratória de Dados (AED)** detalhada sobre o desempenho dos jogadores cotados para representar o Brasil na Copa do Mundo de 2026. O objetivo é identificar, através de métodos estatísticos, os padrões que definem um jogador de nível de seleção nacional em diferentes posições.

## 📋 Sobre o Projeto

Desenvolvido para a disciplina de Estatística, o projeto utiliza Python para processar dados de desempenho e aplicar conceitos de centralização, dispersão e correlação. A análise busca separar o perfil de "veteranos" de "promessas" e entender a eficiência defensiva e ofensiva do elenco.

### Objetivos Principais:
- Analisar medidas de centralização (média, mediana) e dispersão (desvio padrão) de idade e experiência.
- Aplicar o **Coeficiente de Correlação de Pearson** para validar hipóteses sobre o setor defensivo.
- Estabelecer critérios matemáticos para classificar a senioridade dos atletas.

## 📊 Metodologia Estatística

### 1. Definição de Jogadores Experientes
Como a média de jogos na seleção varia drasticamente entre as posições, não utilizamos um número fixo. Adotamos o critério de **quantis**:
- **Zagueiros e Atacantes:** Considerados experientes os que estão no **Top 20%** (percentil 80).
- **Meio-Campistas e Goleiros:** Considerados experientes os que estão no **Top 10%** (percentil 90).

### 2. Análise de Correlação (Zagueiros)
O projeto investiga a relação entre a agressividade defensiva e a disciplina. 
- **Variável X:** Ações Defensivas Ativas (Soma de Interceptações + Divididas).
- **Variável Y:** Quantidade de Faltas Cometidas.
- **Ferramenta:** Coeficiente de Pearson e Linha de Regressão (Tendência) para verificar se uma maior atividade defensiva resulta obrigatoriamente em mais faltas.

## 🛠️ Tecnologias Utilizadas

- **Python 3.x**
- **Pandas & NumPy:** Processamento de dados e cálculos estatísticos.
- **Matplotlib & Seaborn:** Geração de histogramas, boxplots e gráficos de dispersão.
- **Jupyter Notebook:** Documentação e execução do fluxo de análise.

## 📂 Estrutura dos Dados

Os dados estão organizados por setor para permitir análises específicas:
- **Goleiros:** Jogos sem sofrer gols (*clean sheets*) e defesas por partida.
- **Zagueiros:** Interceptações, divididas, ações defensivas totais e faltas.
- **Meio-Campo:** Assistências, cruzamentos e transição defensiva.
- **Atacantes:** Gols (clube e seleção), dribles certos e conversão de pênaltis.
- **Geral (Todos):** Dados demográficos como idade, clube e lateralidade (pé preferido).

## 🚀 Como Executar

1. Clone o repositório.
2. Certifique-se de ter os arquivos CSV ou o `Dataset.xlsx` na raiz do projeto.
3. Instale as bibliotecas:
   ```bash
   pip install pandas numpy matplotlib seaborn openpyxl
