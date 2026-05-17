# TFM - LSTM Portfolio Optimization

Este repositorio contiene el código desarrollado para el Trabajo Final de Máster titulado:

**Optimización de carteras mediante Deep Learning: diseño y análisis de un sistema de asignación dinámica de activos basado en LSTM**

## Descripción

El proyecto implementa un sistema cuantitativo de asignación dinámica de activos basado en redes neuronales LSTM bajo un enfoque end-to-end. El modelo genera directamente los pesos de una cartera compuesta por ETFs y se compara frente a estrategias tradicionales como:

- Buy & Hold sobre ACWI
- Equal Weight
- Optimización Markowitz Max Sharpe restringida
- Modelo LSTM end-to-end

## Universo de inversión

Los activos utilizados son:

- SPY
- VGK
- EWJ
- VWO
- XLK
- XLE
- GLD

El benchmark utilizado es:

- ACWI

## Metodología

El sistema utiliza datos semanales descargados mediante `yfinance`, ingeniería de variables financieras, rebalanceo mensual y validación walk-forward fuera de muestra.

Las principales métricas evaluadas son:

- CAGR
- Volatilidad anualizada
- Ratio de Sharpe
- Maximum Drawdown
- Tracking Error
- Information Ratio
- Turnover

## Notebook principal

El notebook principal del proyecto es:

```text
TFM_LSTM_Portfolio_Optimization.ipynb
