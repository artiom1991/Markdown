# Материалы книги:

### Matt Cone - The Markdown Guide

> __Важно понимать__, что компилятор `Markdown` генерирует шаблонную `HTML-разметку` со своими встроенными стилями. Поэтому в
> файлах `.md` и `.markdown` допускается использование `HTML-разметки` с `inline-стилями`.

> __Где используется__? Чаще всего файлы с расширением `.md` используются для написания документации для программного кода
> или репозиториев на `GitHub`. Однако это не единственное применение формата. `Markdown` также используется для генерации
> простых HTML-шаблонов, разметки для электронных писем и конвертации в `.pdf`.

## Заголовки:

| Синтаксис | Описание                                                                                                                              |
|-----------|---------------------------------------------------------------------------------------------------------------------------------------|
| `#`       | Заголовок первого порядка H1. **Пример**: `# Heading level 1` . **Аналог HTML**: `<h1> Heading level 1 </h1> `                        |
| `##`      | Заголовок первого порядка H2. **Пример**: `## Heading level 2` . **Аналог HTML**: `<h2> Heading level 2 </h2> `                       |
| `###`     | Заголовок первого порядка H3. **Пример**: `### Heading level 3` . **Аналог HTML**: `<h3> Heading level 3 </h3> `                      |
| `####`    | Заголовок первого порядка H4. **Пример**: `#### Heading level 4` . **Аналог HTML**: `<h4> Heading level 4 </h4> `                     |
| `#####`   | Заголовок первого порядка H5. **Пример**: `##### Heading level 5` . **Аналог HTML**: `<h5> Heading level 5 </h5> `                    |
| `######`  | Заголовок первого порядка H6. **Пример**: `###### Heading level 6` . **Аналог HTML**: `<h6> Heading level 6 </h6> `                   |
| `==`      | Альтернативная форма обозначения заголовка первого порядка это под текстом выставить любое количество `==`                            |
| `--`      | Альтернативная форма обозначения заголовка второго порядка это под текстом выставить любое количество `--`                            |

## Выделение текста:

| Синтаксис | Описание                                                                                                                         |
| --------- |----------------------------------------------------------------------------------------------------------------------------------|
| `*`       | Выделение наклонным шрифтом. **Пример**: `*Italic*` . **Аналог HTML**: `<em>Italic</em>`                                         |
| `_`       | Выделение наклонным шрифтом. **Пример**: `_Italic_` . **Аналог HTML**: `<em>Italic</em>`                                         |
| `**`      | Выделение жирным шрифтом. **Пример**: `**Bold**` . **Аналог HTML**: `<strong>Bold</strong>`                                      |
| `__`      | Выделение жирным шрифтом. **Пример**: `__Bold__` . **Аналог HTML**: `<strong>Bold</strong>`                                      |
| `***`     | Выделение жирным и наклонным шрифтом. **Пример**: `***Bold&Italic***` . **Аналог HTML**: `<strong><em>Bold&Italic</em></strong>` |
| `___`     | Выделение жирным и наклонным шрифтом. **Пример**: `___Bold&Italic___` . **Аналог HTML**: `<strong><em>Bold&Italic</em></strong>` |
| `__*`     | Выделение жирным и наклонным шрифтом. **Пример**: `***Bold&Italic***` . **Аналог HTML**: `<strong><em>Bold&Italic</em></strong>` |
| `**_`     | Выделение жирным и наклонным шрифтом. **Пример**: `___Bold&Italic___` . **Аналог HTML**: `<strong><em>Bold&Italic</em></strong>` |
| `~~`      | Текст перечеркивается по центру строки. **Пример**: `~~Strikethrough~~` . **Аналог HTML**: `<del>Strikethrough</del>`            |

## Цитата:

| Синтаксис | Описание                                                                                                                              |
| --------- |---------------------------------------------------------------------------------------------------------------------------------------|
| `>`       | Выделяет текст как цитату и может быть многострочным **Пример**: `> Text`. **Аналог HTML**: `<blockquote><p>Text</p></blockquote>`    |
| `>>`      | Создает вложенные цитаты. Могут быть тоже многострочными.                                                                             |

## Списки:

| Синтаксис | Описание                                                                                                                              |
| --------- |---------------------------------------------------------------------------------------------------------------------------------------|
| `1.`      | Создает упорядоченный список **Пример**: `1.First element`. **Аналог HTML**: `<ol><li>First  element</li></ol>`                       |
| `-`       | Создает неупорядоченный список **Пример**: `- First element`. **Аналог HTML**: `<ul><li>First  element</li></ul>`                     |
| `+`       | Создает неупорядоченный список **Пример**: `+ First element`. **Аналог HTML**: `<ul><li>First  element</li></ul>`                     |
| `*`       | Создает неупорядоченный список **Пример**: `* First element`. **Аналог HTML**: `<ul><li>First  element</li></ul>`                     |

> Чтобы создать вложенный список, необходимо выставить 4 пробела или табуляцию в начале вложенного элемента списка.

> **Markdown**:
>
> ```
>   - First item
>   - Second item
>   - Third item
>       - Indented item
>       - Indented item
>   - Fourth item
> ```

> **Результат в Markdown**:
>
> - First item
> - Second item
> - Third item
> - Indented item
> - Indented item
> - Fourth item

# Список определений:

> В расширенной версии `Markdown` можно создавать списки определений, используя формат, в котором термин задается
> в первой строке, а его определение — в последующих строках. Для определения используется двоеточие и отступ.

