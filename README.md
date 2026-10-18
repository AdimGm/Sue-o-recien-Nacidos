# Pipeline de IA para analizar patrones de sueño en recién nacidos

## 1. Descripción
Proyecto académico que demuestra un flujo de trabajo de Inteligencia Artificial y Machine Learning para explorar patrones de sueño en recién nacidos usando exclusivamente datos sintéticos. El proyecto representa el problema mediante un espacio de estados, implementa un pipeline de razonamiento/búsqueda y entrena un modelo de regresión para estimar la duración total del sueño registrada en un periodo simulado de 24 horas.

**Importante:** los datos son inventados para practicar programación y no representan pacientes reales. El modelo no evalúa la salud del bebé, no detecta trastornos y no debe utilizarse para tomar decisiones médicas o de cuidado infantil.

## 2. Objetivo general
Implementar y documentar un pipeline reproducible en Python, GitHub y Google Colab para generar datos sintéticos, validarlos, explorarlos, entrenar un modelo de regresión y visualizar sus resultados.

## 3. Variables
| Variable | Descripción | Tipo |
|---|---|---|
| edad_dias | Edad simulada en días (0–28) | Numérica |
| tomas_24h | Número simulado de tomas en 24 horas | Numérica |
| despertares_24h | Número simulado de despertares en 24 horas | Numérica |
| siestas_24h | Número simulado de episodios de sueño | Numérica |
| sueno_diurno_h | Horas de sueño diurno simuladas | Numérica |
| sueno_nocturno_h | Horas de sueño nocturno simuladas | Numérica |
| sueno_total_h | Suma de horas de sueño diurno y nocturno; objetivo de regresión | Numérica |

Estas variables son demostrativas y no son criterios clínicos.

## 4. Espacio de estados
- S0: inicio.
- S1: datos sintéticos generados.
- S2: datos validados.
- S3: datos explorados y preparados.
- S4: modelo de regresión entrenado.
- S5: predicciones evaluadas y visualizadas.

Operadores:
- O1: generar datos.
- O2: validar rangos y consistencia.
- O3: explorar y separar variables.
- O4: entrenar el modelo.
- O5: evaluar y visualizar.

## 5. Modelo predictivo
Se utiliza `RandomForestRegressor` para estimar `sueno_total_h` a partir de variables sintéticas. El conjunto de datos se divide en entrenamiento y prueba. Se calculan MAE, RMSE y R² y se grafica la comparación entre valores reales sintéticos y predicciones.

## 6. Estructura del repositorio
```text
pipeline-tipo-c-sueno-recien-nacidos/
├── README.md
├── pipeline_razonamiento_tipo_c.ipynb
└── modelo_prediccion_sueno_tipo_c.ipynb
```

## 7. Ejecución
1. Sube los dos notebooks a GitHub.
2. Abre cada notebook con Google Colab.
3. Ejecuta las celdas en orden.
4. Comprueba las métricas y los gráficos generados.

## 8. Limitaciones y uso responsable
Los datos, relaciones y resultados son artificiales. La evaluación mide únicamente el comportamiento del modelo sobre datos sintéticos; no permite inferir patrones de sueño reales ni realizar recomendaciones clínicas. Para estudios reales se requerirían datos adecuados, revisión ética, protección de datos y validación por especialistas.
