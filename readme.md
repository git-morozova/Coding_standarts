## Улучшения кода в соответствии со стандартами DRY, KISS, YAGNI, SOLID

<table>
    <thead>
        <tr>
            <th>№ п/п</th>
            <th>Исправление</th>
            <th>Проект</th>
            <th>Принцип</th>
            <th>Коммит</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1</td>
            <td>Убраны margin-bottom и margin-top в единый стиль margin (класс .types-blocks-block__text)</td>
            <td>Repair_design_project</td>
            <td>DRY</td>
            <td><a href="https://github.com/git-morozova/Repair_design_project/commit/74b7b21f1bc4471e727c5020e0c8d7bda4bc8fe8">commit 1</a></td>
        </tr>
        <tr>
            <td>2</td>
            <td>Убраны background-image, background-attachment, background-position и background-size в единый стиль background (класс .portfolio)</td>
            <td>Repair_design_project</td>
            <td>DRY</td>
            <td><a href="https://github.com/git-morozova/Repair_design_project/commit/a4ff7eb4af889275945c6ae9b8859e338dd1fd51">commit 2</a></td>
        </tr>
        <tr>
            <td>3</td>
            <td>Убраны background-image, background-attachment, background-position и background-size в единый стиль background (класс .contacts)</td>
            <td>Repair_design_project</td>
            <td>DRY</td>
            <td><a href="https://github.com/git-morozova/Repair_design_project/commit/3d27998500db776137fa962f53d71ee3dbdeae69">commit 3</a></td>
        </tr>
        <tr>
            <td>4</td>
            <td>Объединены повторяющиеся стили position и top для классов .gallery-img__left и .gallery-img__right (mobile.css)</td>
            <td>Repair_design_project</td>
            <td>DRY</td>
            <td><a href="https://github.com/git-morozova/Repair_design_project/commit/7aa945d6faeae2019a68c2a7fcc7e9eef972c5fb">commit 4</a></td>
        </tr>
        <tr>
            <td>5</td>
            <td>Удалены закомментированные куски кода, которые были оставлены на всякий случай или для отладки. Удалено неиспользуемое изображение</td>
            <td>Repair_design_project</td>
            <td>YAGNI</td>
            <td><a href="https://github.com/git-morozova/Repair_design_project/commit/cd01ff04f06c1ce696a5a8191ec282cd80c961ac">commit 5</a></td>
        </tr>
        <tr>
            <td>6</td>
            <td>Частично повторяющийся код (DRY) на вывод ошибок заполнения форм регистрации и аутентификации убран со страниц регистрации и входа на сайт. Сделана отдельная функция для проверки ошибок showError(), в которой объединены коды ошибок, и эта функция записана в файл functions.php к остальным функциям (KISS). На страницах login.php и reg.php теперь просто происходит вызов функции <?php showError() ?></td>
            <td>SPA_Site_with_auth</td>
            <td>KISS + DRY</td>
            <td><a href="https://github.com/git-morozova/SPA_Site_with_auth/commit/f4417ba127c8d7a6ed589bec5c99e9b2849cc39f">commit 6</a></td>
        </tr>
        <tr>
            <td>7</td>
            <td>Убраны функции, которые используются только для расчета скидки - getBirthDay() и getSale(). Раньше скидки за день рождения и за первое посещение сайта были в разных функциях, теперь за этот функционал отвечает единая функция getPrice() (SOLID). Больше не нужно смотреть в разные места, чтобы понять, как считается скидка (KISS).</td>
            <td>KISS+SOLID</td>
            <td><a href="https://github.com/git-morozova/SPA_Site_with_auth/commit/627f27b9da786783afbbec9c6c27a0045a9766c3">commit 7</a></td>
        </tr>
        <tr>
            <td>8</td>
            <td>Убрана со страниц login.php, reg.php и lk.php кнопка "Главная", которая дублирует функционал перехода на главную по ссылке с логотипа.</td>
            <td>YAGNI</td>
            <td><a href="https://github.com/git-morozova/SPA_Site_with_auth/commit/c3436b2a9e261febb0ee0bc4b9b29234080cefd5">commit 8</a></td>
        </tr>
    </tbody>
</table>

## Проверка семантики и валидности верстки сайта

## Доработка верстки по БЭМ

## Линтеры