> **Markdown**:
>
> ```
> First Term
> : This is the definition of the first term.
>
> Second Term
> : This is one definition of the second term.
> : This is another definition of the second term.
> ```

> **Результат в Markdown**:
>
> <dl>
>   <dt>First Term</dt>
>   <dd>This is the definition of the first term.</dd>
>   <dt>Second Term</dt>
>   <dd>This is one definition of the second term. </dd>
>   <dd>This is another definition of the second term.</dd>
> </dl>

> **HTML**:
>
> ```
> <dl>
>   <dt>First Term</dt>
>   <dd>This is the definition of the first term.</dd>
>   <dt>Second Term</dt>
>   <dd>This is one definition of the second term. </dd>
>   <dd>This is another definition of the second term.</dd>
> </dl>
> ```

## Параграф:

> В `Markdown` параграфом считается любая строка, не начинающаяся со специальных символов. Простой перевод строки
> не считается началом нового абзаца. Для создания нового абзаца нужно добавить дополнительную пустую строку
> или сделать так, чтобы строка заканчивалась двумя пробелами перед переводом строки.

## Перевод строки:

> В стандартном `HTML` перевод строки осуществляется через `<br>`. В `Markdown` для этого используются двойные пробелы
> в конце строки, после чего следует перевод строки.

# Изображения:

> Для вставки изображения используется следующий синтаксис: `![Alt](url "Title")`, где `!` обозначает, что это изображение,
> `[Alt]` — текст, который отображается, если изображение не загружается, url в круглых скобках — ссылка на изображение,
> а второй аргумент `"Title"` — заголовок изображения.

> **Markdown**: `![Logo Image](images/logo.png "Site Logo")`

> **HTML**: `<img src="images/logo.png" alt="Logo Image" title="Site Logo">`

# Код:

> Чтобы обозначить текст как код, нужно поместить код между косых кавычек \` \`.

> **Markdown**: <code>\`let isTrue = True;\`</code>.

> **HTML**: `<code>let isTrue = True;</code>`

# Блок кода:

> Чтобы создать блок кода в `Markdown`, нужно использовать отступ в 4 пробела или 1 табуляцию от края документа.
> Если блок кода находится внутри другого элемента (например, внутри списка), нужно использовать
> двойной отступ — 8 пробелов или 2 табуляции.

> **Markdown**:
>
>       <html>
>           <head>
>           </head>
>       </html>

> Также можно поместить код между специальными символами (```) или (~~~) для создания блоков кода.

> **Markdown**:
>
> ```
> /~~~
> <html>
>   <head>
>   </head>
> </html>
> /~~~
> ```

> **HTML**:
>
>       <pre>
>           <code>
>               &lt;html&gt;
>               &lt;head&gt;
>               &lt;/head&gt;
>               &lt;/html&gt;
>           </code>
>       </pre>

# Подсветка синтаксиса:

> Также среди дополнительных возможностей поддерживается подсветка синтаксиса, которая обозначается, например,
> для `JSON` с помощью ` ```json` или `~~~json`. Поддерживаются большинство современных синтаксисов, таких как `HTML`,
> `CSS`, `JSON`, `XML`, `TypeScript`, `Java` и другие.
>
> **Пример**:
>
> ```json
> {
>   "firstName": "John",
>   "lastName": "Smith",
>   "age": 25
> }
> ```

# Горизонтальная черта:

> Для создания горизонтальной линии через весь документ нужно в пустой строке разместить последовательность из
> трех символов. Это могут быть следующие варианты: `___`, `---` или `***`.

 ---

> **Markdown**: `***`.

> **HTML**: `<hr>`

# Ссылки:

> Создание ссылки похоже на создание изображения, только без восклицательного знака, и осуществляется
> по шаблону: `[Текст ссылки](адрес)`, где первый аргумент — это текст ссылки, а второй — адрес. Также ссылка может
> содержать заголовок: `[Текст ссылки](адрес "Заголовок")`.

> **Markdown**: `[Google](https:\\google.com)` или `[Google](https:\\google.com "Google Official Page")`

> **HTML**: `<a href="https:\\google.com">Google</a>` или `<a href="https:\\google.com" title="Google Official Page">Google</a>`

# Таблицы:

> Стандартные возможности `Markdown` не включают создание таблиц, однако большинство сервисов, таких как `GitHub`,
> используют расширенную версию Markdown с дополнительным синтаксисом для таблиц. При помощи символов `|` формируются
> границы таблицы, между которыми задаются значения полей. Первая строка служит заголовком таблицы, а вторая строка
> отделяет заголовок от тела таблицы. Важно сохранять структуру таблицы до конца.
> Также внутри ячеек можно указать выравнивание текста: по левому краю — `:---`, по центру — `:---:`, или по правому краю — `---:`.

> **Markdown**:
>
> `|     Nr    | Description |`  
> `|-----------|-------------|`  
> `| Header    | Title       |`  
> `| Paragraph | Text        |`

> **HTML**:
>
>        <table>
>           <thead>
>               <tr class="header">
>                   <th>Syntax</th>
>                   <th>Description</th>
>               </tr>
>           </thead>
>           <tbody>
>               <tr class="odd">
>                   <td>Header</td>
>                   <td>Title</td>
>               </tr>
>               <tr class="even">
>                   <td>Paragraph</td>
>                   <td>Text</td>
>               </tr>
>           </tbody>
>        </table>
