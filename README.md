# Taller: Construye un Asistente de IA con Streamlit y Replicate

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

### Opción 1: Plantilla + GitHub Codespaces (recomendada)

1. Crea tu propia copia de este repositorio usándolo como plantilla, puedes hacerlo pulsando el botón verde **Step 1: Use this template**.  
2. Abre tu copia del repositorio en un entorno de programación en *GitHub Codespaces*, puedes hacerlo con el botón **Step 2: Open in GitHub Codespaces**.  
3. En el menú de creación de *GitHub Codespaces*, selecciona tu repositorio en el desplegable *Repository* y el resto de campos deberían configurarse solos.  
    > **Importante:** En la parte inferior del menú verás que GitHub te solicita tu token de Replicate así que, si dispones de uno, introdúcelo y pulsa **Create Codespace**.
4. Las dependencias se instalarán automáticamente en el entorno y podrás comenzar el taller.

<p align="center">
  <a href="https://github.com/rodolso/chatbot-streamlit-replicate/generate">
    <img src="https://img.shields.io/badge/Step_1:_Use_this_template-2ea44f?style=for-the-badge&logo=github&logoColor=white" alt="Use this template"/>
  </a>
  <a href="https://codespaces.new/">
    <img src="https://img.shields.io/badge/Step_2:_Open_in_GitHub_Codespaces-181717?style=for-the-badge&logo=github&logoColor=white" alt="Open in GitHub Codespaces"/>
  </a>
</p>

### Opción 2: GitHub Codespaces (sin plantilla)

Si solo quieres explorar el taller libremente, puedes crear un entorno en GitHub Codespaces basado en este repositorio y, si al final te gusta lo que has aprendido, guardar los cambios en tu propio repositorio haciendo un *fork*.

Para hacerlo puedes usar el siguiente acceso rápido:

<p align="center">
  <a href="https://codespaces.new/rodolso/chatbot-streamlit-replicate">
    <img src="https://github.com/codespaces/badge.svg" alt="Open in GitHub Codespaces"/>
  </a>
</p>


### Opción 3: Instalación local

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

Para construir nuestro asistente de IA debes seguir las actividades incluidas en los cuadernos Jupyter del repositorio:

### Parte 1 — Uso de la API de Replicate  
**Archivo:** `01_Como_Usar_Replicate.ipynb`

- Aprenderás a registrarte en Replicate, generar un token y conectarte a la API.  
- Ejecutarás modelos de lenguaje, ajustarás parámetros y realizarás pruebas locales.

### Parte 2 — Creación de la interfaz con Streamlit  
**Archivo:** `02_Interfaz_con_Streamlit.ipynb`

- Construirás la interfaz web del chatbot paso a paso con Streamlit.  
- Implementarás la gestión del estado de sesión, el envío de mensajes y la recepción de respuestas en tiempo real.

Al finalizar ambas partes, tendrás un asistente conversacional completamente funcional y listo para desplegar en *Streamlit Cloud*.

## Consideraciones de seguridad

- No subas credenciales o tokens al repositorio.  
- Usa el archivo `secrets.toml` únicamente en desarrollo local.  
- Verifica que el archivo `.streamlit/secrets.toml` esté correctamente excluido del control de versiones.
- Opcional: Configura los secretos directamente en el entorno de producción (*GitHub Codespaces* y *Streamlit Cloud*).  

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
- Para la licencia de los modelos Llama, consulta el Acuerdo de Licencia de Meta Platforms, Inc.  

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
