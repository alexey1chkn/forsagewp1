﻿=== Saphali Woocommerce Russian ===
Contributors: Saphali
Plugin Name: Saphali Woocommerce Russian
Plugin URI: http://saphali.com/saphali-woocommerce-plugin-wordpress
Donate link: https://money.yandex.ru/to/410011651211340
Tags: woocommerce, woo commerce russian, russian ruble, ukrainian hryvnia, mod, manadger filds checkout
Requires at least: WP 3.3 or higher & WooCommerce 1.6.6 or higher
Tested up to: 5.0
Stable tag: 1.8.4.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Набор русских дополнений к интернет-магазину на Woocommerce.
Adds Russian localization & special Tools in WooCommerce.

== Description ==

WooCommerce Russian! WooCommerce по-русски!
Русскоязычные функциональные дополнения для Woocommerce - специально для русского рынка.

= Интегрирует в магазин: =
* Русский интерфейс. <strong>Важное замечание!</strong>
Мы более не исправляем русский перевод в плагине - https://wordpress.org/plugins/woocommerce/, т.к. он уже корректный. Перевод нашего плагина полезен тем, кто использует Woocommerce 2.0 и ниже, т.е. старые версии плагина. Начиная с версии 1.6.3 плагин содержит украинскую локализацию.
Остальным просто нужно установить https://wordpress.org/plugins/woocommerce/ и все. Если возникают с переводом проблемы с установленной версией WC, то  нужно в самом WC произвести обновление. Можно зайти в “Woocommerce => System Status (Магазин => Состояние системы)”, перейти на вкладку “Tools” (Инструменты), и нажать на кнопку “Force Translation Upgrade”, чтобы обновить перевод.
Теперь основные файлы локализации (помимо тех, которые в Saphali woocommerce russian) находятся здесь:
wp-content/languages/plugins/woocommerce-admin-ru_RU.mo (админ часть), wp-content/languages/plugins/woocommerce-ru_RU.mo (пользовательская часть).
Также <em>как вариант</em> можете скачать файл http://saphali.com/lang.zip и распаковав скопируйте их тогда сюда wp-content/languages/plugins

* Валюты СНГ - Российский рубль (RUB), Украинскую гривну (UAH), Белорусский рубль (руб.), Armenian dram (Դրամ), Киргизский сом (сом) и Казахстанский тенге (тңг), Узбекский сум, Литовский лит
* Возможность настроить заказную форму для оформления заказа
* Управление количеством колонок в каталоге

= Особенности =

* Улучшенная русская и украинская локализация Woocommerce (более полная поддержка русского и украинского языка).
* В общий список валют добавлены — Украинская гривна (грн.), Российский рубль (руб.), Белорусский рубль (руб.), Armenian dram (Դրամ), Киргизский сом (сом) и Казахстанский тенге (тңг), Узбекский сум, Литовский лит
* Управление полями на странице оформления заказа и на странице профиля. Функция позволяет настроить заказную форму для оформления заказа. Можно сделать некоторые поля необязательными при оформлении заказа или удалить их полностью, тем самым упростить оформления заказа. Также можно добавить свои специальные поля.
* Управление количеством колонок в каталоге товаров (Магазин) и категориях.
* Плагин создан с целью упростить разработку интернет-магазинов для российского рынка.
* Плагин не изменяет оригинальные файлы Woocommerce, вы можете обновлять плагин Woocommerce, каждый раз при появлении новых версий!
* Сопоставление полей с методами оплаты и доставки, напр., будет полезно, если некоторые поля не требуется отображать при оплате каким-то методом доставки и/или оплаты, но нужны в каком-то другом методе доставки или оплаты.

<strong>ВНИМАНИЕ!</strong>

Вы можете подключить к магазину все самые популярные российские и украинские платежные системы:
QIWI, Приват24, LiqPay, WebMoney, Яндекс.Деньги, Интеркасса, PayPal для России и Украины, Z-payment, ChronoPay!
Подробнее о плагинах платежных шлюзов: http://saphali.com/wordpress/payment-gateways

Другие русские плагины для интернет-магазина на Woocommerce смотрите в нашем каталоге http://saphali.com/wordpress/woocommerce-plugins

== Installation ==

1. Разархивируйте содержимое zip файла в папку плагинов вашего сайта (wp-content/plugins/), используя вашу любимую FTP программу.
2. Активируйте плагин на странице "Плагины" в панели администратора.
3. Все установка завершена.

== Frequently Asked Questions ==

