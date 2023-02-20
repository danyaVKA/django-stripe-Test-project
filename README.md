# Django Stripe Test Project

Решение тестового задания Stripe с Django
В ходе работы удалось реализовать базовый Stripe api с успешной тестовой (локальной) оплатой по карте с отправкой логов 
в аккаунт Stripe.

При тестировании проекта необходимо ввести в djstriptest/setting.py:
- STRIPE_PUBLIC_KEY
- STRIPE_SECRET_KEY


## О проекте

В проекте использовались Python последней версии (3.11.2) с пакетами:

 - asgiref==3.3.1
 - certifi==2020.12.5
 - chardet==4.0.0
 - Django==3.1.6
 - idna==2.10
 - pytz==2021.1
 - requests==2.25.1
 - sqlparse==0.4.1
 - stripe==2.55.2
 - urllib3==1.26.3

Также для упрощения задачи используется виртуальное окружения, с уже установленными пакетами.

## Installation

Start virtualenv from command line:

```sh
path\venv\Scripts\activate.ps1
```
Setting Django admin:
```sh
python manage.py createsuperuser
login:
password:
python manage.py migrate
```



## Запуск проекта

Для успешной работы неоходимо после запуска сервера Django:

```sh
python manage.py runserver
```

Пройти по адресу:
```sh
127.0.0.1/8000/admin
```
Вести логин и пароль суперпользователя и добавить Test Product, установив цену 2000.

Пройти по адресу:
```sh
127.0.0.1/8000
```

Ввести данные карты (Тестовые данные с Stripe):

![card_1.png](readme_view%2Fcard_1.png)

![card_2.png](readme_view%2Fcard_2.png)

![card_3.png](readme_view%2Fcard_3.png)

![success.png](readme_view%2Fsuccess.png)

Демострация успешной тестовой оплаты:

![Stripe_site.png](readme_view%2FStripe_site.png)