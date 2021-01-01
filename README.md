# DirModel

****************************

A program written in QT c++ to view the tree of a given directory.

<img src="https://raw.githubusercontent.com/maximalisimus/DirModel/main/image/dm-src-mage.png"  height="400">

## Оглавление

1. [Компиляция](#Компиляция)
2. [cqtdeployer](#cqtdeployer)
3. [About](#About)

[:arrow_up:Компиляция](#Компиляция)

Для компиляции приложения воспользуйтесь следующими командами:

```
	$ cd src/DirModel
	
	$ qmake
	
	$ make
```

[:arrow_up:cqtdeployer](#cqtdeployer)

Для того, чтобы независеть от наличия в вашей системе библиотек QT и беспрепятственно пользоваться программой, вопспользуйтесь специальной утилитой сборки библиотек - cqtdeployer.

**Команды для Linux:**

```
	cqtdeployer -bin myApp -qmake /media/D/Qt/6.0.0/gcc_64/bin/qmake -qmlDir ./
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

[:arrow_up:About](#About)

Версия программы 1.0, написана на языке C++ с использованием элементов QT.
Автор программы maximalisimus.
