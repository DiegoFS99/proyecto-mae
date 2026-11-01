# Proyecto MAE: Modelos de análisis estadístico

Proyecto del curso Modelos de análisis estadístico. Trabaja dos casos con datos de competencias de Kaggle:

- **CasaRoble (regresión):** predecir el precio de venta de una vivienda a partir de sus características, las del
  conjunto residencial y las de su entorno.
- **UniBank (clasificación).**

## Notebooks

| Notebook | Contenido |
|---|---|
| `Problema_de_clasificacion.ipynb` | Contexto, limpieza y medidas descriptivas del problema de clasificación. |
| `Problema_de_regresion.ipynb` | Contexto, limpieza y medidas descriptivas del problema de regresión. |
| `Problema_de_regresion_completo.ipynb` | Análisis exploratorio completo de regresión: diagramas de caja, tablas de contingencia y correlaciones. |
| `modelo_regresion_lineal.ipynb` | Modelo de regresión lineal para CasaRoble. Tiene desarrolladas la selección de variables, la determinación de la estructura y las predicciones para Kaggle. Las secciones 3 a 8 están pendientes: estimación, supuestos, bondad de ajuste, intervalos, pruebas e interpretación. |

## Cómo ejecutarlos

1. Crear el entorno e instalar las dependencias (Python 3.13):

   ```
   python -m venv .venv
   .venv\Scripts\activate          # en Windows; en macOS o Linux: source .venv/bin/activate
   pip install -r requirements.txt
   ```

2. Copiar `.env.example` como `.env` y escribir el `KAGGLE_API_TOKEN`. El token se genera desde la cuenta de Kaggle,
   después de aceptar las reglas de la competencia. Los notebooks descargan los datos con `kagglehub`.
3. Abrir el notebook y ejecutar todas las celdas en orden.

`modelo_regresion_lineal.ipynb` genera los archivos `submission_*.csv` para Kaggle. Git no los sigue.
