# Mechanisms of Action (MoA) Prediction
+ **Objetivo:** Desarrollar y optimizar modelos predictivos y no supervisados para la clasificación de las respuestas a los mecanismos de acción (MoA) de diferentes compuestos en muestras biológicas.

+ **Integrante:** Johan Sebastian Henao Cañas | C.C. 1000085432 | Ingenieria de Sistemas.

## Dataset
Los datos del proyecto actual provienen de una competición de Kaggle llamada [**Mechanisms of Action (MoA) Prediction**](https://www.kaggle.com/competitions/lish-moa/data). Se puede acceder a los datos ejecutando los siguientes comandos desde cualquier notebook:
```
# Enlaces directos a los archivos en Google Drive
urls = {
    'train': 'https://drive.google.com/uc?id=1dEP20pVQrKczTk1fbUk4g6WhUe4SOg00',
    'test': 'https://drive.google.com/uc?id=17uN_IpWH_L5Ou-cGguBoe-k8bqU9qCy6',
}

# Descargar y leer cada archivo
dfs = {}
for name, url in urls.items():
    output = f"{name}.csv"
    gdown.download(url, output, quiet=False)
    dfs[name] = pd.read_csv(output)

# Ahora las siguientes variables contienen los DataFrames correspondientes a cada archivo
X = dfs['train']
Test = dfs['test']
```

## Información notebook