= Знак рубля =
В WC 2.5.2 и выше есть встроенный знак рубля, который представлен в виде одного знака (в юникоде). Из-за частых обращений, что знак рубля не отображается нормально в WC 2.5.2 и выше, когда мы убрали формирование знака данным плагином, потому знак рубля вернули обратно. Для тех у кого WC 2.5.2 и выше, и кто хочет использовать на своем сайте знак, который задан в WC, то пусть в файле saphali-woocommerce-lite.php сделает замену:
с
define('SAPHALI_LITE_SYMBOL', 1 ); 
на 
define('SAPHALI_LITE_SYMBOL', 0 );

= Ошибка "Please enter an address to continue" =
При ошибке (в WC > 3.4) "<em>Пожалуйста, введите адрес для продолжения</em>", нужно посмотреть не удалено или не выключено поле <strong>billing_country</strong>. Если есть доставка, то без местонахождения, WC не дает совершить заказ. Зоны доставки работают при определении в первую очередь страны (в зависимости от настроек, геолокализация или адрес магазина), если этого сделать невозможно, т.к. нет соответствующего поля, то происходит вывод данного уведомления.

== Screenshots ==

1. Улучшенная русская локализация Woocommerce. В общий список валют добавлены — Украинская гривна (грн.), Российский рубль (руб.), Белорусский рубль (руб.), Armenian dram (Դրամ), Киргизский сом (сом) и Казахстанский тенге (тңг), Узбекский сум, Литовский лит
2. Управление полями на странице заказа и на странице профиля. Функция позволяет настроить заказную форму регистрации, чтобы настроить магазин на упрощение оформления заказа. Вы можете сделать некоторые поля необязательными при регистрации/оформлении заказа либо удалить их полностью.
3. Управление полями (перемещение в нужную позицию).
4. Как выглядит на странице.
5. Управление количеством колонок в каталоге товаров и рубриках.

== Changelog ==

= 1.8.4.1 =
* Fix вывода Notice

= 1.8.4 =
* Правка связанная с выводом задублированных значений полей в админке.

= 1.8.3 =
* Небольшие правки.

= 1.8.2 =
* Fix позиции полей на странице заказа в WC > 3.0.
* Небольшие правки.

= 1.8.1.1 =
* Небольшие правки (Notice).

= 1.8.1 =
* Небольшие правки

= 1.8.0 =
* Добавлен функционал, который позволяет соотнести поле к методам доставки. Напр., будет полезно, если некоторые поля не требуется выводить при оплате каким-то методом доставки, но нужны в каком-то другом методе доставки.

= 1.7.1 =
* В версии WC 3.x.x отображение добавленных полей, которые отсутствуют по умолчанию в WC.

= 1.7.0 =
* Добавлен функционал, который позволяет соотнести поле к методам оплаты. Напр., будет полезно, если некоторые поля не требуется выводить при оплате каким-то методом оплаты, но нужны при оплате через какой-то другой.

= 1.6.6 =
* Исправлен учет публикации в настройках плагина в версии WC 3.x.x.

= 1.6.5 =
* Fix вывода полей в профиле (исправлен вывод дублей).

= 1.6.4 =
* Совместимость с WPML и др. плагинами мультиязычности. [Для справки. Перевод полей в файлах локализации должен быть обеспечен Вами (Text Domain: woocommerce). В данном плагине не располагается перевод полей, т.к. предугадать их невозможно (их название Вы сами задаете в настройках, потому и перевод делать также необходимо Вам). Если Вы название полей не изменяете, то названия должны быть на английском, чтобы не готовить новый перевод на другие языки].

= 1.6.3 =
* Реализована возможность править администратором введенные данные дополнительных полей в заказе.
* Обновлен стиль для российского рубля.
* Добавлена украинская локализация, которая имеет более полный перевод на украинский язык относительно версии перевода основного релиза WC.

= 1.6.2 =
* Изменения в связи с переводом для WC выше 2.5.0.

= 1.6.1 =
* Добавлена валюта - новый белорусский рубль (BYN)

= 1.6.0 =
* Из-за частых обращений, что знак рубля не отображается нормально в WC 2.5.2 и выше, знак рубля вернули, как было. Для тех у кого WC 2.5.2 и выше, и кто хочет использовать на своем сайте знак, который задан в WC, то пусть в файле saphali-woocommerce-lite.php сделает замену:
с
define('SAPHALI_LITE_SYMBOL', 1 ); 
на 
define('SAPHALI_LITE_SYMBOL', 0 );

