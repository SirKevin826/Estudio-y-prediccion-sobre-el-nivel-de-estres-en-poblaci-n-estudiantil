# Estudio-y-prediccion-sobre-el-nivel-de-estres-en-poblaci-n-estudiantil

## Descripción general

Proyecto de desarrollo completo de un proyecto de clasificación predictiva del nivel de estrés (bajo, medio, alto) a partir de 20 factores psicológicos, fisiológicos, académicos y sociales, siguiendo la metodología CRISP-DM. Se cubren las fases de comprensión y preparación de datos, análisis exploratorio y de correlación, modelado comparativo y evaluación, cerrando con recomendaciones de despliegue.

El propósito de este análisis es identificar los factores más asociados al nivel de estrés en una población estudiantil y construir un modelo capaz de clasificar a un individuo en una de tres categorías de estrés (bajo, medio, alto) a partir de indicadores autorreportados de salud mental, salud física, entorno académico y entorno social.

## Datos

El dataset stress_level, obtenido mediante la librería meddatasets, contiene 1,100 registros y 21 columnas: 20 variables predictoras de tipo entero y la variable objetivo stress_level (0 = bajo, 1 = medio, 2 = alto). Las variables cubren cuatro dimensiones:
- Psicológica/emocional: anxiety_level, self_esteem, mental_health_history, depression, future_career_concerns.
- Fisiológica: headache, blood_pressure, sleep_quality, breathing_problem.
- Entorno y necesidades básicas: noise_level, living_conditions, safety, basic_needs.
- Académico y social: academic_performance, study_load, teacher_student_relationship, social_support, peer_pressure, extracurricular_activities, bullying.

En cuanto a la Calidad de los datos, se encontraron con lo siguiente:
- Valores nulos: 0 en las 21 columnas.
- Registros duplicados: 0.
- Tipos de datos: consistentes (int64 en todas las columnas), sin necesidad de conversión.

## Metodologías

Para la realización del proyecto, se contó con los siguientes acciones

- Ciclo CRISP-DM: Compresión del negocio y datos, preparación de datos, y modelado de regesión logistica multinomial.

- Análisis de correlación: correlación con la variable objetivo, y multicolinealidad entre predictores.

- Modelado: Modelado de regresión logisitica multinomial, desarrollo de Random Forest y Gradient Boosting y comparación de los tres modelados

## Hallazgos principales

Los tres modelos evaluados (regresión logística multinomial, Random Forest y Gradient Boosting) alcanzan un desempeño equivalente (86–89% de accuracy), lo que indica que la relación entre los factores analizados y el nivel de estrés es predominantemente lineal. 

## Recomendaciones

Se recomienda la regresión logística multinomial como modelo final por su balance entre precisión e interpretabilidad.

