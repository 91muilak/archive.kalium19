# Material Design Colors
Готовая палитра Material Design Colors в формате SASS-переменных.

- Используется `map-get` для получения переменных
- Переменные начинаются с приставки `mdc-`
- При ошибке используйте `@use "sass:map";` в начале файла стилей

## Пример использования
```scss
.text-error {
  color: map-get($mdc-red, 50);
  background: map-get($mdc-grey, 900);
}
```

### Существующие цвета
1. `red`
2. `pink`
3. `purple`
4. `deep-purple`
5. `indigo`
6. `blue`
7. `light-blue`
8. `cyan`
9. `teal`
10. `green`
11. `light-green`
12. `lime`
13. `yellow`
14. `amber`
15. `orange`
16. `deep-orange`
17. `brown`
18. `grey`
19. `blue-grey`

### Градации цветов
- 50
- 100
- 200
- 300
- 400
- 500
- 600
- 700
- 800
- 900
- A100
- A200
- A400
- A700

## Импорт и установка
Можно напрямую склонировать репозиторий и достать всё что нужно. Но также можно установить MDC в качестве Git Submodule командой:

```bash
git submodule add https://github.com/91muilak/material-design-colors to/path
```

### Импорт
Импорт выполняется через `@import` в SASS. Можно по отдельности подключить конкретный цвет, а можно подключить файл `_palette.scss`, в котором все импорты уже прописаны.

```scss
@import 'amber';
@import 'blue-grey';
@import 'blue';
@import 'brown';
@import 'cyan';
@import 'deep-orange';
@import 'deep-purple';
@import 'green';
@import 'grey';
@import 'indigo';
@import 'light-blue';
@import 'light-green';
@import 'lime';
@import 'orange';
@import 'pink';
@import 'purple';
@import 'red';
@import 'teal';
@import 'yellow';
```

> В Вашем случае путь к файлу может отличаться.