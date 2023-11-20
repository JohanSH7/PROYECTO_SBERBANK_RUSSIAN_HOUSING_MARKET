# Mechanisms of Action (MoA) Prediction
+ **Objetivo:** Desarrollar y optimizar modelos predictivos y no supervisados para la clasificación de las respuestas a los mecanismos de acción (MoA) de diferentes compuestos en muestras biológicas.

+ **Integrante:** Johan Sebastian Henao Cañas | C.C. 1000085432 | Ingenieria de Sistemas.

## Dataset
Los datos del proyecto actual provienen de una competición de Kaggle llamada [**Mechanisms of Action (MoA) Prediction**](https://www.kaggle.com/competitions/lish-moa/data). Se puede acceder a los datos ejecutando los siguientes comandos desde cualquier notebook:
```
# Instalar la librería necesaria
!pip install gdown

# Definir el enlace compartido de Google Drive (carpeta)
enlace_carpeta = "https://drive.google.com/drive/folders/1Xgn2u3v0Iun0kdn5NSeuE_5SlaxG4FTO?usp=sharing"

# Listar los archivos dentro de la carpeta
archivos_en_carpeta = [
    "train_drug.csv",
    "train_features.csv",
    "train_targets_scored.csv",
]
# Descargar cada archivo de la carpeta
import gdown
for archivo in archivos_en_carpeta:
    # Construir el enlace de descarga directa
    enlace_descarga = f"{enlace_carpeta}/{archivo}"

    # Descargar el archivo
    gdown.download(enlace_descarga, output=archivo, quiet=False)
```

## Información notebook
