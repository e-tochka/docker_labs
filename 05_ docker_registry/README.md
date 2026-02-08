# 1 Поднимите локальный registry

Поднимаем контейнер:
![5-1](imgs/5-1.png)

Проверяем:
![5-2](imgs/5-2.png)

# 2 Проверка registry по API
![5-3](imgs/5-3.png)

# 3 Подготовьте мини-проект
![5-4](imgs/5-4.png)
index.html:
![5-5](imgs/5-5.png)

deckerfile:
![5-6](imgs/5-6.png)

# 4 Сборка образа
запускаем:
![5-7](imgs/5-7.png)

Проверка:
![5-8](imgs/5-8.png)

# 5 Привязка образа к registry через tag
![5-9](imgs/5-9.png)
проверка:
![5-10](imgs/5-10.png)

# 6 Push в registry
![5-11](imgs/5-11.png)

# 7 Проверка, что образ реально в registry
Проверьте список репозиториев: curl `http://localhost:5000/v2/_catalog`

Ожидаемо: {"repositories":["web-demo-<ваш_логин>"]}
![5-12](imgs/5-12.png)

Проверьте список тегов: curl `http://localhost:5000/v2/web-demo-username/tags/list`

Ожидаемо: {"name":"web-demo-<ваш_логин>","tags":["1.0"]}
![5-13](imgs/5-13.png)

# 8 Проверка pull
Удаляю тег:
![5-14](imgs/5-14.png)

Пулю:
![5-15](imgs/5-15.png)

# 9 Проверка запуском контейнера
![5-16](imgs/5-16.png)

курлык:

![curl](imgs/curl.png)
![5-17](imgs/5-17.png)
сайт:
![5-18](imgs/5-18.png)

# 10 Самостоятельная часть
## 10.1 Версия 2.0
![translate](imgs/translate.png)

![5-19](imgs/5-19.png)

Пересобрал:
![5-20](imgs/5-20.png)

Привязка к registry:
![5-21](imgs/5-21.png)

Push:
![5-22](imgs/5-22.png)

проверка тега. Ожидаемый результат: `{"name":"web-demo-username","tags":["1.0","2.0"]}`
![5-23](imgs/5-23.png)


## 10.2 Второй запуск на другом порту