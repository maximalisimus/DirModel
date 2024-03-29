# DirModel

****************************

Программа для просмотра дерева заданной директории.

<img src="https://raw.githubusercontent.com/maximalisimus/DirModel/main/image/DirModel-v.1.1-screenshot.png"  height="400">

<a name="Oglavlenie"></a>

## Оглавление

1. [Компиляция](#Компиляция)
2. [cqtdeployer](#cqtdeployer)
3. [Использование](#Использование)
4. [About](#About)

## <a name="Компиляция">Компиляция</a>

Для компиляции приложения с помощью qmake воспользуйтесь следующими командами:

```
	$ cd src/DirModel
	
	$ qmake
	
	$ make
```

А для компиляции приложения с помощью cmake вот этими:

```
	$ cd src/DirModel
	
	$ mkdir build
	
	$ cd build
	
	$ cmake -G "Unix Makefiles" ..
	
	$ make

```

---

[К оглавлению](#Oglavlenie)

## <a name="cqtdeployer">cqtdeployer</a>

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

---

[К оглавлению](#Oglavlenie)

## <a name="Использование">Использование</a>

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

---

[К оглавлению](#Oglavlenie)

## <a name="About">About</a>

Версия программы 1.1, написана на языке C++ с использованием элементов QT.

Автор программы: [maximalisimus](https://github.com/maximalisimus).
