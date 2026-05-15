# 📈 analise-acoes-brasileiras

> Análise comparativa do desempenho histórico de ações da B3 no período de Janeiro/2023 a Maio/2026.

---

## 📋 Sobre o Projeto

Este projeto realiza uma **análise financeira exploratória** de cinco importantes empresas brasileiras listadas na B3, utilizando dados históricos obtidos via `yfinance`. O notebook inclui um código de referência baseado na Petrobrás (PETR4) e estende a análise para mais quatro empresas do índice Ibovespa.

---

## 🏢 Empresas Analisadas

| Empresa         | Ticker (Yahoo Finance) | Setor              |
|-----------------|------------------------|--------------------|
| Petrobrás       | `PETR4.SA`             | Energia / Petróleo |
| Vale S.A.       | `VALE3.SA`             | Mineração          |
| Ambev S.A.      | `ABEV3.SA`             | Bebidas            |
| Itaú Unibanco   | `ITUB4.SA`             | Bancos             |
| Banco do Brasil | `BBAS3.SA`             | Bancos             |

---

## 🔍 Análises Realizadas

Para cada empresa, o notebook executa as seguintes etapas:

1. **Download dos dados históricos** via `yfinance` (Jan/2023 – Mai/2026)
2. **Inspeção inicial** — 5 primeiras e 5 últimas linhas do DataFrame
3. **Média anual** do preço de fechamento (por ano do período)
4. **Desvio-padrão anual** do preço de fechamento
5. **Retorno semestral** — variação percentual entre semestres consecutivos
6. **Gráfico de linha** do preço de fechamento com eixo X rotulado por semestre
7. **Tabela resumo semestral** com abertura, fechamento, média, desvio-padrão, mínimo, máximo e retorno

---

## 🛠️ Tecnologias Utilizadas

- **Python 3.x**
- [`yfinance`](https://github.com/ranaroussi/yfinance) — coleta de dados históricos de ações
- [`pandas`](https://pandas.pydata.org/) — manipulação e análise de dados
- [`matplotlib`](https://matplotlib.org/) — visualização de dados
- [`seaborn`](https://seaborn.pydata.org/) — estilização dos gráficos

---

## 🚀 Como Executar

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/analise-acoes-brasileiras.git
cd analise-acoes-brasileiras
```

### 2. Instale as dependências

```bash
pip install yfinance pandas matplotlib seaborn notebook
```

### 3. Abra o notebook

```bash
jupyter notebook Atividade_ANÁLISE_COMPARATIVA_DE_AÇÕES_BRASILEIRAS_.ipynb
```

> **Alternativa:** você também pode abrir o notebook no [Google Colab](https://colab.research.google.com/) e executar as células diretamente — todas as dependências são instaladas automaticamente via `!pip install`.

---

## 📁 Estrutura do Repositório

```
analise-acoes-brasileiras/
│
├── Atividade_ANÁLISE_COMPARATIVA_DE_AÇÕES_BRASILEIRAS_.ipynb   # Notebook principal
└── README.md                                                    # Este arquivo
```

---

## 📊 Exemplo de Saída

O notebook gera gráficos como o abaixo para cada ativo, com destaque nos fechamentos semestrais:

```
PETROBRÁS (PETR4.SA) - Preço de Fechamento (Jan/2023 a Mai/2026)
Eixo X: 2023-S1 | 2023-S2 | 2024-S1 | 2024-S2 | 2025-S1 | 2025-S2 | 2026-S1
```

Além de tabelas de resumo no formato:

```
 Ano | Semestre | Abertura | Fechamento | Média  | Desvio | Mínimo | Máximo | Retorno_%
2023 |    S1    |  R$28.xx |   R$30.xx  | R$29.xx| R$1.xx | R$26.xx| R$33.xx|  +7.xx%
```

---

## 📝 Observações

- Os dados são obtidos em tempo real via API do Yahoo Finance — resultados podem variar conforme a data de execução.
- O ano de 2026 contém dados parciais (até 14/05/2026).
- Os preços estão expressos em **Reais (R$)**.

---

## 📄 Licença

Este projeto foi desenvolvido para fins **educacionais**. Sinta-se livre para utilizar, adaptar e compartilhar.
