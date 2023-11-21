# Mechanisms of Action (MoA) Prediction
+ **Objetivo:** Desarrollar y optimizar modelos predictivos y no supervisados para la clasificación de las respuestas a los mecanismos de acción (MoA) de diferentes compuestos en muestras biológicas.

+ **Integrante:** Johan Sebastian Henao Cañas | C.C. 1000085432 | Ingenieria de Sistemas.

## Dataset
Los datos del proyecto actual provienen de una competición de Kaggle llamada [**Mechanisms of Action (MoA) Prediction**](https://www.kaggle.com/competitions/lish-moa/data). Se puede acceder a los datos ejecutando los siguientes comandos desde cualquier notebook:
```
# Enlaces directos a los archivos en Google Drive
urls = {
    'train_targets_scored': 'https://drive.google.com/uc?id=12majHautYikmbSBlN1qNyzlkp076rFc2',
    'train_features': 'https://drive.google.com/uc?id=1XKVyJT3LRgYXozASXo6WT0WNPhktfvaa',
    'test_features': 'https://drive.google.com/uc?id=1R2tc7jX5Vrt74XF9Gpeo6UAjrO06DXmn'
}

# Descargar y leer cada archivo
dfs = {}
for name, url in urls.items():
    output = f"{name}.csv"
    gdown.download(url, output, quiet=False)
    dfs[name] = pd.read_csv(output)

# Ahora dfs contiene los DataFrames correspondientes a cada archivo
Y = dfs['train_targets_scored']
X = dfs['train_features']
test = dfs['test_features']
```

## Información notebook
