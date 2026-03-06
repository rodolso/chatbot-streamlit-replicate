# Taller: Construye un Asistente de IA con Streamlit y Replicate

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/rodolso/chatbot-streamlit-replicate)

## Descripción

En este taller aprenderás a crear un asistente de inteligencia artificial desde cero, combinando la facilidad de uso de **Streamlit** con la potencia de los modelos de **Replicate**.

## Características principales

- Configuración de API sencilla con validación automática.  
- Interfaz conversacional con historial de conversación.  
- System Prompt editable para personalizar el comportamiento del modelo.  
- Streaming de respuestas en tiempo real.  
- Despliegue gratuito en Streamlit Cloud.

## Requisitos previos

- Una cuenta en [GitHub](https://github.com/signup).
- Una cuenta en [Replicate](https://replicate.com) para obtener un API Token.
- Una cuenta en [Streamlit Cloud](https://streamlit.io/cloud) para el despliegue.

## Instalación

### Opción 1: GitHub Codespaces (recomendada)

1. Usa este repositorio como plantilla.  
2. Desde tu copia del repositorio, abre tu entorno en **GitHub Codespaces** con el botón que encontrarás justo debajo.  
3. Las dependencias se instalarán automáticamente.

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/rodolso/chatbot-streamlit-replicate)

### Opción 2: Instalación local

```bash
# 1. Clona el repositorio
git clone https://github.com/rodolso/chatbot-streamlit-replicate.git
cd chatbot-streamlit-replicate

# 2. Crea un entorno virtual
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate

# 3. Instala las dependencias
pip install -r requirements.txt
```

## Instrucciones

Para completar correctamente el taller, y construir el asistente de IA, debes seguir las actividades incluidas en los cuadernos Jupyter del repositorio:

### Parte 1 — Uso de la API de Replicate  
**Archivo:** `01_Como_Usar_Replicate.ipynb`

- Aprenderás a registrarte en Replicate, generar un token y conectarte a la API.  
- Ejecutarás modelos de lenguaje, ajustarás parámetros y realizarás pruebas locales.

### Parte 2 — Creación de la interfaz con Streamlit  
**Archivo:** `02_Interfaz_con_Streamlit.ipynb`

- Construirás la interfaz web del chatbot paso a paso con Streamlit.  
- Implementarás la gestión del estado de sesión, el envío de mensajes y la recepción de respuestas en tiempo real.

Al finalizar ambas partes, tendrás un asistente conversacional completamente funcional y listo para desplegar en Streamlit Cloud.

## Consideraciones de seguridad

- No subas credenciales o tokens al repositorio.  
- Usa el archivo `secrets.toml` únicamente en desarrollo local.  
- Verifica que el archivo `.streamlit/secrets.toml` esté correctamente excluido del control de versiones.
- Opcional: Configura los secretos directamente en el entorno de producción (Streamlit Cloud).  

## Costes estimados

| Servicio | Coste | Detalles |
|-----------|--------|----------|
| **GitHub Codespaces** | Gratuito (hasta 120h/mes) | Instancias de 2 núcleos |
| **Streamlit Cloud** | Gratuito | Limitaciones de CPU y memoria |
| **Replicate API** | Pago por uso | Meta Llama 3 8B Instruct: ~$0.0005 / 1K tokens entrada, ~$0.0025 / 1K tokens salida |


## Contribuciones

Proyecto en desarrollo, las contribuciones son bienvenidas.  
Si encuentras un error o quieres proponer mejoras, abre un *issue* o envía un *pull request*.  

## Licencia

- Este proyecto se distribuye bajo licencia MIT.  
- Para la licencia de los modelos LLaMA, consulta el Acuerdo de Licencia de Meta Platforms, Inc.  

## Aviso

El objetivo de este taller es construir una Prueba de Concepto sencilla.  
La aplicación resultante no está lista para producción y se proporciona sin garantía alguna. El uso de este proyecto es bajo tu propia responsabilidad.

## Autoría

Rodrigo Oliver - [LinkedIn](https://www.linkedin.com/in/rodrigo-oliver)  
*Data Scientist, Lead Instructor Bootcamp Data Science Online @ The Bridge School*  

Proyecto adaptado a partir de:  
- [streamlit-replicate-app](https://github.com/sfc-gh-cnantasenamat/streamlit-replicate-app)  
- [llama2-chatbot](https://github.com/a16z-infra/llama2-chatbot)

## Recursos adicionales

- [Documentación oficial de Streamlit](https://docs.streamlit.io)  
- [Documentación de Replicate](https://replicate.com/docs)  
- [Meta Llama 3 8B Instruct en Replicate](https://replicate.com/meta/meta-llama-3-8b-instruct)  
