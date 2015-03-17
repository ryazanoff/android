Gradle, Manifest. Класс Activity и его жизненный цикл. Структура xml файлов. layout.xml файлы Activity. 
Класс View и элементы Layout: TextView, Button, EditText ... Layout-group: LinearLayout, RelativeLayout. 
Относительное/абсолютное задание размеров элементов. Обработчики нажатия.

##Gradle
Система автоматической сборки приложений. Не является особенностью Android, была возможность установить и на Java, но в Android
Studio стала обязательной. 

Как правило существует 2 файла build.gradle - для проекта и для модуля. Нас интересует для модуля. 

Добавление библиотеки происходит следующим образом

dependencies {
    compile 'com.squareup.picasso:picasso:2.3.2'
}

Так же тут прописываются некоторые параметры приложения - такие как номер версии и версии андроида. Так же Gradle мы будем 
использовать для релиза приложения. Когда в градле что-то меняется необходимо синхронизовать проект.

##Manifest
Манифест нужен для задания некоторых настроек и параметров приложения. Например:
  1. объявляет имя Java-пакета приложения, который служит уникальным идентификатором;
  2. описывает компоненты приложения — деятельности, службы, приемники широковещательных намерений и контент-провайдеры, что позволяет вызывать классы, которые реализуют каждый из компонентов, и объявляет их намерения
  3. ссодержит список необходимых разрешений для обращения к защищенным частям API и взаимодействия с другими приложениями;
  4. объявляет разрешения, которые сторонние приложения обязаны иметь для взаимодействия с компонентами данного приложения;

Общая структура манифеста:

```xml
<?xml version="1.0" encoding="utf-8"?>

<manifest>

    <uses-permission />
    <permission />
    <permission-tree />
    <permission-group />
    <instrumentation />
    <uses-sdk />
    <uses-configuration />  
    <uses-feature />  
    <supports-screens />  
    <compatible-screens />  
    <supports-gl-texture />  

    <application>

        <activity>
            <intent-filter>
                <action />
                <category />
                <data />
            </intent-filter>
            <meta-data />
        </activity>

        <activity-alias>
            <intent-filter> . . . </intent-filter>
            <meta-data />
        </activity-alias>

        <service>
            <intent-filter> . . . </intent-filter>
            <meta-data/>
        </service>

        <receiver>
            <intent-filter> . . . </intent-filter>
            <meta-data />
        </receiver>

        <provider>
            <grant-uri-permission />
            <meta-data />
            <path-permission />
        </provider>

        <uses-library />

    </application>

</manifest>
```


