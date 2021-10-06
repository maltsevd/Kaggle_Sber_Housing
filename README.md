Sberbank Russian Housing Market
https://www.kaggle.com/c/sberbank-russian-housing-market/data

### Клонируем репозиторий и создаем образ
```
$ git clone https://github.com/maltsevd/Kaggle_Sber_Housing.git
$ cd Kaggle_Sber_Housing
$ docker build -t maltsevd/kaggle_sber_housing .
```

### Запускаем контейнер

Здесь Вам нужно создать каталог локально и сохранить туда предобученную модель (<your_local_path_to_pretrained_models> нужно заменить на полный путь к этому каталогу)
```
$ docker run -d -p 8180:8180 -p -v <your_local_path_to_pretrained_models>:/app/app/models maltsevd/kaggle_sber_housing
```

### Переходим на localhost:8181