= 1.5.9 =
* Для WC 2.5.2 используется знак рубля предусмотренный в самом WC.

= 1.5.8 =
* Fix в WC 2.4.x.

= 1.5.7 =
* Добавлен фильтр количества колонок.

= 1.5.6 =
* В Woocommerce 2.2 и выше отключена дополнительная локализация для WC, т.к. в этом уже нет надобности.

= 1.5.5 =
* Изменения в связи с выходом Woocommerce 2.3.

= 1.5.4 =
* Исправлен вывод дополнительных полей для версий WC 2.2.0 - 2.2.2.

= 1.5.3 =
* Вывод дополнительных полей в профиле/аккаунте покупателя.

= 1.5.2 =
* Изменения в связи с выходом Woocommerce 2.2.

= 1.5.1 =
* Добавлен литовский лит.

= 1.5 =
* Изменения в связи с выходом Woocommerce 2.1.0.

= 1.4 =
* В управлении полями реализована возможность использовать различные типы полей (select, checkbox, textarea).

= 1.3.8.1 =
* Поля, которые имеют пустые заголовки не выводятся в письме, в заказах

= 1.3.8 =
* Добавлен узбекский сум

= 1.3.7.2 =
* Небольшие исправления связанные с символом валюты RUB

= 1.3.7.1 =
* Изменения связанные с совместимостью WPML.

= 1.3.7 =
* Добавлен фильтр отображения полей по умолчанию. Отсутствие этого фильтра приводило к тому, что поля подтягивались javascript'oм не так как нужно (название поля и его обязательность отображалось как по умолчанию в WC).

= 1.3.6.2 =
* Повышение приоритета знака валюты по Лебедеву (для рубля) над встроенным.

= 1.3.6.1 =
* Исправлена ошибка отображения дополнительных полей заполненных покупателем (в письме и в заказе).

= 1.3.6 =
* Устранена ошибка не сохранения некоторых атрибутов поля (напр, поле "Название компании" теперь можно отмечать как обязательное, указывать текст по умолчанию). 
* Добавленные произвольные поля теперь можно сортировать вместе со стандартными полями (устранена разрозненность сортировки полей, которые есть по умолчанию, и тех, которые добавлены по надобности).
* Исправлены некритичные ошибки.

= 1.3.5 =
* Добавлена функция вывода дополнительных полей в письмах и при просмотре заказа покупателем.

= 1.3.4 =
* Добавлены валюты: Киргизский сом (сом) и Казахстанский тенге (тңг).

= 1.3.3 =
* Мелкие исправления по локализации под WooCommerce
* Добавлена поддержка валюты русского рубля в виде символа.

= 1.3.2.1 =
* Мелкие исправления по локализации под WooCommerce

= 1.3.2 =
* Мелкие исправления по локализации под WooCommerce

= 1.3.1 =
* Завершение локализации под WooCommerce 2.0

= 1.3.0 =
* Расширение локализации под WooCommerce
* Адаптация под WooCommerce 2.0.0
* Переписан код, т.к. на серверах, в которых php не понимал ограничители <? и <?= выдавал ошибку "Parse error: syntax error, unexpected..."

= 1.2.3.2 =
* Расширение локализации под WooCommerce

= 1.2.3.1 =
* Ошибка загрузки в repository

= 1.2.3 =
* На странице управления дополнительными полями и полями доставки исправлена ошибка добавления полей.
* Добавлен вывод дополнительных полей на странице профиля пользователя, а также на странице редактирования заказа.

= 1.2.2 =
* На странице управления дополнительными полями и полями доставки в заголовке к атрибутам "Название" и "Класс поля" добавлена подсказка.
* Задан стиль для неактивного поля.
* Небольшие исправления.

= 1.2.1 =
* На странице управления дополнительными полями и полями доставки в заголовке к атрибуту clear добавлена подсказка.

= 1.2 =
* Добавлено управление атрибутами clear и class в управлении полями.
* Исправлена ошибка в указании обязательного поля в управлении дополнительными полями и полями доставки.

= 1.1 =
* Исправлена ошибка в управлении полями на странице заказа и на странице профиля.

