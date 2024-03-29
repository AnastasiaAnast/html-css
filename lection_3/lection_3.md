# Работа с макетом и cоздание блочной структуры

- что такое макет
- визуальная верстка
- работа с макетом figma
- строчные и блочные эл-ты
- формирование блочной модели

**Макет** - финальный вид сайта, его картинка, которую отрисовал дизайнер.

**Визуальная верстка** - сборка макета из любого графического редактора (фш/фигма/скетч) - конвертация в удобный программисту вид.
Avokode.com

Плюсы глобальной визуальной верстки:

- Возможность работы практически с любым графическим редактором
- Возможность скачивания изображений в SVG-формате
- Работа со слоями макета
- Настройка отображаемых стилей
- Веб-версия

Figma - графический редактор + визуальная верстка.
Работа с макетом в формате Figma.

режим inspect - прав верх угол

не копируем блок "позиционирование" в фигма

скачать картинку - снизу справа export, выбрать формат изображения - SVG - векторные отрисованные изображения

## Основные теги для верстки div, span

- Блочные эл-ты (div)
- Строчные эл-ты (span - парный тег для стилизации текста)

## Особенности блочных эл-тов

1. Блочные элементы отображаются на веб-странице в виде прямоугольника
2. Занимают всю доступную ширину (100% экрана в ширину)
3. Высота определяется содержимым (без содержимого - 0%)
4. Начинаются с новой строки
5. Допускается вкладывать один блочный элемент внутрь другого
6. Запрещено добавлять внутрь строчных элементов блочные

Строчные эл-ты - для стилизации части текста (<span>, <a>(ссылка), <i>(курсив), <b>(жирный), <strong>(жирный+приотритет слову)...):

1. Не распространяются на всю ширину (ширина не 100%) - она зависит от контента
2. Нельзя менять высоту
3. Отступы будут действовать
4. Не можем внутри строчных располагать блочные эл-ты, но можем строчные

Самый важный инструмент в глобальном создании сайта - отладчик браузера.
Делится визуально на три части:

- html
- css
- js (окно js можно закрывать)

Через отладчик отлично видны блоки на странице, можно перетаскивать блоки - менять местами, также в отладчике, дописывать код - это будет "черновик", который не сохранится при обновлении страницы.

Оранжевые границы в отладчике - это отступы. У эл-тов изначально может присутствоввать стандартная стилистика и в нее будут входить отступы.

При наведении на элемент всегда можно определить блочный он или строчный - если блочный - займет всю ширину экрана.

**Поставить ссылку на нужный кусок текста** - вырезать нужный текст, на его месте вставить тег "a":

        <a href="#">вырезанный текст</a>

здесь # будет являться "заглушкой" - на ее месте потом можно будет поставить ссылку.

## Формирование блочной модели

Помимо шрины и высоты эл-та есть еще 2 вида отступов:

- padding (внутренний отступ)
- border (рамка)
- margin (внешний отступ)

Нажимаем на любой эл-т: если блок располагается внутри - отступ будет внутренний, снаружи - внешний. Если нет фоновых значений - отступ может быть и внутренний, и внешний.

## Блочная модель: как записываются параметры:

**margin**: 25px 10px; (внушний отступ снаружи (оранжевая граница) 25 писелей сверху и снизу, 10 слева и справа)
**border**: 5px solid black; (рамка 5-ти пиксельная, сплошная черная)
**padding**: 10px; (внутренний отступ 10 пикселей со всех сторон)
**width**: 200px; (ширина)
**height**: 100px; (высота)

Первым делом в проекте обнуляем стандартные отступы (а потом - задаем)
