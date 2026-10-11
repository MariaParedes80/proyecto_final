# 🎓 Proyecto Universitario: Interfaz de IA Resiliente con Streamlit

Este proyecto implementa una aplicación web local que integra un modelo de lenguaje de Meta AI con un conjunto de datos, utilizando una arquitectura preparada para tolerar fallos de infraestructura.

---

## 🛠️ 1. Requisitos del Sistema
* **Versión de Python:** Python 3.10 o superior (Recomendado Python 3.11).
* **Servidor de Modelos:** Ollama instalado y activo.
* **Modelo Utilizado:** `llama3.2:3b` (~2.0 GB de peso en disco).

---

## 🚀 2. Configuración del Entorno Local

Siga estos comandos en orden secuencial dentro de su terminal para clonar el repositorio y levantar el entorno:

```bash
# 1. Clonar el repositorio
git clone https://github.com
cd TU_REPOSITORIO

# 2. Creación del entorno virtual aislado
python -m venv env

# 3. Activación del entorno virtual
# En Windows (PowerShell):
.\env\Scripts\Activate.ps1
# En Windows (CMD clásico):
.\env\Scripts\activate.bat
# En macOS / Linux:
source env/bin/activate

# 4. Actualizar el gestor de paquetes e instalar dependencias
pip install --upgrade pip
pip install -r requirements.txt
```

---

## 🦙 3. Configuración de Ollama y Descarga del Modelo

1. Descargue e instale la aplicación correspondiente a su sistema operativo desde [ollama.com](https://ollama.com).
2. Ejecute la aplicación Ollama (asegúrese de ver su icono en la barra de tareas).
3. Abra una terminal en su sistema y ejecute el comando de aprovisionamiento:
   ```bash
   ollama pull llama3.2:3b
   ```

---

## 📊 4. Obtención y Ubicación del Dataset

Para que la aplicación funcione correctamente con los datos solicitados:
* El archivo de datos debe llamarse **`dataset.csv`**.
* Debe estar ubicado obligatoriamente dentro de la carpeta llamada **`data`** en la raíz del proyecto.
* Si el archivo no existe en la ruta `./data/dataset.csv`, la aplicación de Streamlit mostrará una alerta controlada en pantalla indicándole al usuario que debe colocar el archivo allí.

---

## 💻 5. Ejecución de la Aplicación

Con el entorno virtual activado (`env`) y Ollama corriendo en segundo plano, ejecute:

```bash
streamlit run app.py
```

La aplicación se desplegará automáticamente en su navegador web en la dirección local `http://localhost:8501`.