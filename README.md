# Task at Rubyroid Labs Course

Необходимо написать утилиту `gemfiler`, которая будет показывать отфильтрованные версии гемов. 

Входные параметры: 
* Имя gem'а
* Указание версий в формате, совместимом с Gemfile

Вывод на консоль:
* Все версии данной библиотеки, при этом красным цветом подсвечиваются отфильтрованные версии.

Требования:
* Утилита должна парсить входные параметры с использованием существующих библиотек.
* Все версии gem'ов должны браться путем парсинга страницы или через взаимодействите с rubygems API
* Утилита должна быть поделена на независимые модули, каждый должен быть представлен отдельным классом.
* Правильная обработка потока ошибок.

Примеры:
```
./gemfiler devise '~> 2.1.3'
./gemfiler rails '>= 3.1'
./gemfiler rails '>= 3.1' '< 4.0'
```