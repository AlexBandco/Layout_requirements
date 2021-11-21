# Требования к верстке / Layout markup / HTML, CSS, JavaScript
## Основные
1. Валидный код по W3.ORG
2. Верстка в bootstrap или с использованием других готовых фреймворков недопустима. Только вручную
подготовленный код (bootstrap можно использовать только для задания сетки).
3. Браузеры, в которых должно быть как в макете:
- Internet Explorer 11
- Opera последняя стабильная версия
- Safari последняя стабильная версия
- Mozilla последняя стабильная версия
- Chrome последняя стабильная версия
4. Меню стараемся делать через <ul></ul>
5. Использовать наследование шрифтов (если требуемого шрифта нет на компьютере где отображается сайт,
то нужно заменять на более простой стандартный шрифт)
6. Не использовать таблицы, кроме случаев, где они являются контентом (содержимым страницы).
7. Не использовать тэг img кроме случаев, где картинка является контентом или явным элементом картинкой.
8. Верстка контента (содержимое страницы, которое заносит контент менеджер) должна быть с
использованием “голых” тэгов. Например, не допускается <p class=”text”> правильно - <p>.
Вся контентная часть должна быть заключена в тэг, например <div class=”content”> и все что внутри этого тэга
приходит из системы управления сайтом. Все стилевые определения содержимого контента должны быть
вида: .content p или .content h2 и т.д.
В случае если в контенте используется два стиля для одного и того же элемента, например, два вида таблиц,
то допускается для таблицы по умолчанию стиль: .content table для дополнительной таблицы стиль: .content
table.styled
9. Единственный тэг h1 на странице. Это заголовок страницы.
10. Заголовки - в контенте делать тэгами h2-h6 без применения bold или strong
11. Табу на названия классов “title” и “mail”, они используются в окнах визуального редактора CMS.
12. Верстка должна быть выполнена таким образом, что в случае наполнения сайта текстовым контентом
большего объема, ничего не разваливалось. Это касается также дополнительных колонок, виджетов и т.д.
Кроме тех случаев, где заданы ограничения дизайном сайта. Все изображения в контент заносит
пользователь, это надо учесть и сделать так, чтобы случайно добавленные большие изображения не ломали
верстку. В контейнере, в который предусматривается вставка статей / текста силами контент менеджера,
нельзя прописывать изображениям margin:0 и padding:0. Иначе невозможно редактировать отступы от
картинок до текста средствами визуального редактора CMS.
13. При верстке картинок в списках любых элементов, а также карточках элемента учитывать, что реальные
изображения по соотношению сторон могут отличаться от запланированных. При этом изображение должно
быть корректно вписано в указанную для него область по меньшей из двух сторон, центрироваться по обоим
измерениям, а по большей стороне должно обрезаться все, что не вошло в отведенный контейнер. Этого
эффекта можно добиться с помощью стиля «background-size: cover» или другими способами.
14. Рекомендуемая структура папки plain:
- все картинки, имеющие отношение к дизайну, хранятся в каталоге img
- все картинки, имеющие отношение к временному тестовому контенту (поступающему из админки),
хранятся в папке temp
  - стилевые файлы в папке css
  - javascript код сайта и javascript библиотеки jquery, colorbox и т.п код в папке js
  - шрифты в папке fonts
15. Необходимо, чтобы все ссылки на внешние ресурсы были помечены аттрибутом rel=nofollow
16. Изображения должны содержать и TITLE, и ALT
17. Использование JS – можно использовать JQuery, готовые библиотеки каруселей (например slick, owl или
любые другие достаточно популярные). Допускается использование чистого JS. НЕ допускается
использование каких-либо js фреймворков (AngularJS, Ember.js, Vue.js. и другие).
18. Необходимо использование системы управления версиями git (например, https://github.com/), для более
удобного отслеживания внесенных правок (если до этого не пользовались — самое время начать, как делают
профессионалы). Без этого внесение правок и исправление ошибок после сдачи проекта очень
затруднительно.

## Дополнительные
1. Не объединять скрипты в один файл или объединять только сторонние скрипты (например, bootstrap, jquery и др.). Скрипты же написанные именно для этого сайта (далее называю самописные) должны быть точно в отдельном файле (например, main.js или site.js).

Также нельзя минифицровать файлы с самописным js. Можно вообще не минифицировать любой js.

2. Не объединять стили в один файл или объединять только сторонние стили (например, bootstrap, jquery и др.). Стили же написанные именно для этого сайта (далее называю самописные) должны быть точно в отдельном файле (например, main.css или site.css).

Также нельзя минифицровать файлы с самописным css. Можно вообще не минифицировать любой css.

3. Требование к JS при наличии такового в верстке: 
Можно использовать JQuery, готовые библиотеки каруселей (например slick, owl или любые другие достаточно популярные). Допускается использование чистого JS. НЕ допускается использование каких-либо js фреймворков (AngularJS, Ember.js, Vue.js. и другие).
