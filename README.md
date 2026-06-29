````markdown
# OpenAI API Quickstart - Python

Este repositorio contiene múltiples aplicaciones de inicio rápido para diferentes endpoints de la API de OpenAI (chat, asistentes, etc.). Consulta la carpeta `examples` para probar distintos ejemplos y comenzar a utilizar la API de OpenAI.

## Autor

**Abelardo Carcamo**

Estudiante de Licenciatura en Ciberseguridad

Universidad Tecnológica de Panamá (UTP)

Grupo: **1S3232**

---

## Solicitud básica

Para enviar tu primera solicitud a la API utilizando el SDK de OpenAI para Python, asegúrate de tener instaladas las dependencias necesarias y luego ejecuta el siguiente código:

```python
from openai import OpenAI

client = OpenAI()

completion = client.chat.completions.create(
    model="gpt-3.5-turbo",
    messages=[
        {"role": "system", "content": "You are a helpful assistant."},
        {"role": "user", "content": "Hello!"}
    ]
)

print(completion.choices[0].message)
```

## Configuración

1. Si no tienes Python instalado, descárgalo e instálalo desde **Python.org**.

2. Clona este repositorio.

3. Navega al directorio del proyecto:

```bash
cd openai-quickstart-python
```

4. Crea un nuevo entorno virtual.

### macOS

```bash
python -m venv venv
source venv/bin/activate
```

### Windows

```cmd
python -m venv venv
.\venv\Scripts\activate
```

5. Instala las dependencias del proyecto:

```bash
pip install -r requirements.txt
```

6. Crea una copia del archivo de variables de entorno de ejemplo:

### Linux / macOS

```bash
cp .env.example .env
```

### Windows (PowerShell)

```powershell
Copy-Item .env.example .env
```

7. Agrega tu clave de API de OpenAI al archivo `.env` recién creado.

```text
OPENAI_API_KEY=tu_api_key
```

8. Ejecuta la aplicación.

Este paso depende del ejemplo que desees ejecutar.

Si el ejemplo utiliza Flask (como `chat-basic`), puedes iniciarlo con:

```bash
flask run
```

o directamente con:

```bash
python examples/chat-basic/app.py
```

Una vez iniciado, podrás acceder a la aplicación desde tu navegador en:

```
http://localhost:5000
```

Si el ejemplo corresponde a un script de Python sin Flask, simplemente ejecútalo con:

```bash
python nombre_del_archivo.py
```

## Ejemplos incluidos

La carpeta `examples` contiene diferentes ejemplos para aprender a utilizar la API de OpenAI:

- **chat-basic** — Aplicación básica de chat utilizando Flask.
- **assistant-basic** — Ejemplo básico del uso de asistentes.
- **assistant-functions** — Ejemplo del uso de Function Calling.
- **assistant-flask** — Interfaz web para interactuar con asistentes mediante Flask.

Estos ejemplos sirven como punto de partida para comprender el funcionamiento del SDK de OpenAI y desarrollar aplicaciones propias.
````
