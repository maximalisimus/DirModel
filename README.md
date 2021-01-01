# DirModel

****************************

Программа для просмотра дерева заданной директории.

<img src="https://raw.githubusercontent.com/maximalisimus/DirModel/main/image/DirModel-v.1.1-screenshot.png"  height="400">

## Оглавление

1. [Компиляция](#Компиляция)
2. [cqtdeployer](#cqtdeployer)
3. [Использование](#Использование)
4. [About](#About)

[:arrow_up:Компиляция](#Компиляция)

Для компиляции приложения воспользуйтесь следующими командами:

```
	$ cd src/DirModel
	
	$ qmake
	
	$ make
```

[:arrow_up:cqtdeployer](#cqtdeployer)

Для того, чтобы не зависеть от наличия в вашей системе библиотек QT и беспрепятственно пользоваться программой, вопспользуйтесь специальной утилитой сборки библиотек - cqtdeployer.

**Команды для Linux:**

```
	cqtdeployer -bin myApp -qmake /usr/bin/qmake -qmlDir ./
```

**Команды для Windows:**

```
	cqtdeployer -bin myApp.exe -qmake C:\\Qt\Qt5.7.0\5.7\mingw53_32/bin\qmake.exe -qmlDir .
```

* cqtdeployer - это вызов утилиты. (до версии 1.4 в Windows использовалась команда %cqtdeployer%)
* -bin - флаг для передачи путей исполняемых файлов приложения.
* myApp.exe и myApp - сам путь к исполняемому файлу приложения
* -qmake - флаг для передачи путей к qmake для развертывания qt.
* -qmlDir - флаг для передачи путей к qml файлам приложения.

[:arrow_up:Использование](#Использование)

**Ключи и параметры программы:**
```
-d, --d, -dir, --dir, /d 		- Задание рабочей директории
-w, --w, /w, -width, --width 		- Размер окна программы по ширине
-h, --h, -height, --height 		- Размер окна программы по высоте
-s, --s, /s, -size, --size 		- Размер шрифта программы
-v, --v, /v, -version, --version 	- Версия
--help, -help, /?, ?, /h 		- Помощь
```

Программу можно использовать без параметров, тогда все параметры будут установлены по умолчанию, а путь к рабочей директории запрошен далее с помощью диалога выбора директории.
По умолчанию устанавливаются следующие параметры: 
* Размеры окна - 640x480
* Размер шрифта - 12px

[:arrow_up:About](#About)

Версия программы 1.0, написана на языке C++ с использованием элементов QT.

Автор программы: [maximalisimus](https://github.com/maximalisimus).