= 1.0 =
* Улучшенная русская локализация Woocommerce (корректировка перевода и дополнительный перевод).
* В общий список валют добавлены — Украинская гривна (грн.), Российский рубль (руб.) и Белорусский рубль (руб.)
* Управление полями на странице заказа и на странице профиля. Функция позволяет настроить заказную форму регистрации, чтобы настроить магазин на упрощение оформления заказа. Вы можете сделать некоторые поля необязательными при регистрации/оформлении заказа либо удалить их полностью.
* Управление количеством колонок в каталоге товаров и рубриках.


== License ==

Этот плагин является бесплатным для всех, поскольку он выпущен под GPL. Вы можете использовать его бесплатно в ваших интернет-магазинах. Но если Вам нравится этот плагин, вы можете поблагодарить нас, если поделитесь с друзями и коллегами ссылкой на наш сайт.

== Translations ==

Мы допускаем, что русскую локализацию для Woocommerce можно еще больше улучшить. Если вы заметили в настройках Woocommerce некорректный перевод или его можно заменить на альтернативный и более подходящий здесь - https://translate.wordpress.org/projects/wp-plugins/woocommerce/stable/ru/default

== Demo ==
Проверить этот плагин в работе вы можете на нашем сайте http://saphali.com/ - на странице "Демо Интернет-магазин".

== Upgrade Notice ==
= 1.6.0 =
* Из-за частых обращений, что знак рубля не отображается нормально в WC 2.5.2 и выше, знак рубля вернули, как было. Для тех у кого WC 2.5.2 и выше, и кто хочет использовать на своем сайте знак, который в WC прописан, то пусть в файле saphali-woocommerce-lite.php сделает замену:
с
define('SAPHALI_LITE_SYMBOL', 1 ); 
на 
define('SAPHALI_LITE_SYMBOL', 0 );

= 1.5.9 =
* Для WC 2.5.2 используется знак рубля предусмотренный в самом WC.

= 1.4 =
* В управлении полями реализована возможность использовать различные типы полей (select, checkbox, textarea).

= 1.3.8.1 =
* Поля, которые имеют пустые заголовки не выводятся в письме, в заказах

= 1.3.8 =
* Добавлен узбекский сум

= 1.3.7.2 =
* Небольшие исправления связанные с символом валюты RUB

= 1.3.7.1 =
* Изменения связанные с совместимостью WPML.

= 1.3.7 =
* Добавлен фильтр отображения полей по умолчанию. Отсутствие этого фильтра приводило к тому, что поля подтягивались javascript'oм не так как нужно (название поля и его обязательность отображалось как по умолчанию в WC).

= 1.3.6.2 =
* Повышение приоритета знака валюты по Лебедеву (для рубля) над встроенным.

= 1.3.6.1 =
* Исправлена ошибка отображения дополнительных полей заполненных покупателем (в письме и в заказе).

= 1.3.6 =
* Устранена ошибка не сохранения некоторых атрибутов поля (напр, поле "Название компании" теперь можно отмечать как обязательное, указывать текст по умолчанию). 
* Добавленные произвольные поля теперь можно сортировать вместе со стандартными полями (устранена разрозненность сортировки полей, которые есть по умолчанию, и тех, которые добавлены по надобности).
* Исправлены некритичные ошибки.

= 1.3.2.1 =
* Мелкие исправления по локализации под WooCommerce

= 1.3.2 =
* Мелкие исправления по локализации под WooCommerce

= 1.3.1 =
* Завершение локализации под WooCommerce 2.0

= 1.3.0 =
* Расширение локализации под WooCommerce
* Адаптация под WooCommerce 2.0.0
* Переписан код, т.к. на серверах, в которых php не понимал ограничители <? и <?= выдавал ошибку "Parse error: syntax error, unexpected..."

= 1.2.3.2 =
* Улучшение локализации под WooCommerce

= 1.2.3 =
* На странице управления дополнительными полями и полями доставки исправлена ошибка добавления полей.
* Добавлен вывод дополнительных полей на странице профиля пользователя, а также на странице редактирования заказа.

= 1.2.2 =
* На странице управления дополнительными полями и полями доставки в заголовке к атрибутам "Название" и "Класс поля" добавлена подсказка.
* Задан стиль для неактивного поля.
* Небольшие исправления.

= 1.2.1 =
* На странице управления дополнительными полями и полями доставки в заголовке к атрибуту clear добавлена подсказка.

= 1.2 =
* Добавлено управление атрибутами clear и class в управлении полями.
* Исправлена ошибка в указании обязательного поля в управлении дополнительными полями и полями доставки.

= 1.1 =
Исправлена ошибка в управлении полями на странице заказа и на странице профиля.

= 1.0 =
Выпущен релиз.


