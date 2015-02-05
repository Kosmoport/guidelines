###Kosmoport Styleguide — CSS (SCSS)
При написании/компилировании css используются:

 * SCSS (node-sass || libsass) 
 * Autoprefixer с конфигом: `> 5%, last 2 versions, Firefox ESR, Opera 12.1`
 * CSScomb
 
Файл `styles/styles.scss` комилируется в `css/styles.min.css` с картой кода.

### Организация файлов

### SCSS
Структура `styles.scss`

* В первую очередь подключаем `reset.scss` для сброса стилей.
* Файл `vars.scss` содержит все переменные которые будут использоваться в проекте
* `fonts.scss` для подключаемых шрифтов
* `helpers.scss` содержит нужные в проекте миксины и грид
* Папка `blocks` включает в себя стили которые относятся к определенным блокам проекта, а так же `_icon.scss` и `_button.scss`
Пример SCSS файла
```scss
@import 'reset';

@import 'vars';
@import 'fonts';

@import 'helpers';

@import 'blocks/button';
@import 'blocks/icons';

@import 'blocks/footer';
@import 'blocks/header';
```

