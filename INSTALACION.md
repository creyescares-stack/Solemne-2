# 🔧 Guía de Instalación

## Solución a Errores de Importación

Si ves errores como "No se ha podido resolver la importación 'streamlit'", significa que necesitas instalar las dependencias de Python.

## Pasos para Instalar

### 1. Abrir Terminal o Línea de Comandos

**Windows:**
- Presiona `Win + R`
- Escribe `cmd` y presiona Enter

**Mac/Linux:**
- Abre la aplicación Terminal

### 2. Navegar a la Carpeta del Proyecto

```bash
cd ruta/a/tu/proyecto
```

### 3. Instalar las Dependencias

```bash
pip install -r requirements.txt
```

O instalar manualmente cada paquete:

```bash
pip install streamlit==1.29.0
pip install pandas==2.1.4
pip install plotly==5.18.0
```

### 4. Verificar la Instalación

```bash
pip list
```

Deberías ver en la lista:
- streamlit
- pandas
- plotly

### 5. Ejecutar la Aplicación

```bash
streamlit run app.py
```

## Alternativa: Usar Entorno Virtual (Recomendado)

### Crear entorno virtual:

```bash
python -m venv venv
```

### Activar el entorno:

**Windows:**
```bash
venv\Scripts\activate
```

**Mac/Linux:**
```bash
source venv/bin/activate
```

### Instalar dependencias:

```bash
pip install -r requirements.txt
```

### Ejecutar aplicación:

```bash
streamlit run app.py
```

## Despliegue en Streamlit Cloud (Sin Instalación Local)

Si no quieres instalar nada localmente, puedes desplegar directamente en la nube:

1. Sube el proyecto a GitHub
2. Ve a [share.streamlit.io](https://share.streamlit.io)
3. Conecta tu repositorio
4. ¡Listo! Streamlit Cloud instalará todo automáticamente

## Problemas Comunes

### Error: "pip no se reconoce como comando"

Solución: Instala Python desde [python.org](https://python.org) y marca la opción "Add Python to PATH"

### Error: "Permission denied"

Solución en Mac/Linux: Usa `pip3` en lugar de `pip`
```bash
pip3 install -r requirements.txt
```

### Error de versión de Python

Este proyecto requiere Python 3.8 o superior. Verifica tu versión:
```bash
python --version
