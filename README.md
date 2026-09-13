# ⚙️ Automatización de Operaciones para Clínica Psicológica (n8n)

Este repositorio contiene una serie de workflows creados en n8n para automatizar distintos procesos de una clínica de psicología. 

> **Nota de Privacidad:** Todos los archivos `.json` de este repositorio son muestras estructurales. Se han eliminado datos personales, nombres del equipo médico, IDs de Google Sheets, webhooks y Chat IDs de Telegram para proteger la privacidad de la clínica y los pacientes.

## 📂 Flujos Incluidos

### 1. `Semestral y Anual.json`
Un sistema de análisis de datos que se ejecuta periódicamente. 
* **Función:** Lee los registros brutos de pacientes desde Google Sheets, clasifica a los pacientes (mutualistas o privados) y calcula los ratios de conversión semestrales y anuales. 
* **Salida:** Registra los resultados históricos en una base de datos y envía un informe ejecutivo directamente a los responsables vía Telegram.

### 2. `ResumenReseñasSemanal.json`
Analista de experiencia de cliente impulsado por Inteligencia Artificial.
* **Función:** Recopila semanalmente las reseñas de las diferentes sedes de la clínica desde Google Sheets y las envía a un agente de IA. El agente categoriza el feedback (tiempos de espera, empatía, instalaciones, etc.).
* **Salida:** Genera un resumen ejecutivo que se guarda en Sheets y se difunde al equipo directivo por Telegram.

### 3. `ReseñasAutomatizacion.json`
Respondedor de reseñas automático.
* **Función:** Monitorea de forma continua la recepción de nuevas reseñas. Utiliza un agente de IA para redactar respuestas empáticas y personalizadas.
* **Salida:** Publica automáticamente la respuesta en Google y notifica al equipo por Telegram.

