# Predição do Consumo de Combustível

## Descrição

Este projeto visa prever o consumo de combustível de um veículo com base no tamanho do motor e no número de cilindros, utilizando um modelo de regressão linear. O projeto disponibiliza uma API FastAPI para realizar as previsões.

## Dados

Os dados utilizados para treinar o modelo estão no arquivo `FuelConsumption.csv`.

## Modelo

O modelo de regressão linear foi treinado utilizando a biblioteca scikit-learn e está salvo no arquivo `LinearModel.pkl`.

## Uso

O modelo pode ser utilizado para prever o consumo de combustível de um veículo informando o tamanho do motor e o número de cilindros.

**API FastAPI:**

A API FastAPI pode ser utilizada para realizar as previsões.

**Endpoint:** `/predict/`

**Método:** `POST`

**Entrada:**

```json
{
  "input1": tamanho_do_motor,
  "input2": numero_de_cilindros
}
```

**Saída:**

```json
{
  "prediction": consumo_de_combustivel
}
```

## Arquivos

* `app.py`: Arquivo principal do projeto, contendo a API FastAPI.
* `FuelConsumption.csv`: Dados utilizados para treinar o modelo.
* `LinearModel.pkl`: Modelo de regressão linear treinado.
* `Notebook.ipynb`: Notebook com o código para treinar o modelo.

## Resultados

O modelo apresentou um erro médio absoluto de aproximadamente 2.8 L/100km na predição do consumo de combustível.

## Autor

Felipe

## Contato

felipe.b.moraes@gmail.com
