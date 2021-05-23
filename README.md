# Start temptate Gulp4

Я собрал этот стартовый шаблон для обеспечения быстрого старта верстки и продакш-сброрки интернет-проекта под заказ по предоставленному Figma- или PSD-макету. В качестве сборщика использую Gulp 4. Реализована возможность создания критического css. Реализована возможность конвертации изображений в формате .jpg и .png в современный формат изображений webp.

К стартовому шаблону присоединил современную версию normalize. В файле grid.css реализована возможность использования двух сеток bootstrap 4 и bootstrap 5. Пл умолчанию включена возможность верстки по сетке bootstrap 5.
Ширина контентного контейнера для настольной версии шаблона составляет 1320px.


К макету по умолчанию присоединил:
jQuery v3.3.1
jquery.PageScroll2id v1.5.8
Magnific Popup v1.1.0
Owl Carousel v2.3.4
jquery.nicescroll v3.7.6
font-awesome-4.7.0

Чтобы подключить/отключить другие плагины, фрейворки и так далее к шаблоны откройте файлы:

```
scss/_libs.scss
gulpfile.js
```

Этот стартовый шаблон предназначен для сборки HTML5 шаблонов любой сложности с помощью Gulp4. Макет подготовлен к адаптивной верстке шаблона.

Стартовый шаблон ничем не перегружен и способен только собрать стили и скрипты в один файл соответственно, собрать продакт-версию для размещения сверстанного шаблона на хостинг.

### Как установить стартовый шаблон

Установите nodejs с поддержкой npm [https://nodejs.org/en/](https://nodejs.org/en/)
Установите git bash, если вы не используете консоль и они не установлена на компьютере под управлением Windows 10 [gitforwindows](https://gitforwindows.org/)

Установите gulp глобально. Эта операция выполняется только один раз на установленную операционную систему. Для этого в консоли пропишите команду

```
npm install gulp-cli -g
```

Чтобы узнать какая версия Gulp установлена, пропишите команду

```
gulp -v
```

На момент написания этой инструкции получил следующий ответ

```
CLI version 2.0.1
Local version 4.0.0
```

Чтобы узнать какая версия nodejs установлена, пропишите команду

```
node -v
```

Чтобы узнать какие пакеты и версии пакетов npm установлены, пропишите команду

```
npm list -g --depth=0
```

Разархивируйте скачанный стартовый пакет шаблона, переместите его в каталог, в котором будет выполняться вся разработка. Откройте его в консоли. Пропишите команду

```
npm i
```

Будет выполняться установка всех модулей Gulp.

### Как запустить сборку шаблона

После завершения установки пропишите помаду для запуска сервера:

```
gulp
```

Через минуту автоматически запуститься сервер и в браузере откроется главная страница сайта. Необходимо открыть файлы и выпоолнять верстку шаблона.

каталог sass - прописывать стили для оформления шаблона
каталог libs/common.js - прописывать стили для оформления шаблона
index.html - верстка шаблона

Если есть необходимость установить плагины jQuery, все каталоги разместите в калалоге libs.
Чтобы подключить js-файлы прописывать путь к ним в файле gulpfile.js
Чтобы подключить файлы css, пропишите пути к ним в файле app/scss/_ libs.scss

### Финальная сборка шаблона

В консоли наберите команду

```
gulp build
```

### Создание критического css

В консоли наберите команду

```
gulp criticalcss
```
### Конвертация изображений в webp

В консоли наберите команду

```
gulp towebp
```

Все полученные изображения в новом формате помещаются в каталог с исходными изображениями.

### Размещение шаблона на хостинг

Отредактируйте таск ftp. Вставьте реальные данные полученные в письме:

```
		host:     'vh210.timeweb.ru',
		user:     'cw25156',
		password: '2qzRb2Wo2zjm',
```
Отредактируйте путь к корневой папке сайта, в нее будут размещаться файлы разрабатываемого шаблона:
```
.pipe( conn.dest( '/public_html' ) );
```

В консоли наберите команду

```
gulp ftp
```

## Все наявные точки излома для адаптации под все мобильные устройства:

    1920 базовая точка
    1680 дополнительная точка
1.  1440 основная точка
2.  1336 основная точка
    1280 дополнительная точка
3.  1200 основная точка
4.  1190 основная точка
5.  1080 основная точка
6.  1024 основная точка
7.   992 основная точка
8.   980 основная точка 
     834 дополнительная точка
     812 дополнительная точка
9.   815 основная точка
10.  800 основная точка
11.  768 основная точка 
12.  740 основная точка
13.  736 основная точка
     734 дополнительная точка
     684 дополнительная точка
14.  667 основная точка
     640 дополнительная точка
15.  600 основная точка 
16.  568 основная точка
17.  480 основная точка
18.  425 основная точка
19.  414 основная точка
     412 дополнительная точка
20.  387 основная точка
21.  384 основная точка
     375 дополнительная точка
22.  360 основная точка
23.  320 основная точка

## Контроль за качеством кода

По умолчанию выполнена настройка линтинга или контроля за качеством кода в процессе вертски и програмирования. 

В сборке уже установлены и настроены такие инструменты:

* Eslint
* Prettier
* Stylelint
  
Чтобы эти инструменты используйте IDE VSCode и установите плагины:

* Prettier - Code formatter
* ESLint | Dirk Baeumer
* vscode-stylelint

## Связаться по вопросам создания сайта под ключ:
<br>

[![facebook](https://img.shields.io/badge/-Facebook-1877F2?style=for-the-badge&logo=Figma&logoColor=eeffff)](https://www.facebook.com/frontendercode)
[![Telegram](https://img.shields.io/badge/-Telegram-26A5E4?style=for-the-badge&logo=Telegram&logoColor=eeffff)](https://t.me/frontendcoder)
[![Instagram](https://img.shields.io/badge/-Instagram-E4405F?style=for-the-badge&logo=Instagram&logoColor=eeffff)](https://www.instagram.com/frontendercode/?hl=ru)
[![GitHub](https://img.shields.io/badge/-GitHub-181717?style=for-the-badge&logo=GitHub&logoColor=eeffff)](https://github.com/frontend-coder)



[![Portfolio](https://img.shields.io/badge/-Портфолио-181717?style=for-the-badge&logo=Internet-Archive&logoColor=eeffff)](https://frontend-coder.github.io)
