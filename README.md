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

•	¿Cuántas solicitudes son para un solo paciente vs múltiples pacientes?
•	¿Qué diagnosticados están más afectados por la falta de disponibilidad de medicamentos?
•	¿Cuáles son los medicamentos más críticos según la cantidad solicitada?
•	¿Qué formas farmacéuticas tienen mayor demanda?
•	De los primeros tres medicamentos más críticos según su forma farmacéutica, ¿Cómo varia la cantidad solicitada del medicamento con mayor demanda?

