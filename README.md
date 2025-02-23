# Analisis de medicamentos no disponibles con Excel

En este proyecto analizaremos los medicamentos no disponibles, este conjunto de datos se encuentra en la página de [Datos Abiertos](https://www.datos.gov.co/d/sdmr-tfmf). Se trata en una deficiencia de medicamentos indispensables para diferentes enfermedades o patologías como la leucemia mieloide aguda, acondroplasia y diferentes tipos de tumores, que, por condiciones en su comercialización, hay muy pocas o nulas existencias de estos medicamentos.

## Tabla de contenido

- [Diccionario de datos](#diccionario-de-datos)
- [Limpieza y formato de datos](#limpieza-y-formato-de-datos)
- [Preguntas problemas](#preguntas-problemas)
- [Analisis](#analisis)

## Diccionario de datos

| Nombre columna | Tipo de dato |
| --- | --- |
| Fecha de autorización | Marca de tiempo |
| Tipo solicitud | Texto |
| Solicitante/Importador | Texto |
| IUM| Texto |
| Principio activo 1 | Texto |
| Concentración 1 | Texto |
| Unidad medida 1 | Texto |
| Principio activo 2 | Texto |
| Concentración 2 | Texto |
| Unidad medida 2 | Texto |
| Forma farmaceutica | Texto |
| Nombre comercial | Texto |
| Cantidad solicitada | Número |
| Presentación comercial | Texto |
| Diagnostico | Texto |
| Codigo diagnostico | Texto |

## Limpieza y formato de datos

En la limpieza de los datos hubo problemas en definir correctamente el formato fecha de la primera celda, la solución que me funciono fue eliminar datos innecesarios mediante la herramienta reemplazar y luego darle el formato correcto con la herramienta de texto en columnas.

![image](https://github.com/user-attachments/assets/62df0001-580d-4d2c-b3c7-4a1270d68689)
![image](https://github.com/user-attachments/assets/bebe9e25-ba99-4689-bedc-5889cacf6a68)

## Preguntas problema

- ¿Cuántas solicitudes son para un solo paciente vs múltiples pacientes?
- ¿Qué diagnosticados están más afectados por la falta de disponibilidad de medicamentos?
- ¿Cuáles son los medicamentos más críticos según la cantidad solicitada?
- ¿Qué formas farmacéuticas tienen mayor demanda?
- De los primeros tres medicamentos más críticos según su forma farmacéutica, ¿Cómo varia la cantidad solicitada del medicamento con mayor demanda?

## Análisis

- ¿Cuántas solicitudes son para un solo paciente vs múltiples pacientes?

![image](https://github.com/user-attachments/assets/fe6984d3-5625-42b6-bf07-09865927ad0d)

> Hay 4.442 solicitudes para un solo paciente vs 2.602 solicitudes para múltiples pacientes.

- ¿Qué diagnosticados están más afectados por la falta de disponibilidad de medicamentos?

![image](https://github.com/user-attachments/assets/687c63da-3f0c-4717-8c05-691fda4caad7)

> Dentro del top 10, los primeros tres (excluyendo los no reportados) diagnósticos más afectados por la disponibilidad de medicamentos son:
  > 1.	Distrofia muscular con 992 casos
  > 2.	Fibrosis quística con manifestaciones pulmonares con 299 casos
  > 3.	Fibrosis quística, sin otra especificación con 256 casos

- ¿Cuáles son los medicamentos más críticos según la cantidad solicitada?

![image](https://github.com/user-attachments/assets/1ceb20d2-1620-4373-ab9e-a95b648b6373)

> Dentro del top 10, los primeros tres medicamentos más críticos según la cantidad solicitada son:
>   1.	Tolvaptan con 19.067 medicamentos solicitados
>   2.	Fibrinogeno coagulable con 19.030 medicamentos solicitados
>   3.	Inmunoglobulina humana normal con 16.640 medicamentos solicitados

- ¿Qué formas farmacéuticas tienen mayor demanda?

![image](https://github.com/user-attachments/assets/d7a75cca-69e7-4ae1-88c5-87f418275675)

> Dentro del top 10 de las formas farmacéuticas las tres primeras que tienen mayor demanda son:
>   1.	Solución inyectable con 2.509 solicitudes
>   2.	Tableta con 1.926 solicitudes
>   3.	Polvo liofilizado para reconstruir con 850 solicitudes

- De los primeros tres medicamentos más críticos según su forma farmacéutica, ¿Cómo varia la cantidad solicitada del medicamento con mayor demanda?

![image](https://github.com/user-attachments/assets/61e9d345-a28e-45aa-a4dd-9e16e3b4e6d6)

> El medicamento con mayor demanda según la suma de solicitudes y la forma farmacéutica más demandada es el Tolvaptan – Tolvaheal TAB, lo cual se presenta su desviación estándar en el grafico anterior.
