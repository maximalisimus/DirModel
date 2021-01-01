# DirModel

A program written in QT c++ to view the tree of a given directory.

## Оглавление

1. [Компиляция](#Компиляция)
2. [cqtdeployer](#cqtdeployer)
3. [About](#About)

[:arrow_up:Компиляция](#Компиляция)

Для компиляции приложения воспользуйтесь следующими командами:

```
	$ qmake
	
	$ make
```

[:arrow_up:cqtdeployer](#cqtdeployer)

Для того, чтобы независимо от наличия в вашей системе библиотек переносить программу, вопспользуйтесь специальной утилитой сборки библиотек - cqtdeployer.

**Linux:**
	```
		cqtdeployer -bin myApp -qmake /media/D/Qt/6.0.0/gcc_64/bin/qmake -qmlDir ./
	```

**Windows:**
	```
		cqtdeployer -bin myApp.exe -qmake /media/D/Qt/6.0.0/mingw810_64/bin/qmake.exe -qmlDir ./
	```

* cqtdeployer - это вызов утилиты. (до версии 1.4 в Windows использовалась команда %cqtdeployer%)
* -bin - флаг для передачи путей исполняемых файлов приложения.
* myApp.exe и myApp - сам путь к исполняемому файлу приложения
* -qmake - флаг для передачи путей к qmake для развертывания qt.
* -qmlDir - флаг для передачи путей к qml файлам приложения.

[:arrow_up:About](#About)

Версия программы 1.0, написана на языке C++ с использованием элементов QT.
Автор программы maximalisimus.
