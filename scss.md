###Kosmoport Styleguide
Органицая файлов и форматирование кода от Kosmoport!
#css
При написании css используется Sass, Autoprefixer , Css Comp
###Организация файлов

###Scss
Структура [style.scss]
* В первую очередь подключаем [reset.scss] для сброса стилей.
* Файл [vars.scss] содержит все переменные которые будут использоваться в проекте
* [fonts.scss] для подключаемых шрифтов
* [helpers.scss] содержит нужные в проекте миксины и грид
* Папка blocks включает в себя стили которые относятся к определенным блокам проекта, а так же [icons.scss] и [buttons.scss]

```sh
@import 'reset';

@import 'vars';
@import 'fonts';

@import 'helpers';

@import 'blocks/button';
@import 'blocks/icons';

@import 'blocks/footer';
@import 'blocks/header';
```

