##  Implement  tailwindcss

1.tailwindcssをpipenvにインストール(pipenv installで多分入ってる)
```
python -m pip install django-tailwind
```

2.`settings.py`のINSTALLED_APPSに`tailwind`を追加

3.Djangoアプリを作成する(APP名 : `CREATE_APP_NAME`
```
python manage.py tailwind init CREATE_APP_NAME
```

4.新しく作った`CREATE_APP_NAME`を`settings.py`のINSTALLED_APPSに追加

5.`settings.py`に以下を追加
```
TAILWIND_APP_NAME = 'CREATE_APP_NAME'
```

6.tailwindcssに必要な全ての依存関係をインストール
```
python manage.py tailwind install
```

7.普段通りに実行
```
python manage.py runserver
```

1. CSSの製品版をビルド???
```
python manage.py tailwind build
```

(django-tailwind pypi.org)[https://pypi.org/project/django-tailwind/]
