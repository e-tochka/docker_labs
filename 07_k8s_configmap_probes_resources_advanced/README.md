# Преподготовка

![0-1](img/0-1.png)

[base.yaml](pods/base.yaml)

![0-2](img/0-2.png)

![0-3](img/0-3.png)

# Часть 1. Обновление ConfigMap и применение новой конфигурации

![1-1](img/1-1.png)

![1-2](img/1-2.png)

![1-3](img/1-3.png)

![1-4](img/1-4.png)

![1-5](img/1-5.png)

# Часть 2. Startup probe и медленный старт приложения

[slow-start.yaml](pods/slow-start.yaml)

![2-1](img/2-1.png)

![2-2](img/2-2.png)

# Часть 3. Ошибка liveness probe и перезапуски контейнера

[liveness-probe.yaml](pods/liveness-probe.yaml)

![3-1](img/3-1.png)

# Часть 4. Слишком маленький memory limit и OOMKilled

[oom.yaml](pods/oom.yaml)

![4-1](img/4-1.png)

# ЧАСТЬ 5. CPU LIMIT И ДЕГРАДАЦИЯ

[cpu.yaml](pods/cpu.yaml)

![5-1](img/5-1.png)

# Часть 6. Pod Pending из-за завышенных requests

[pending.yaml](pods/pending.yaml)

![6-1](img/6-1.png)

# Часть 7. Сравнение трех состояний: NotReady, CrashLoopBackOff, Pending

| Состояние        | Когда возникает                           | Основной симптом          | Где смотреть причину |
| ---------------- | ----------------------------------------- | ------------------------- | -------------------- |
| NotReady         | Приложение не отвечает, probe не проходит | Pod Running, но 0/1 READY | describe pod, events |
| CrashLoopBackOff | Падает контейнер, liveness убивает        | Постоянные рестарты       | describe pod, logs   |
| Pending          | Не хватает ресурсов на ноде               | Pod не стартует           | describe pod, events |
