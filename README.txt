Команды терминала

Установка:
npm i

Запуск режима разработчика (c запуском сервера)
npm run dev

Запуск сборки проекта (без запуска сервера, только финальная сборка)
npm run build

Запуск сборки проекта и выгрузка результата на сервер по FTP. (без запуска локальконо сервера)
Конфигурация FTP находится в файле ftp.js
npm run deploy

Запуск сборки проекта и создание zip архива с именем проекта. (без запуска локальконо сервера)
npm run zip




//------------------------------------------------------------------------------

Используются алиасы пути к папкам:
@img = src/img
@scss = src/scss
@js = src/js

Плагин для VS Code - Path Autocomplete
Настройки (Settings JSON):
"path-autocomplete.pathMappings": {
	"@img": "${folder}/src/img", // алиас для папки img
	"@scss": "${folder}/src/scss", // алиас для папки scss
	"@js": "${folder}/src/js", //  алиас для папки js
}



//------------------------------------------------------------------------------

Проблемы и их решения:
Ошибка del
Решение:
в терминале прописать npm i del@6
либо в package.json поменять версию "del": "6",
--------------------------------------
Ошибка node-sass.
Решения:
npm rebuild node-sass
и/или
npm install sass gulp-sass --save-dev
--------------------------------------
Ошибка Pyton
Решени:
npm install --global windows-build-tools
--------------------------------------