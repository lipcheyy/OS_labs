# Лабораторна робота №3
## **Docker.**
<br>
Виконав студент 2 курсу <br>
ФІТ ІПЗ-1.2 <br>
Липчей Владислав Васильович

&nbsp;
### **Використання готових Docker Images.**
Для початку я зайшов на сайт Dockerhub, де знайшов офіційний образ wordpress, та встановив собі цей образ командою
```
    docker pull wordpress
```

Далі я створив файл docker-compose.yml, в який я вставив стек з сайту
![](img/docker-compose.jpg)

Наступним кроком було зробити пул

![](img/wordpressPull.jpg)
Тепер можна відкривати localhost на порті 8080, який вказаний в стеку, і бачити результат:
![](img/wordpressPage.jpg)

![](img/wordpressPage2.jpg)
&nbsp;
### **Створення HTML сторінки та занесення її в Docker Image. Залити даний Docker Image на Docker Hub.**

- Створити HTML сторінку із вашим ПІБ, групою та № Л.Р..
- Створити Docker Image із цією сторінкою.
- Реалізувати можливість запуску цієї сторінки з контейнера (потрібно sudo usermod -aG docker username сервер NGINX до прикладу). 
- Перевірити на працездатність контейнера на основі вашого образу. 
- Залити готовий образ на Docker Hub.

Для цього нам потрібні 2 файли:
 - index.html
 - Dockerfile

вмістиме Dockerfile:
    
        FROM nginx:alpine
        COPY . /usr/share/nginx/html
Далі створюємо образ labwork і розгортаємо його на порті 8080

![](img/htmlBuild.jpg)

Результат

![](img/res.jpg)

**Заливаємо образ на dockerhub**

Для початку я створю пустий репозиторій 


![](img/dockerHub.jpg)

Далі пушу на віддалений репозиторій

![](img/dockerPush.jpg)
