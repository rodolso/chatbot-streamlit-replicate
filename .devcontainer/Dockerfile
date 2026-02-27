FROM python:3.12-slim

WORKDIR /workspace

# Instalar dependencias del sistema necesarias para compilación
RUN apt-get update && apt-get install -y --no-install-recommends \
    git \
    curl \
    && rm -rf /var/lib/apt/lists/*

# Copiar e instalar dependencias de Python
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Kernel de Python para los notebooks del workshop en VS Code
RUN pip install --no-cache-dir ipykernel
