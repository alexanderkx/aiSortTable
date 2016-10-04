# Простая сортировка таблицы на чистом JavaScript
![](http://alexanderweb.ru/upload/git/aiSortTable_git_img.gif?raw=true])

Ещё один вариант простой сортировки таблицы. На данный момент сортирует строки/числа. В планах также реализовать сортировку по датам/времени.

[ **Demo: [codepen.io](http://codepen.io/alexanderweb/pen/XjzzZy)** ]

## Подключение

Ничего не обычного, подключаем js:

```html
<script src="/path/to/src/js/aiSortTable.min.js"></script>
```

и при необходимости css:

```html
<link rel="stylesheet" href="/path/to/src/css/aiSortTable.min.css">
```

## Использование

```javascript
aiSortTable.init("myTable", [0, 3], function(e) {
  console.log(e);
});
```

Первым параметром передаём `id` таблицы (к которой требуется применить сортировку), вторым параметром передаём массив колонок для сортировки `(0 ... n)`. Последним параметром идёт функция, которая сработает после сортировки.

## CSS

- `.ai_th_sortable` - Ячейка шапки, при клике на которую происходит сортировка;
- `.ai_th_sortable__up` - Состояние сортировки по убыванию;
- `.ai_th_sortable__down` - Состояние сортировки по возростанию;
- `.ai_td_active` - Класс ячеек в активной колонке.
