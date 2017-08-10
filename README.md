![image](http://presswall.springhead.su/static/images/logo.png)

Запуск сайта Легкомаркет
===
Настроен тестовый сервер, выложена текущая версия сайта. Все изменения будут доступны по адресу http://presswall.springhead.su. Обновления планируются раз в сутки.

Создан список задач, закрытие которых необходимо для запуска - https://github.com/springhead-su/presswall/issues. Участие в обсуждениях приветствуется (необходимо зарегистрироваться на гитхабе - https://github.com).

#### Ближайшие работы
- Оформление заказа.
- Админка, наполнение контентом.

---

- [Товары](#Товары)
  - [Список и фильтрация товаров](#Список-и-фильтрация-товаров)
  - [Детали товара](#Детали-товара)
  - [Наполнение товарами](#Наполнение-товарами)
- [Оформление заказа](#Оформление-заказа)
  - [Шаги оформления заказа](#Шаги-оформления-заказа)
  - [1. Товары и услуги](#1-Товары-и-услуги)
  - [2. Получение заказа](#2-Получение-заказа)
  - [3. Контактные данные](#3-Контактные-данные)
  - [4. Способы-оплаты](#4-Способы-оплаты)
  - [Проверьте ваш заказ](#Проверьте-ваш-заказ)
  - [Заказ оформлен](#Заказ-оформлен)

Товары
---
### Список и фильтрация товаров
Товары выводятся на странице категории с сортировкой по цене по возрастанию.

По умолчанию включен режим Оптимальный выбор - на странице выводится три товара. При выключении режима оптимального выбора появляются быстрые фильтры по особенностям товаров. Если при выбранных фильтрах существует возможность дополнительной фильтрации по техническим характеристикам - выводится второстепенный фильтр (например, по размеру).

**Задачи:**
- [Сортировка товаров](https://github.com/springhead-su/presswall/issues/2) - нужна дополнительная сортировка или нет?
- Фильтрация товаров - требуется заполнение всех товаров для дополнительного тестирования.
- Привязка товаров к фильтрам - по мере наполнения и тестирования работы фильтров.

### Детали товара
При клике на товар он открывается во всплывающем окне. Слева выводятся все изображения товара с прокруткой. Справа - подробная карточка товара.

**Задачи:**
- Закрывать всплывающее окно при нажатии на esc.
- Для всплывающего окна требуются качественные фотографии каждого товара.

### Наполнение товарами
Товарами частично наполнен раздел Баннерные стенды. Дальнейшее наполнение будет после запуска админки.

**Задачи:**
- Наполнение товарами - ожидает админку.
- Заголовки товаров - надо придумать.
- Подбор изображений ко всем товарам.
- Проставление цен товаров.

Оформление заказа
---
### Шаги оформления заказа
1. Товары и услуги
2. Получение заказа
3. Контактные данные
4. Способы оплаты
- Проверьте ваш заказ
- Заказ оформлен

Все изменения на любом шаге сразу сохраняются. Можно ходить по шагам туда-сюда. Выводятся "хлебные крошки" всех шагов.

### 1. Товары и услуги
Возможность загрузить файлы или предоставить необходимую информацию для конкретного товара (загрузить макет дизайна, указать время мероприятия и тп). Выводятся все товары (чтобы не показалось, что товар пропал из корзины), даже если нет опций.

**Задачи:**
- ~~Прототип страницы~~
- Проектирование случая, когда у товара нет опций
- Улучшение дизайна страницы
- По мере заполнения товаров во всех категориях проверить список необходимых опций, скорректировать по результатам тестирования
- Механизм загрузки файлов

### 2. Получение заказа
Получение заказа возможно двумя основными способами: самовывоз и курьерская доставка. Выбор конкретного способа зависит от выбранного города. Изначально город выбирается в соответствии с автоматически определенным городом для всего сайта.

**Самовывоз** осуществляется со склада, если выбран Санкт-Петербург (возможно появление складов в других городах), или с терминала транспортной компании. Стоимость для склада фиксированная (500 руб.), для терминала - вычисляется по тарифам транспортной компании. Вывоз с терминала предлагается с ближайшего терминала к выбранному городу.

**Курьерская доставка** доступна для любого города. Стоимость рассчитывается по фиксированному тарифу для Санкт-Петербурга или по тарифам транспортной компании для остальных городов.

**Задачи:**
- ~~Прототип страницы~~
- Улучшение дизайна страницы
- [Интеграция с api транспортной компании](https://github.com/springhead-su/presswall/issues/4)

### 3. Контактные данные
Вводятся данные контактного лица, независимо от того, физ. или юр. лицо оформляет заказ. Дополнительно можно указать данные получателя (если принимать заказ будет другой человек).

**Задачи:**
- ~~Прототип страницы~~
- Улучшение дизайна страницы
- Дизайн галочки

### 4. Способы оплаты
Онлайн оплата осуществляется через систему электронных платежей payanyway. Возможно выбрать из трех основных опций:
1. Банковская карта
2. Электронные платежи
3. Банковские системы
Все опции переводят на сайт payanyway на соответствующие страницы с выбранным видом платежной системы.

Для юр. лиц доступна оплата по безналичному расчету. При выборе предлагается заполнить дополнительную информацию, необходимую для оформления документов.

**Задачи:**
- ~~Прототип страницы~~
- Улучшение дизайна страницы
- [Интеграция с api payanyway](https://github.com/springhead-su/presswall/issues/11)

### Проверьте ваш заказ
Выводится только при выборе онлайн оплаты для дополнительной проверки и перехода на сайт платежной системы. При выборе оплаты по безналичном расчету не показывается

**Задачи:**
- ~~Прототип страницы~~
- Улучшение дизайна страницы

### Заказ оформлен
Показывается после онлайн оплаты или после оформления заказа при выборе оплаты по безналу. При выборе оплаты по безналу предлагается скачать необходимые документы.

**Задачи:**
- ~~Прототип страницы~~
- Улучшение дизайна страницы
- Формирование документов для юр. лиц
