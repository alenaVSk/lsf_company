# проект "Drive Avto-2"
Это информационная система для автосервиса (ведение учёта заказов и материалов) создана на платформе LsFusion как альтернатива приложению [‘Drive Avto’](https://github.com/alenaVSk/flask_sql_company) (Python, Flask, PostgreSql), 
но с улучшенной архитектурой и функционалом.

**_Разделы Программы:_**

### «Заказы» 
[«Журнал заказов»](https://github.com/alenaVSk/Photo_Image/blob/main/screenshot%20lsf_company/%D0%B6%D1%83%D1%80%D0%BD%D0%B0%D0%BB%20%D0%B7%D0%B0%D0%BA%D0%B0%D0%B7%D0%BE%D0%B2.png) (MODULE Customer):  регистрация заказов, вносятся данные о клиентах, их авто. 

«Реестр актов выполненных работ» ([1](https://github.com/alenaVSk/Photo_Image/blob/main/screenshot%20lsf_company/%D1%80%D0%B5%D0%B5%D1%81%D1%82%D1%80%20%D0%B0%D0%BA%D1%82%D0%BE%D0%B2%201.png), [2](https://github.com/alenaVSk/Photo_Image/blob/main/screenshot%20lsf_company/%D1%80%D0%B5%D0%B5%D1%81%D1%82%D1%80%20%D0%B0%D0%BA%D1%82%D0%BE%D0%B2%202.png)) (MODULE Statement): вносится вся необходимая информация о заказе (выполненная работа и использованные материалы, автоматический расчёт стоимости со скидкой и без,
автоматический ввод пользователя).

При просмотре Акта выполненных работ ([1](https://github.com/alenaVSk/Photo_Image/blob/main/screenshot%20lsf_company/%D0%B0%D0%BA%D1%82%20%D0%B2%D1%8B%D0%BF%20%D1%80%D0%B0%D0%B1%D0%BE%D1%82-1.png) , [2](https://github.com/alenaVSk/Photo_Image/blob/main/screenshot%20lsf_company/%D0%B0%D0%BA%D1%82%20%D0%B2%D1%8B%D0%BF%20%D1%80%D0%B0%D0%B1%D0%BE%D1%82-2.png)) с помощью инструкции DESIGN доработан дизайн формы.
Сформирован шаблон (редактирование jrxml-файла) ["Акт выполненных работ"](https://github.com/alenaVSk/Photo_Image/blob/main/screenshot%20lsf_company/%D0%90%D0%BA%D1%82%20%D0%B2%D1%8B%D0%BF%20%D1%80%D0%B0%D0%B1%D0%BE%D1%82.pdf).

### «Материалы»  
[«Приходные накладные»](https://github.com/alenaVSk/Photo_Image/blob/main/screenshot%20lsf_company/%D0%BC%D0%B0%D1%82%D0%B5%D1%80%D0%B8%D0%B0%D0%BB%D1%8B-%3E%D0%BF%D1%80%D0%B8%D1%85%20%D0%BD%D0%B0%D0%BA%D0%BB%D0%B0%D0%B4%D0%BD%D1%8B%D0%B5.png) (MODULE Receipt): вносятся данные о поступившем на склад товаре, автоматический расчёт итоговой суммы,  автоматический ввод пользователя и даты заполнения.

[«Текущие остатки»](https://github.com/alenaVSk/Photo_Image/blob/main/screenshot%20lsf_company/%D0%BC%D0%B0%D1%82%D0%B5%D1%80%D0%B8%D0%B0%D0%BB%D1%8B-%3E%D1%82%D0%B5%D0%BA%20%D0%BE%D1%81%D1%82%D0%B0%D1%82%D0%BA%D0%B8.png) (MODULE StockItem): автоматически выводятся остатки по каждому товару, т. е. по накладной товар принимается на склад, а по Акту вып. работ (раздел использованные материалы) 
товар списывается со склада.

### «Справочники»
[«Товары»](https://github.com/alenaVSk/Photo_Image/blob/main/screenshot%20lsf_company/%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BE%D1%87%D0%BD%D0%B8%D0%BA%D0%B8-%3E%D1%82%D0%BE%D0%B2%D0%B0%D1%80%D1%8B.png) (MODULE Item), [«Организации»](https://github.com/alenaVSk/Photo_Image/blob/main/screenshot%20lsf_company/%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BE%D1%87%D0%BD%D0%B8%D0%BA%D0%B8-%3E%D0%BE%D1%80%D0%B3%D0%B0%D0%BD%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D0%B8.png) (MODULE LegalEntity), [«Авто»](https://github.com/alenaVSk/Photo_Image/blob/main/screenshot%20lsf_company/%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BE%D1%87%D0%BD%D0%B8%D0%BA%D0%B8-%3E%D0%B0%D0%B2%D1%82%D0%BE.png), [«Работники»](https://github.com/alenaVSk/Photo_Image/blob/main/screenshot%20lsf_company/%D1%81%D0%BF%D1%80%D0%B0%D0%B2%D0%BE%D1%87%D0%BD%D0%B8%D0%BA%D0%B8-%3E%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%BD%D0%B8%D0%BA%D0%B8.png) (MODULE Employees).

В MODULE StockAccounting описано меню системы.
