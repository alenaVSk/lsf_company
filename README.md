# проект "Drive Avto-2"
Это информационная система для автосервиса (ведение учёта заказов и материалов) создана на платформе LsFusion как альтернатива приложению [‘Drive Avto’](https://github.com/alenaVSk/flask_sql_company) (Python, Flask, PostgreSql), 
но с с улучшенной архитектурой и функционалом.

**_Разделы Программы:_**

### «Заказы» 
«Журнал заказов» (MODULE Customer):  регистрация заказов, вносятся данные о клиентах, их авто.

«Реестр актов выполненных работ» (MODULE Statement): вносится вся необходимая информация о заказе (выполненная работа и использованные материалы, автоматический расчёт стоимости со скидкой и без,
автоматический ввод пользователя).

При просмотре Акта выполненных работ с помощью инструкции DESIGN доработан дизайн формы.

### «Материалы»  
«Приходные накладные» (MODULE Receipt): вносятся данные о поступившем на склад товаре, автоматический расчёт итоговой суммы,  автоматический ввод пользователя и даты заполнения.

«Текущие остатки» (MODULE StockItem): автоматически выводятся остатки по каждому товару, т. е. по накладной товар принимается на склад, а по Акту вып. работ (раздел использованные материалы) 
товар списывается со склада.

### «Справочники»
«Товары» (MODULE Item), «Организации» (MODULE LegalEntity), «Авто», «Работники» (MODULE Employees).

В MODULE StockAccounting описано меню системы.
