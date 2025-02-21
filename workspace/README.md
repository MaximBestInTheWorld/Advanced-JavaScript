# «Рабочее окружение»

## Кейс 1. npm package
Я решил организовать разработку игры с использованием правильных инструментов, а именно что проект нужно создавать с помощью `npm`, управлять зависимостями и сборкой тоже с его помощью. 

### Процесс реализации
Создал GitHub-проект, после чего с помощью `npm init` сгенерировал package:
1. package name - defender-game
1. version - 1.0.0
1. description - "Browser based game"
1. entry point - index.js
1. test command - оставьте пустым
1. git repository - URL вашего GitHub репозитория 
1. keywords - game
1. author - ваше имя или псевдоним
1. license - ISC

Добавил [`.gitignore`](../.gitignore).

---

## Кейс 2. Babel
Подключил Babel к проекту и настроить сборку с его использованием.

### Процесс реализации
1. Установил Babel (`npm install --save-dev @babel/core @babel/cli @babel/preset-env`).
2. Установил CoreJS (`npm install core-js@3`).

2. Настроил скрипт запуска `build` для сборки с помощью `npm`.
3. Создал конфиг `babel.config.json` и прописал `@babel/preset-env`
4. Создал файл `src/app.js`
5. Удостоверился, что проект собирается, если в консоли запустить команду `npm run build`, и в каталоге `dist` формируется преобразованный Babel код.
6. Добавил каталог `dist` в `.gitignore`.
