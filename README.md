## Modelo de Valoración de Activos Financieros (CAPM)

Este proyecto implementa una calculadora del modelo de valoración de activos financieros (CAPM) utilizando Python y Streamlit. 

#### Características:

- Los usuarios pueden seleccionar hasta 4 acciones de una lista predefinida para analizar.
- Permite especificar el número de años de datos históricos a considerar.
- Proporciona gráficos interactivos para visualizar los precios históricos de las acciones seleccionadas y sus precios normalizados.
- Calcula el valor Beta para cada acción seleccionada con respecto al índice S&P 500. También calcula el rendimiento esperado utilizando la fórmula del CAPM.


#### Detalles de Implementación:
- Fuentes de Datos: Utiliza Yahoo Finance (a través de yfinance) y Federal Reserve Economic Data (FRED) a través de pandas_datareader para obtener precios históricos de acciones y datos del índice S&P 500.
- Visualización: Utiliza plotly y plotly.express para generar gráficos interactivos dentro de la aplicación Streamlit.
- Funciones Auxiliares: Incluye funciones en functions.py para normalizar precios, calcular rendimientos diarios y calcular valores Beta.

##### Configuración:
Para ejecutar esta aplicación localmente:
- Clone el repositorio.

    `git clone https://github.com/vcarol/capm-app.git`
- Instale los paquetes requeridos (streamlit, pandas, yfinance, plotly, numpy, pandas_datareader) utilizando pip.

    `pip install -r requirements.txt`
- Ejecute la aplicación con streamlit run capm.py desde la línea de comandos.
    
    `streamlit run capm.py`

O lo puedes probar directamente aquí:
[Ver demo](https://capm-app.streamlit.app/)