### Подключить .css к документу html - посредством link:

        <link rel="stylesheet" href="style.css" />

В каждом документе html, к которому будут применены стили, необходимо вставить в теге head после строчки:

            <meta name="viewport" content="width=device-width,

Если html лежит внутри другой папки, путь до файла css изменится (css в папке наверх - ../имя.css)

### Задать класс для заголовка/параграфа:

Вписать class="название класса" внутрь нужного тега (каждого). Прим:

        <a class="menu_link" href="">Контакты</a><br />
        <h1 class="h1">Главная страница</h1>

Внутри файла .css класс пишется через точку: прим: .menu_link и внутри фигурных скобок - св-ва

        .menu_link {
        color: cornflowerblue;
        font-size: 16px;
        line-height: 20px;
        }
