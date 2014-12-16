VbaDeveloper
============

VbaDeveloper это надстройка (addin)  для MS Excel, которая позволяет импортирвать и экспортировать исходный код проектов на VBA.


Особенности
--------------

1. Автоэкспорт по сохранению:
    - классов
    - модулей
    - форм
    - etc.
2.  Пользовательское меню в ленте быстрого доступа, позволяющее
    - Сделать экспорт всех открытых проектов
    - Сделать импорт всех проектов из предустановленной директории
    - Сделать автоформатирование кода


Настройка окружения
------------------------------

Это всего лишь форк оригинального [проекта](https://github.com/hilkoc/vbaDeveloper), Вы можете самостоятельно собрать проект, используя [инструкции](https://github.com/hilkoc/vbaDeveloper/blob/master/src/vbaDeveloper.xlam/Build.bas). Но это форк был создан для хранения [собранного](https://github.com/mcgr0g/vbaDeveloper/releases/tag/v1.0) проекта, тем более со сборкой на [есть](https://github.com/hilkoc/vbaDeveloper/issues/1) сложности. Для того что бы его использовать вам потребуется:

 1. [Сохранить](https://github.com/mcgr0g/vbaDeveloper/releases/download/v1.0/vbaDeveloper.zip) `vbaDeveloper.xlam` к себе на локальную машину в
    директорию `C:\Users\%username%\AppData\Roaming\Microsoft\AddIns`
 2. Открыть Excel и на вкладке Разработчик добавить надстройку "Vbadeveloper"
 3. Сохранить проект, например с именем `C:\project\hardproj\okgo.xlsm` и закрыть Excel
 4. Заново открыть файл. При этом надстройка автоматически подключится о чем вам сообщит диалоговое окно.
 5. Файлы проекта  будут сохраняться в `src` директорию  рядом: `C:\project\hardproj\src\okgo.xlsm\`. При этом `okgo.xlsm\` это  поддиректория src.