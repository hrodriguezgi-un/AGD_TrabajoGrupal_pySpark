# Análisis e Implementación en SparkQL

Los dos conjuntos de datos entregados, CSV separados por coma, Evaluación del Pitch (2021.04.13 ISoftware).csv y Asistencia del Pitch (2021.04.13 ISoftware).csv proceden de dos encuestas realizadas con Google Forms.

Los archivos proceden de las evaluaciones de los pitch (exposiciones cortas de negocio) que realizan los estudiantes de la asignatura de Ingeniería de Software. Los estudiantes están organizados en equipos. Cada equipo realiza una presentación de máximo 15 minutos, una vez inicia la presentación todos los estudiantes deben registrar su asistencia lo cual queda registrado en 'Asistencia del Pitch (2021.04.13 ISoftware).csv' incluidos los miembros del equipo.

El archivo Asistencia del Pitch (2021.04.13 ISoftware).csv contiene las columnas: "Marca temporal" es tiempo dado en fecha y hora, "Nombre de usuario" es el correo electrónico del estudiante y es texto,"Equipo al que perteneces:" equipo de trabajo al que pertenece el estudiante también es texto y "Equipo que va a exponer:" equipo que el estudiante va a tender a su presentación.

El archivo Evaluación del Pitch (2021.04.13 ISoftware).csv contiene las columnas "Marca temporal" es tiempo dado en fecha y hora, "Nombre de usuario" es el correo electrónico del estudiante y es texto, "Equipo que vas a evaluar:" equipo que ha expuesto y que va a ser evaluado por cada estudiante que no sea integrante; a continuación, se tienen las siguientes columnas que corresponden a la evaluación de los respectivos ítems:

- "Introducción: El equipo responde adecuadamente ¿Quiénes son y por qué están aquí?",
- "Equipo: El equipo responde adecuadamente ¿Quiénes están detrás de la idea y cuál es su función?",
- "Problema: El equipo responde adecuadamente ¿Qué problema resolverá?, ¿es realmente un problema?",
- "Ventajas: El equipo responde adecuadamente ¿Por qué su solución es especial?, ¿qué la hace distinta de otras?",
- "Solución: El equipo responde adecuadamente ¿Cómo piensa resolver el problema?",
- "Producto: El equipo responde adecuadamente ¿Cómo funciona el producto o servicio? Muestra algunos ejemplos.",
- "Tracción: El equipo responde adecuadamente si cuenta con clientes que demuestran potencial.",
- "Mercado: El equipo responde conoce, o por lo menos intentar predecir, el tamaño del mercado que impactará.",
- "Competencia: El equipo responde adecuadamente ¿Cuáles son las soluciones alternativas al problema que plantea?",
- "Modelo de negocio: El equipo responde adecuadamente ¿Cómo hará dinero? ",
- "Inversión: El equipo responde adecuadamente ¿Cuál es su presupuesto y cuánto espera ganar?",
- "Contacto: El equipo deja los datos al cliente y muestra cómo pueden contactarle.",
- "Exposición: ¿Qué tan coordinados estaban los expositores?",
- "Exposición: ¿Los expositores se expresaron con claridad y se hicieron entender?",
- "Exposición: Las diapositivas son claras y coherentes y apoyaron adecuadamente la exposición.",
- "Suponiendo que eres inversionista, ¿Estarías dispuesto a invertir dinero en este equipo? (esta pregunta no se pondera en la nota)",
- "Observaciones para el equipo, estas observaciones las debe considerar el equipo para mejorar la siguiente presentación."
Cada ítem se evalúa con la siguiente escala: 0. Ausente; 1. Deficiente; 2. Regular; 3. Aceptable; 4. Bueno; 5. Excelente

Cargue los datos, cada archivo en una tabla SparkSQL y responda cada una de las consultas dadas en cada celda. Tenga en cuenta que algunas consultas pueden tener como resultado el vacío.
