[![Новости](https://img.shields.io/badge/объявления-277a8c?logo=github)](https://github.com/91muilak/kalium19/discussions/3)
[![Обсуждение](https://img.shields.io/badge/обсуждение-000000?logo=github)](https://github.com/91muilak/kalium19/discussions/4)


<img title="Логотип проекта" src=".github/logo.png" alt="Logo" width="100px" align="right" /> Kalium19 ![](https://img.shields.io/github/package-json/var/91muilak/kalium19?label=%20)
======
:package: Набор утилит, миксинов, расширений на языке препроцессора [SASS](https://github.com/sass) для помощи в ускорении и упрощении написания CSS-стилей.

![GitHub Repo stars](https://img.shields.io/github/stars/91muilak/kalium19?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/91muilak/kalium19?style=social)
![GitHub Forks](https://img.shields.io/github/forks/91muilak/kalium19?style=social)
![GitHub contributors](https://img.shields.io/github/contributors/91muilak/kalium19?style=social&logo=github)

![Последний коммит](https://img.shields.io/github/last-commit/91muilak/kalium19)
![Количество коммитов в год](https://img.shields.io/github/commit-activity/y/91muilak/kalium19)
![Последний релиз](https://img.shields.io/github/v/release/91muilak/kalium19)
![Дата последнего релиза](https://img.shields.io/github/release-date/91muilak/kalium19)
![Количество ЯП](https://img.shields.io/github/languages/count/91muilak/kalium19?color=fff)
![Топ ЯП](https://img.shields.io/github/languages/top/91muilak/kalium19?color=C76494)
![Размер репозитория](https://img.shields.io/github/repo-size/91muilak/kalium19?color=ffb600)
![Размер кода](https://img.shields.io/github/languages/code-size/91muilak/kalium19)
[![Количество открытых issue](https://img.shields.io/github/issues-raw/91muilak/kalium19)
![Количество закрытых issues](https://img.shields.io/github/issues-closed-raw/91muilak/kalium19?color=354a6d)](https://github.com/91muilak/kalium19/issues)
[![Количество открытых PR](https://img.shields.io/github/issues-pr-raw/91muilak/kalium19?label=open%20PR%27s)
![Количество закрытых PR](https://img.shields.io/github/issues-pr-closed-raw/91muilak/kalium19?label=closed%20PR%27s)](https://github.com/91muilak/kalium19/pulls)
![visitors](https://visitor-badge.laobi.icu/badge?page_id=91muilak.kalium19)

## 🗿 Как использовать?
После выполнения [этапа установки](https://github.com/91muilak/kalium19#-%D1%83%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0-) вам становятся доступны все миксины и утилиты из пакета `kalium19`. Для примера посмотрим как использовать миксины Box Shadow и Border Radius: 

```scss
// src/card.scss

@import '/path/to/kalium19';

.card {

  background-color: #42b922;
  padding         : 1em 1.2em;
  ...

  // Добавим закругления
  @include border-radius(8px);

  // Добавим тени
  @include box-shadow(
    rgba(60, 64, 67, 0.3) 0px 1px 2px 0px, 
    rgba(60, 64, 67, 0.15) 0px 2px 6px 2px
  );

}
```
```css
/* output/card.css */
.card {

  background-color: #42b922;
  padding         : 1em 1.2em;
  ...

  -webkit-border-radius: 8px;
  -moz-border-radius   : 8px;
  border-radius        : 8px;

  -webkit-box-shadow: rgba(60, 64, 67, 0.3) 0px 1px 2px 0px, rgba(60, 64, 67, 0.15) 0px 2px 6px 2px;
  -moz-box-shadow   : rgba(60, 64, 67, 0.3) 0px 1px 2px 0px, rgba(60, 64, 67, 0.15) 0px 2px 6px 2px;
  box-shadow        : rgba(60, 64, 67, 0.3) 0px 1px 2px 0px, rgba(60, 64, 67, 0.15) 0px 2px 6px 2px;

}
```
Помимо этих двух миксинов есть и другие. Подробнее в [документации](https://kalium19.netlify.app).
## 📥 Установка ![](https://img.shields.io/github/package-json/version/91muilak/kalium19/main?label=%20)
Выполнить установку Kalium19 можно склонировав весь репозиторий напрямую с GitHub или же установить через пакетный менеджер [npm](https://nodejs.org/en/download/).
### 🔴 npm
Для установки Kalium19 в проект выполните команду:
```bash
npm i @rx1310/kalium19
```
и добавьте файл в импорт:
```scss
@import 'node_modules/@rx1310/kalium19/kalium19';
```

### :octocat: Git
Для клонирования проекта необходимо иметь установленный [git](https://git-scm.com/downloads). Если он установлен, то просто выполните команду в терминале:
```bash
git clone https://github.com/91muilak/kalium19
```
и добавьте файл в импорт:
```scss
@import 'kalium19/kalium19';
```
### 🗂 Git Submodules
Для клонирования в качестве субмодуля также нужен установленный [git](https://git-scm.com/downloads). Если он установлен, то просто выполните команду в терминале:
```bash
git submodule add https://github.com/91muilak/kalium19
```
и добавьте файл в импорт:
```scss
@import 'kalium19/kalium19';
```
## 📦 Сборка
Для сборки проекта необходим пакетный менеджер [npm](https://nodejs.org/en/download/), который устанавливается вместе с NodeJS. Если npm уже установлен, то откройте в терминале папку проекта и выполните команду:
```bash
npm install
```
Команда установит [`sass`](https://www.npmjs.com/package/sass) ![Версия SASS](https://img.shields.io/github/package-json/dependency-version/91muilak/kalium19/dev/sass/main?label=%20) чтобы скомпилировать SASS в CSS.  Для компиляции необходимо выполнить команду `npm run sass:compile`. После этого появится папка _css_ с готовыми CSS-файлами.

**Другие команды:**
- `npm run sass:watch` - вотчинг изменений в файлах и мгновенная компиляция;
- `npm run sass:watch-compressed` - то же что и `npm run sass:watch`, но компилируется уже минифицированный CSS;

> В принципе вы можете воспользоваться любым другим способом или утилитой для компиляции SASS.
## 👥 Комьюнити
[Я](https://github.com/rx1310) буду рад получить от вас фидбек или какую-либо помощь для улучшения проекта. Идеи 💡, код 👩‍💻, советы 👌 и всё что только можно - я буду рад 😊.

[![Telegram](https://img.shields.io/badge/telegram-26A5E4?logo=telegram)](https://t.me/rx1310)
[![Дискуссии](https://img.shields.io/github/discussions/91muilak/kalium19?logo=github)](https://github.com/91muilak/kalium19/discussions)
[![Discord](https://img.shields.io/discord/917901779394514954?color=5865F2&label=discord&logo=discord&logoColor=fff)](https://discord.gg/fvW9mHE6)

## 📜 Лицензия ![Лицензия](https://img.shields.io/github/license/91muilak/kalium19?label=%20)
Проект распространяется по свободной [лицензии MIT](LICENSE).

```
MIT License

Copyright (c) 2021 The Kalium19 Project Authors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

![Ключевые слова](https://img.shields.io/github/package-json/keywords/91muilak/kalium19?label=%20)