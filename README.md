# Chatbot con la API de OpenAI en Python

## Descripción

Este proyecto consiste en la implementación de un chatbot utilizando la API de OpenAI y Python, siguiendo la estructura y funcionamiento del repositorio oficial **OpenAI Quickstart Python**.

El objetivo es comprender el funcionamiento de la API, la arquitectura de un chatbot, el manejo del historial de conversación, el uso de Flask para aplicaciones web y la integración con modelos de lenguaje.

Este proyecto ha sido desarrollado con fines académicos para la asignatura correspondiente de la Licenciatura en Ciberseguridad.

---

# Objetivos

## Objetivo General

Replicar el funcionamiento del repositorio oficial **OpenAI Quickstart Python**, comprendiendo cada uno de sus componentes y el proceso completo de comunicación entre la aplicación y la API de OpenAI.

## Objetivos Específicos

- Configurar correctamente el entorno de desarrollo.
- Comprender la estructura del proyecto.
- Implementar un chatbot utilizando la API de OpenAI.
- Comprender el funcionamiento del historial de conversación.
- Implementar transmisión de respuestas (Streaming).
- Comprender el uso de Function Calling.
- Analizar el funcionamiento de Flask como servidor web.

---

# Tecnologías utilizadas

- Python
- Flask
- OpenAI API
- HTML5
- CSS3
- JavaScript
- Git
- GitHub

---

# Requisitos

- Python 3.10 o superior
- Cuenta en OpenAI
- API Key válida
- Git

---

# Instalación

## 1. Clonar el repositorio

```bash
git clone <URL_DEL_REPOSITORIO>
```

## 2. Ingresar al proyecto

```bash
cd openai-quickstart-python
```

## 3. Crear un entorno virtual

### Windows

```powershell
python -m venv venv
.\venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

## 4. Instalar las dependencias

```bash
pip install -r requirements.txt
```

## 5. Configurar la API Key

Crear un archivo llamado

```
.env
```

con el siguiente contenido:

```env
OPENAI_API_KEY=TU_API_KEY
```

---

# Estructura del proyecto

```
openai-quickstart-python
│
├── examples
│   ├── assistant-basic
│   ├── assistant-flask
│   ├── assistant-functions
│   └── chat-basic
│
├── .env.example
├── .gitignore
├── README.md
└── requirements.txt
```

---

# Ejecución

Cada ejemplo puede ejecutarse de forma independiente.

Ejemplo:

```bash
python app.py
```

o

```bash
flask run
```

dependiendo del ejemplo seleccionado.

---

# Autor

**Chester Ivan Ferrer Hernandez**

Estudiante de Licenciatura en Ciberseguridad

Grupo **1S3232**

---

# Créditos

Este proyecto se basa en el repositorio oficial **OpenAI Quickstart Python**, utilizado exclusivamente con fines educativos y académicos.