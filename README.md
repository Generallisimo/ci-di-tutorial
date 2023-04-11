Для ci.cd мы установим банальные скрипты 
  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "build:storybook": "node ./scripts/storybook.js",
    "test:unit": "react-scripts test",
    "test:e2e": "node ./scripts/e2e.test.js",
    "lint": "node ./scripts/eslint.js",
    "type:check": "node ./scripts/typecheck.js",
    "i18n:check": "node ./scripts/i18n-check.js"
  },

npm install -g react-scripts

Дальше мы создадим папки и будем теститировать

Потом созд папку и файл где будут прописываться проверки для сайта
После push они будут показываться в action

после редактируем его на пул и пуш, так чтобы тесты были на проверку и заливаем новую ветку с ошибками, после проверки исправляемя и видим отличную работу ci/cd