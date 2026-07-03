# 📊 Análise de Transações Financeiras

Projeto desenvolvido para a disciplina de Programação em Python, com o objetivo de realizar a leitura, validação, processamento e análise de transações financeiras a partir de um arquivo CSV.

Além do processamento dos dados, o projeto gera um relatório em JSON e uma visualização gráfica utilizando Matplotlib.

---

## 📌 Objetivos

O sistema é capaz de:

- Ler transações a partir de um arquivo CSV;
- Validar registros inválidos;
- Identificar transações suspeitas;
- Gerar um resumo mensal das movimentações;
- Exportar os resultados para um arquivo JSON;
- Exibir um relatório formatado no notebook;
- Gerar um gráfico em barras empilhadas com créditos e débitos por mês.

---

## 🛠️ Tecnologias utilizadas

- Python 3
- Google Colab
- CSV
- JSON
- Matplotlib

---

## 📁 Estrutura do projeto

```
.
├── analise_transacoes_financeiras.ipynb
├── transacoes.csv
├── relatorio.json
├── grafico.png
└── README.md
```

---

## ⚙️ Funcionalidades

O notebook foi organizado em funções com responsabilidades separadas:

- `ler_transacoes()`
  - Realiza a leitura do arquivo CSV.

- `validar_transacao()`
  - Verifica se cada transação possui dados válidos.

- `processar_transacoes()`
  - Filtra registros inválidos e identifica transações suspeitas.

- `gerar_relatorio()`
  - Calcula o resumo financeiro mensal.

- `salvar_json()`
  - Salva o relatório em formato JSON.

- `exibir_relatorio()`
  - Exibe um resumo formatado da análise.

---

## 🔍 Validações realizadas

Durante o processamento são verificadas situações como:

- Campos obrigatórios vazios;
- Valores inválidos;
- Conversão numérica;
- Tratamento de erros com `try/except`;
- Identificação de transações acima do limite considerado suspeito.

---

## 📈 Visualização

O projeto gera automaticamente um gráfico de barras empilhadas contendo:

- Total de créditos por mês;
- Total de débitos por mês.

O gráfico é salvo como:

```
grafico.png
```

---

## 📄 Arquivo JSON

Após o processamento é criado automaticamente:

```
relatorio.json
```

O arquivo contém:

- Data de geração;
- Quantidade de transações válidas;
- Quantidade de transações inválidas;
- Resumo mensal das movimentações.

---

## ▶️ Como executar

1. Abra o notebook no Google Colab.
2. Certifique-se de que o arquivo `transacoes.csv` esteja na mesma pasta.
3. Execute todas as células em ordem.
4. Ao final serão gerados:
   - relatório exibido na tela;
   - `relatorio.json`;
   - `grafico.png`.

---
