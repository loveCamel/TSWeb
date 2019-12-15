# TSWeb | TypeScript + Webpack |
Стартовое окружение разработчика для работы с TypeScript и less.
Инструмент сборки: Webpack

Состав окружения
--
- #####TypeScript
- #####TSLinter
- #####Babel + Plugins
- #####Less
- #####PostCss
- ###### and other optimizations
Для разработки с данным окружением рекомендуется использовать VS Code

Установка
--
Необходимые инструменты: 
[node.js](https://nodejs.org)

Что бы убедиться, что у вас установлен node.js, выполните команду:

`$ node -v`

Терминал должен отобразить вашу версию node.js, например:

`$ v10.15.0`

Если у вас в терминале вылезла ошибка, установите node.js

#####Если node.js установлен, склонируйте репозитрий и установите необходимые зависимости

Для клонирования репозитория вы можете воспользоваться командой 
(если установлен git):

`$ git clone https://github.com/loveCamel/TSWeb`

Для установки зависимостей наберите:

`$ npm i`

Готово.

Команды
--
- npm run dev - Запускает веб сервер и режим разработки.

- npm run build - Запускает сборку проекта со всеми оптимизациями. 
Проект будет собран в папку dist

- npm run lint - Запускает проверку TSLint. 
Результат будет записан в файл '_tslint_logs.txt' в корневой директории проекта.

Статические файлы (картинки, шрифты и т.д)
--
Все статические файлы хранятся в "src/assets"

#####Структура папки assets:

- fonts/ - папка с шрифтами
- img/ - папка с изображениями
- less/ - папка с less файлами
- libs/ - папка с сторонними библиотеками
- static/ - папка с файлами, которые будут перенесены в корень проекта "dist/".

После команды `npm run build` все папки из "src/assets/" будут копированы в директорию "dist/assets/"
Кроме папки "static/". Содержимое этой папки будет скопированно в корень директории сборки "dist/"