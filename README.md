# Лабораторна робота №4
## **TERRAFORM**
<br>
Виконав студент 2 курсу <br>
ФІТ ІПЗ-1.2 <br>
Липчей Владислав Васильович

&nbsp;
### **Для початку налаштуємо облікові дані, виберемо свій проект, та cтворимо обліковий запис для служб**
![](img/1.jpg)
### **Вибираю роль project owner**
![](img/2.jpg)
### **Створюю ключ в форматі json та переношу його в папку з проектом**
![](img/3.jpg)
### **Перехожу в вкладку з образами віртуальних машин та включаю computing engines**
![](img/4.jpg)
### **В терраформ файлі я прописую свого провайдера, ключ облікових даних, створюю 2 ресурси і пудключаю АРІ googlecompute i cloudresourcemanager, такоє прописую те що ми будемо відкривати файли на портах 443 та 80 на дефолтній мережі**
![](img/8.jpg)
### **Тут я вказую тип віртуальної машини, та пишу скрипт для встановлення апач сервера та занесення даних в файл index.html**
![](img/9.jpg)
### **Ініціалізую терраформ в папці проекто та виконую terraform apply**
![](img/5.jpg)
### **Мій образ**
![](img/6.jpg)
### **Результат готова html сторінка**
![](img/7.jpg)




