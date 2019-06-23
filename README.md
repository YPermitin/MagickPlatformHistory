# История изменений версий прикладных программ и технологической платформы 1С

## Общие сведения

Репозиторий содержит информацию об истории изменений версий прикладных программ и технологической платформы 1С:Предприятие.
Источником данных является сайт [releases.1c.ru](https://releases.1c.ru/total).

> *Репозиторий содержит только историю изменений информации о релизах и не предлагает ссылки для скачивания программ и прикладных решений, а также другую закрытую информацию с сайта ИТС.*

## Как получена информация

Для получения информации используется учетная запись сайта [releases.1c.ru](https://releases.1c.ru/total) с ограниченными правами.
На момент создания репозитория, ресурс позволял зарегистрировать учетную запись без возможности загрузки обновлений, т.е. только для просмотра актуальных версий программ. Подписка ИТС или приобретение других платных услуг в этом случае не нужны.

Обновление информации в репозитории выполняется 1 раз в 30 минут. Такая периодичность, например, используется для обновления данных из RSS-лент в различном ПО (Microsoft Outlook и другое ПО).

## Структура репозитория

Структура репозитория следующая.

```text
|-- Data
  |-- <КатегорияПродукта>
    |-- History
      |-- <ИмяПродукта.json>
    |-- ActualReleases.json
    |-- CategoryInfo.json
  |-- LastUpdates.json
|-- Readme.md
```
### Общее описание файлов:


#### "ActualReleases.json"

Cодержит информацию об актуальных релизах продуктов в данной категории:
  - Имя и идентификатор категории
  - Количество актуальных релизов
  - Список актуальных релизов с полями
    - Имя (Name)
    - Версия (Version)
    - Дата публикации (PublishingDate)
    - Плановые версии (PlanVersions)
    - Плановые даты публикации (PlanReleaseDates)
    - Плановые даты аткуализации данных о будущих релизах (PlanUpdateDates)
    - Демоверсии (DemoVersions)
    - Даты публикации демоверсий (DemoPublicationDates)

#### "CategoryInfo.json"

Описывает основную информацию о категории продуктов:
  - Имя и идентификатор категории.
  - Дата последнего обновления.
  - Количество и список продуктов в категории.

#### "<ИмяПродукта.json>"

В каталоге "Data/<КатегорияПродукта>/History" файл "<ИмяПродукта.json>" содержит:
  - Имя продукта
  - Имя и идентификатор категории
  - Количество изменений информации о продукте
  - Историю изменений информации по продукту в виде версий с полями:
    - Дата создания версии (Created)
    - Имя (Name)
    - Версия (Version)
    - Дата публикации (PublishingDate)
    - Плановые версии (PlanVersions)
    - Плановые даты публикации (PlanReleaseDates)
    - Плановые даты аткуализации данных о будущих релизах (PlanUpdateDates)
    - Демоверсии (DemoVersions)
    - Даты публикации демоверсий (DemoPublicationDates)

#### "LastUpdates.json"

Содержит информацию о последних релизах программ и прикладных решений, которые были выпущены за последнюю неделю.

Таким образом, вся информация содержится в каталоге "Data" и разбита по категориям.

## Отказ от ответственности

Вся информация предоставляется "КАК ЕСТЬ". Автор не несет ответственности за качество предоставляемых данных и их актуальность. Использование информации из репозитория полностью на Вашей ответственности.
