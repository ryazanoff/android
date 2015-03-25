##Intent
Намерения - позволяют запускать различные компоненты - фотографии, отправить письмо, браузер, звонок. Наиболее распространенный
вариант - запуск другой активности
Бывают двух типов - явные (Explicit) и неявные (Implicit)

###Явные
```java
Intent intent = new Intent(HelloWorld.this, AboutActivity.class);
startActivity(intent);
```
Первый параметр - *Context*. Activity является подклассом Context. 
Вкратце, Context – это объект, который предоставляет доступ к базовым функциям приложения таким как: доступ к ресурсам, к файловой системе, вызов Activiy и т.д. 
Второй параметр - имя класса. Система, просмотрев манифест определит, что нам нужно запустить новое активити. 
[https://lh4.googleusercontent.com/-zJcXjNOv0wk/Ton0Jh7sU4I/AAAAAAAAAa4/8j80xc1nbGM/s800/20111003_L0022_L_ExplicitIntent.jpg]()

###Неявные
[https://lh4.googleusercontent.com/-uLJgLPXCzOg/Ton0Jjr0CZI/AAAAAAAAAa8/ThvAvfrju1g/s800/20111003_L0022_L_ImplicitIntent.jpg]()


http://startandroid.ru/ru/uroki/vse-uroki-spiskom/59-urok-22-intent-intent-filter-context-teorija.html
http://developer.alexanderklimov.ru/android/theory/intent.php

[http://startandroid.ru/ru/uroki/vse-uroki-spiskom/70-urok-31-zachem-u-intent-est-atribut-data-chto-takoe-uri-vyzyvaem-sistemnye-prilozhenija.html](Что такое URI и зачем это нужно)

