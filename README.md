# Proyecto Python - Gestión de Datos

## Descripción

Proyecto desarrollado con **Python y FastAPI** para la creación de una API REST orientada a la gestión de información.

El proyecto cuenta con diferentes versiones implementadas mediante ramas de Git, permitiendo trabajar con distintos mecanismos de almacenamiento de datos.

### Versiones del proyecto

* **`main`**: contiene la versión principal y estable del proyecto.
* **`v-memoria`**: utiliza estructuras de datos en memoria para almacenar la información.
* **`v-postgres`**: utiliza PostgreSQL como sistema de almacenamiento persistente.

## Objetivos

* Desarrollar una API REST utilizando FastAPI.
* Implementar diferentes mecanismos de almacenamiento.
* Practicar el manejo de ramas y versiones con Git.
* Separar el código de acuerdo con las diferentes implementaciones del proyecto.
* Facilitar las pruebas y documentación de los diferentes endpoints de la API.

## Tecnologías utilizadas

* **Python** — Lenguaje principal de programación.
* **FastAPI** — Framework utilizado para desarrollar la API REST.
* **Uvicorn** — Servidor utilizado para ejecutar la aplicación.
* **Git** — Sistema de control de versiones.
* **GitHub** — Plataforma para alojar y gestionar el repositorio.
* **PostgreSQL** — Sistema de gestión de bases de datos utilizado en la rama `v-postgres`.

## Estructura del proyecto

```text
proyecto_python/
│
├── app/
│   ├── main.py
│   └── ...
│
├── tests/
│   └── ...
│
├── .gitignore
├── README.md
└── requirements.txt
```

## Instalación

### 1. Clonar el repositorio

```bash
git clone URL_DEL_REPOSITORIO
```

### 2. Ingresar al proyecto

```bash
cd proyecto_python
```

### 3. Crear el entorno virtual

```bash
python -m venv .venv
```

### 4. Activar el entorno virtual

En Windows utilizando Git Bash:

```bash
source .venv/Scripts/activate
```

En PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

### 5. Instalar las dependencias

```bash
pip install -r requirements.txt
```

## Ejecución

Para iniciar el servidor de desarrollo:

```bash
fastapi dev app/main.py
```

También se puede ejecutar mediante Python:

```bash
python -m fastapi dev app/main.py
```

Una vez iniciado el servidor, la aplicación estará disponible en:

```text
http://127.0.0.1:8000
```

## Ramas del proyecto

### `main`

Contiene la versión principal y estable del proyecto. Esta rama sirve como base para las diferentes implementaciones.

### `v-memoria`

Implementa el almacenamiento de los datos **directamente en memoria**, utilizando estructuras de datos propias de Python.

Esta versión permite trabajar con la información sin utilizar una base de datos externa.

### `v-postgres`

Implementa el almacenamiento **persistente mediante PostgreSQL**.

Esta versión permite conservar la información en una base de datos y trabajar con un sistema de almacenamiento más adecuado para un entorno de producción.

## Documentación de la API

FastAPI genera automáticamente documentación interactiva para consultar y probar los endpoints de la aplicación.

### Swagger UI

```text
http://127.0.0.1:8000/docs
```

### ReDoc

```text
http://127.0.0.1:8000/redoc
```

## Control de versiones

El proyecto utiliza **Git** para controlar los cambios y mantener diferentes versiones mediante ramas.

```text
main
├── v-memoria
└── v-postgres
```

Cada rama representa una implementación diferente del sistema, permitiendo desarrollar y probar las funcionalidades de manera independiente.

## Autor

Proyecto desarrollado como parte del proceso de formación en **ADSO — Análisis y Desarrollo de Software del SENA**.
