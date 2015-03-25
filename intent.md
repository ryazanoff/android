##Intent
Намерения - позволяют запускать различные компоненты - фотографии, отправить письмо, браузер, звонок. Наиболее распространенный
вариант - запуск другой активности
Бывают двух типов - явные (Explicit) и неявные (Implicit)

###Явные
![Явные](https://lh4.googleusercontent.com/-zJcXjNOv0wk/Ton0Jh7sU4I/AAAAAAAAAa4/8j80xc1nbGM/s800/20111003_L0022_L_ExplicitIntent.jpg] "Явные")
```java
Intent intent = new Intent(HelloWorld.this, AboutActivity.class);
startActivity(intent);
```
Первый параметр - *Context*. Activity является подклассом Context. 
Вкратце, Context – это объект, который предоставляет доступ к базовым функциям приложения таким как: доступ к ресурсам, к файловой системе, вызов Activiy и т.д. 
Второй параметр - имя класса. Система, просмотрев манифест определит, что нам нужно запустить новое активити. 


###Неявные
![Неявные](https://lh4.googleusercontent.com/-uLJgLPXCzOg/Ton0Jjr0CZI/AAAAAAAAAa8/ThvAvfrju1g/s800/20111003_L0022_L_ImplicitIntent.jpg] "Неявные")


http://startandroid.ru/ru/uroki/vse-uroki-spiskom/59-urok-22-intent-intent-filter-context-teorija.html
http://developer.alexanderklimov.ru/android/theory/intent.php

[Что такое URI и зачем это нужно](http://startandroid.ru/ru/uroki/vse-uroki-spiskom/70-urok-31-zachem-u-intent-est-atribut-data-chto-takoe-uri-vyzyvaem-sistemnye-prilozhenija.html)

###Диалоги и т.д.
[Всплывающие окна](http://developer.alexanderklimov.ru/android/toast.php)

[АлертДиалоги](http://developer.alexanderklimov.ru/android/alertdialog.php)

[Создание кастомного диалога](http://stackoverflow.com/questions/13341560/how-to-create-a-custom-dialog-box-in-android)

[Ман от гугла](http://developer.android.com/guide/topics/ui/dialogs.html)

[Статья на хабре](http://habrahabr.ru/post/166469/)

###Меню
http://developer.alexanderklimov.ru/android/menu.php

###Темы и стили
http://habrahabr.ru/post/133307/

###9 patch
http://habrahabr.ru/post/113623/

http://romannurik.github.io/AndroidAssetStudio/nine-patches.html
