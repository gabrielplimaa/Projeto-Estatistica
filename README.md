# ⚽ Perfil Estatístico dos Jogadores da Seleção Brasileira (Ciclo Copa 2026)

Este projeto apresenta uma **Análise Exploratória de Dados (AED)** detalhada sobre o desempenho dos jogadores cotados para representar o Brasil na Copa do Mundo de 2026. O objetivo é identificar, através de métodos estatísticos, os padrões que definem um jogador de nível de seleção nacional em diferentes posições.

## 👥 Autores 
* **Ivan Pinto da Rocha Filho** 
* **Mateus Dornellas Camara de Freitas** 
* **João Pedro Patriota de Carvalho** 
* **Arthur Queiroz Silva**
* **Gabriel Pereira Lima**
* **Pedro de Melo Dhalia**
* **Arthur Xavier Rego Monteiro**
* **Guilherme Cireno Baltar**
* **Caio Augusto Machado de Melo**

## 📋 Sobre o Projeto
Desenvolvido para a disciplina de **Estatística**, o projeto utiliza Python para processar dados de desempenho e aplicar conceitos de centralização, dispersão e correlação. A análise busca separar o perfil de "veteranos" de "promessas" e entender a eficiência defensiva e ofensiva do elenco atual.

### Objetivos Principais:
* Analisar medidas de centralização (média, mediana) e dispersão (desvio padrão) de idade e experiência.
* Aplicar o **Coeficiente de Correlação de Pearson** para validar hipóteses sobre o setor defensivo.
* Estabelecer critérios matemáticos (percentis) para classificar a senioridade dos atletas.

## 📊 Metodologia Estatística

### 1. Definição de Jogadores Experientes
Como a média de jogos na seleção varia drasticamente entre as posições, adotamos o critério de **quantis** para evitar distorções:
* **Zagueiros e Atacantes:** Considerados experientes os que estão no **Top 20%** (percentil 80).
* **Meio-Campistas e Goleiros:** Considerados experientes os que estão no **Top 10%** (percentil 90).

### 2. Análise de Correlação (Zagueiros)
O projeto investiga a relação entre a agressividade defensiva e a disciplina:
* **Variável X:** Ações Defensivas Ativas (Soma de Interceptações + Divididas).
* **Variável Y:** Quantidade de Faltas Cometidas.
* **Ferramenta:** Coeficiente de Pearson e Linha de Regressão para verificar se uma maior atividade defensiva resulta em um aumento proporcional de faltas.

## 🛠️ Tecnologias Utilizadas
* **Python 3.x**
* **Pandas & NumPy:** Processamento de dados e cálculos.
* **Matplotlib & Seaborn:** Geração de histogramas, boxplots e gráficos de dispersão.

## 📂 Estrutura dos Dados
A base de dados foi dividida em setores para análises específicas:
* **Goleiros:** Clean sheets e defesas por partida.
* **Zagueiros:** Interceptações, divididas e faltas.
* **Meio-Campo:** Assistências, cruzamentos e transição.
* **Atacantes:** Gols, dribles e conversão de pênaltis.

## 🚀 Como Executar
1. Clone o repositório.
2. Certifique-se de ter os arquivos CSV ou o `Dataset.xlsx` na raiz do projeto.
3. Instale as bibliotecas necessárias:
   ```bash
   pip install pandas numpy matplotlib seaborn openpyxl
