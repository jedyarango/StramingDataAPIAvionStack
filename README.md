# ✈️ AviationStack Data Streaming Pipeline (GCP)

Este proyecto implementa una arquitectura de **Streaming de Datos** en tiempo real utilizando la API de **AviationStack**. El objetivo es ingestar, procesar y almacenar información de vuelos en vivo dentro de la infraestructura de Google Cloud Platform.

---

## 🏗️ Arquitectura del Proyecto

El flujo de datos sigue este camino:
1. **Extracción:** Script en Python que consume la API de AviationStack.
2. **Ingesta:** Mensajería en tiempo real mediante **Pub/Sub**.
3. **Procesamiento:** Ejecución serverless del script mediante **Cloud Run**.
4. **Almacenamiento:** Data Warehouse en **BigQuery** para análisis.
5. **Seguridad:** Gestión de permisos y roles con **IAM**.

---

## 📊 Visualización del Proyecto
<img width="886" height="451" alt="image" src="https://github.com/user-attachments/assets/52a909c1-95cf-4bd3-a417-a38bf6b6dcd7" />
<img width="886" height="441" alt="image" src="https://github.com/user-attachments/assets/b4b52488-d017-4176-aa43-7a2f6b8672e5" />


## 🛠️ Tecnologías Utilizadas

* **Google Cloud Pub/Sub:** Ingesta de mensajes de streaming.
* **Google Cloud Run:** Orquestación y ejecución de script.
* **BigQuery:** Almacenamiento y análisis de datos a gran escala.
* **IAM (Identity and Access Management):** Configuración de Service Accounts y permisos mínimos necesarios.
* **Python:** Lenguaje principal para la lógica de extracción y carga (ETL).

---
