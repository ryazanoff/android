##Fragment
[Ман от гугла](http://developer.android.com/guide/components/fragments.html)

Fragment — модульная часть activity, у которой свой жизненный цикл и свои обработчики различных событий. Android добавил фрагменты с API 11, для того, чтобы разработчики могли разрабатывать более гибкие пользовательские интерфейсы на больших экранах, таких как экраны планшетов. Через некоторое время была написана библиотека, которая добавляет поддержку фрагментов в более старые версии. 

Плюсы по сравнению с использованием activity видны сразу:
С помощью них можно легко сделать дизайн адаптивный под планшеты
Разделение кода на функциональные модули, а следовательно поддержка кода обходится дешевле


Основные классы

Есть три основных класса:
android.app.Fragment — от него, собственно говоря. и будут наследоваться наши фрагменты
android.app.FragmentManager — с помощью экземпляра этого класса происходит все взаимодействие между фрагментами
android.app.FragmentTransaction — ну и этот класс, как понятно по названию, нужен для совершения транзакций.
В настоящее время появляются разновидности класса Fragment, для решения определенных задач — ListFragment, PreferenceFragment и др.


###Простой пример с фрагментом

Создаем 2 layout для фрагментов.

```xml
  <?xml version="1.0" encoding="utf-8"?>
  <LinearLayout
   xmlns:android="http://schemas.android.com/apk/res/android"
   android:layout_width="match_parent"
   android:layout_height="match_parent"
   android:background="#77ff0000"
   android:orientation="vertical">
  <TextView
   android:id="@+id/textView1"
   android:layout_width="wrap_content"
   android:layout_height="wrap_content"
   android:text="Fragment 1">
  </TextView>
  </LinearLayout>
```

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout
 xmlns:android="http://schemas.android.com/apk/res/android"
 android:layout_width="match_parent"
 android:layout_height="match_parent"
 android:background="#7700ff00"
 android:orientation="vertical">
<TextView
 android:id="@+id/textView2"
 android:layout_width="wrap_content"
 android:layout_height="wrap_content"
 android:text="Fragment 2">
</TextView>
</LinearLayout>
```
