# Desigualdad socioeconómica en comprensión lectora en Chile

## 1. Descripción del proyecto

Este proyecto corresponde a la Entrega 03 del curso Narración Gráfica de No Ficción (COM-208), de la Pontificia Universidad Católica de Chile.

La investigación analiza la evolución de los puntajes de comprensión lectora de estudiantes chilenos según quintil socioeconómico y cultural, utilizando resultados de PISA entre 2006 y 2022.

Forma parte del proyecto grupal Cuando las brechas se achican, pero no todos avanzan, que investiga las desigualdades educativas desde dos dimensiones: género y nivel socioeconómico.

## 2. Pregunta de investigación

¿Cómo ha evolucionado la diferencia de desempeño lector entre los estudiantes chilenos de los quintiles socioeconómicos más altos y más bajos entre 2006 y 2022?

## 3. Hipótesis

La ventaja en comprensión lectora de los estudiantes socioeconómicamente más favorecidos persiste, pero la distancia respecto de los menos favorecidos ha disminuido. Esta reducción se explica descriptivamente tanto por el avance del quintil inferior como por el retroceso del superior.

## 4. Fuente de datos

Los datos provienen de la Agencia de Calidad de la Educación de Chile, presentación PISA 2022: Evaluación internacional de estudiantes tras la pandemia, página 27, gráfico «Lectura: tendencia Chile según quintil socioeconómico y cultural 2006–2022».

Se utilizan seis evaluaciones: 2006, 2009, 2012, 2015, 2018 y 2022.

Los puntajes fueron transcritos del gráfico oficial. No corresponden a microdatos individuales.

## 5. Preparación y limpieza

La base se organizó en formato CSV mediante Python y pandas.

Se realizaron las siguientes operaciones:

1. Transcripción de los puntajes publicados.
2. Organización de los registros por año y quintil.
3. Estandarización de los nombres de los cinco quintiles.
4. Comprobación de registros y valores faltantes.
5. Cálculo de la diferencia entre los quintiles extremos.

La base final contiene 30 registros: cinco quintiles en seis años.

### Diccionario de datos

| Variable | Descripción |
|---|---|
| anio | Año de aplicación de PISA |
| quintil_socioeconomico | Grupo socioeconómico y cultural |
| puntaje_lectura | Puntaje promedio de comprensión lectora |

No se imputaron valores ni se calcularon estimaciones estadísticas adicionales.

## 6. Visualización

Se desarrolló un gráfico de líneas con Altair para comparar la evolución de los cinco quintiles socioeconómicos y culturales.

La visualización permite identificar las diferencias entre grupos, observar períodos de aumento o disminución y consultar los puntajes mediante herramientas interactivas.

El gráfico se exporta en HTML interactivo y JPG estático.

## 7. Principales hallazgos

En 2006, el quintil más favorecido obtuvo 517 puntos y el menos favorecido 391, una diferencia de 126 puntos.

En 2022, los puntajes fueron 495 y 413, respectivamente, reduciendo la distancia a 82 puntos.

Entre 2006 y 2022, el quintil superior disminuyó 22 puntos y el inferior aumentó 22 puntos.

Según el informe oficial, entre 2018 y 2022 el quintil más favorecido fue el único que registró una disminución estadísticamente significativa en lectura.

## 8. Limitaciones

Los datos son promedios agregados de distintas aplicaciones de PISA. No permiten identificar trayectorias individuales ni establecer relaciones causales entre nivel socioeconómico y desempeño lector.

Las diferencias y variaciones calculadas son descriptivas. No se estimaron intervalos de confianza ni pruebas propias de significancia estadística.

## 9. Reproducibilidad

El análisis se desarrolla en Google Colab utilizando Python, pandas, Altair y vl-convert-python.

Para reproducirlo:

1. Abrir visualizacion_pisa_socioeconomico_chile.ipynb en Google Colab.
2. Ejecutar las celdas en orden.
3. Generar el CSV a partir de los valores documentados.
4. Construir el gráfico interactivo.
5. Exportar las versiones HTML y JPG.

## 10. Archivos del repositorio

- README.md: documentación del proyecto.
- cronica.md: crónica periodística.
- pisa_chile_lectura_quintiles_2006_2022.csv: base de datos limpia.
- visualizacion_pisa_socioeconomico_chile.ipynb: código reproducible.
- visualizacion_pisa_socioeconomico.html: visualización interactiva.
- visualizacion_pisa_socioeconomico.jpg: visualización estática.

