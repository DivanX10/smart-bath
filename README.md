## Проект "Умная ванна"
> Проект только на стадии развитии, всю цепочку событии можно наблюдать в чате [Умный дом с диваном](https://t.me/smart_home_divan). Умная ванна проект сложный и будет множество задач, которые нужно решить. Готовые решения будут публиковаться здесь. 

Я выражаю благодарность людям в своем чате, которые принимали участие в проекте умная ванна и без них этот проект бы не появился

Процесс сборки можете прочитать в разделе [Wiki](https://github.com/DivanX10/smart-bath/wiki)

**1) Что такое умная ванна и зачем нужна умная ванна?**

Умная ванна это полностью автоматическая ванна, которая управляется через умный дом на платформе Home Assistant, а также может управляться через голосовой помощник Алиса. С развитием умного дома я ищу что-то новое, то, чего прежде не было у меня. Хочется, чтобы умный дом был по истинне настоящим умным домом и не хочется ограничиваться освещением, климатом и охранной системой. Умный дом должен расширяться во всех сферах насколько это возможно. Умная ванна это удобно и круто. Представьте, что вам надо искупать детей, сказали, Алиса, приготовь ванну детям и запустится процесс приготовления ванны. При наполнении ванны будет добавлена пена и вода наполнится до половины уровня ванны, а после сообщит детям, что ванна готова. Цветовой индикатор в ванне будет показывать какая температура воды, чтобы визуально можно было понимать какая температура воды. Если решили сами полежать в горячей ванне, то как только ляжем, ванна поймет, что человек лег в ванну и начнет наполнять воду.

Для понимания можете посмотреть [видео автора](https://youtu.be/_B7byL6H7NE), который собрал автоматизированную ванну и которым я вдохновился

**2) Что умеет умная ванна?**
* Автоматически смешивать горячую и холодную воду
* Автоматически закрывать и открывать сливной клапан
* Автоматически наполнять ванну до нужного уровня по просьбе голосового помощника Алиса или когда человек лег в ванну
* Автоматически сливать воду в ванной
* Автоматически делать мойку ванны после мытья
* Регулировать напор воды
* Регулировать температуру подаваемой воды
* Добавить горячей воды, если долго лежим в ванне и вода немного остыла. Будет частичный слив воды и добавление новой порции горячей воды
* Иметь аварийное выключение всей системы на случай протечки
* Опционально можно добавить адресную светодиодную ленту для индикации температуры или готовности ванны
* Опционально можно добавить управление ванной через планшет
* Опционально можно добавить добавление пенки в воду при наполнении ванны


## Схема умной ванны
![image](https://user-images.githubusercontent.com/64090632/192654137-efa8b03f-fac0-4592-8547-d73852db96e2.png)

## Комплектующие для сборки умной ванны
> Важно! Не все комплектующие приобретены и не все комплектующие пока доехали до меня. Некоторые комплектующие могут меняться в ходе опытных проб. По мере публикации готовых работ,   

<details>
  <summary>1) 8 канальное реле zigbee (в налиичии)</summary>

* Подробная статья о [Zigbee реле на 8 каналов](https://modkam.ru/2020/06/24/zigbee-rele-na-8-kanalov/)    
* 8 канальное реле zigbee можете заказать у Григория https://t.me/avenit
* [Видео обзор](https://youtu.be/ytuvblyAoo0) Modkam - 8х канальное Zigbee реле с сухими контактами, подключение внешних датчиков на канале [Alex Kvazis - технологии умного дома](https://www.youtube.com/c/AlexKvazis/videos)


![image](https://user-images.githubusercontent.com/64090632/192657403-07199f10-7540-4328-8489-d425c8b7775a.png)
</details>

<details>
  <summary>2) Электропривод поворотный TIM M030101DAB для трехходового клапана для смешивания горячей и холодной воды</summary>

Электропривод поворотный TIM M030101DAB брал [здесь](https://www.ozon.ru/product/servoprivod-dlya-krana-raspredelitelnogo-230v-dlina-provoda-1-5m-tim-485927636/?sh=LmakeLtZzw)
  
![image](https://user-images.githubusercontent.com/64090632/192656548-7994fcb8-eee7-489b-8e65-1ba55ecb0bae.png) 
</details>

<details>
  <summary>3) Cервопривод MG945 для управления сливным клапаном</summary>

Сервопривод MG945 для управления сливным клапаномc мощностью 12 кг брал [здесь](https://www.ozon.ru/product/716305913/?sh=LmakeJH9iQ&utm_campaign=productpage_link&utm_medium=share_button&utm_source=smm)
  
![image](https://user-images.githubusercontent.com/64090632/196492259-8ebf9d65-8b5d-4a3e-9800-b8ff98b79a33.png)
</details>

<details>
  <summary>4) Датчик допплера MH-ET LIVE HB100 X для обнаружения человека когда ложимся в ванну</summary>

Датчик допплера MH-ET LIVE HB100 X брал [здесь](https://aliexpress.ru/item/4000322455586.html?sku_id=10000001320564017)  
![image](https://user-images.githubusercontent.com/64090632/192656809-0863d89c-ee09-4609-ba43-86564644a7c5.png) 
</details>

<details>
  <summary>5) Бесконтактный датчик воды XKC-Y25-V для определения уровня воды</summary>

Бесконтактный датчик воды XKC-Y25-V брал [здесь](https://aliexpress.ru/item/1005004165856762.html)
  
![image](https://user-images.githubusercontent.com/64090632/192657537-5ab68d17-e48e-4437-9812-e38bf0d3c265.png) 
</details>

<details>
  <summary>6) Водосчетчик с герконом (не с НАМУР) для учета наполняемой воды с точностью 1 импульс - 1 литр</summary>

[ВСГД-15-03 (110ММ) СЧЕТЧИК ГОРЯЧЕЙ ВОДЫ С ИМП. ВЫХОДОМ](https://www.teplovodomer.ru/catalog/schetchiki-vody/kvartirnye-schetchiki-vody/dn-15/vsgd-15-03-110mm-schetchik-goryachey-vody-s-imp-vykhodom/)
  
![image](https://user-images.githubusercontent.com/64090632/192657779-d00d83ee-c861-42b2-b6bb-bdf51c3c5589.png)
</details>

<details>
  <summary>7) Электрический моторизованный шаровой кран для регулировки напора воды, а также открыть и закрыть воду</summary>

* Электрический моторизованный шаровой кран [брал здесь](https://aliexpress.ru/item/1005003224042573.html)
* Обзор [FrankEver FK_V02 - Zigbee кран с регулировкой открытия](https://youtu.be/lpL6xAYuBHk) можете посмотреть на канале [Alex Kvazis - технологии умного дома](https://www.youtube.com/c/AlexKvazis/videos) 
  
![image](https://user-images.githubusercontent.com/64090632/192659320-4b3b5dd5-483d-4699-8dbc-d6b365cdba43.png)

</details>

<details>
  <summary>8) Фильтр грубой очистки воды</summary>
  
![image](https://user-images.githubusercontent.com/64090632/192660219-284d3fc0-cb62-4c2f-b3c6-9856c4ec553d.png)

</details>

<details>
  <summary>9) Обратный клапан воды</summary>
  
![image](https://user-images.githubusercontent.com/64090632/192660369-6822061b-97f1-402a-ac70-8df9bbcf4021.png)

</details>

<details>
  <summary>10) Сифон для ванны AlcaPlast click/clack с плоским переливом A564CRM1-80. Сифон со встроенным фитингом, что позволяет подключить шланг с водой и наполнять ванну водой</summary>
  
![image](https://user-images.githubusercontent.com/64090632/193369955-59d2433c-1ce4-4595-8ef1-300d29481631.png)
![image](https://user-images.githubusercontent.com/64090632/193598027-856c0aab-c638-48da-ba7b-72a89a028073.png)

</details>

<details>
  <summary>11) Датчик температуры воды DS18B20 и адаптер питания</summary>

Датчик температуры воды DS18B20 и адаптер брал [здесь](https://aliexpress.ru/item/32467815969.html)
 
![image](https://user-images.githubusercontent.com/64090632/193369539-cd92100a-f390-4632-967a-61bbaf779100.png)

</details>

<details>
  <summary>12) Тройник для погружного датчика температуры VALTEC VTr.136.N.0504 3/4"x1/2"x3/4" + гильза для погружного датчика температуры 1/2" х 90 мм</summary>
  
![image](https://user-images.githubusercontent.com/64090632/192899430-7c4f0223-c60c-4653-bc85-b4f552903dae.png)
![image](https://user-images.githubusercontent.com/64090632/193655715-905d8579-7967-46d2-877f-6e4a8a24b8c0.png)
</details>

<details>
  <summary>13) Водонепроницаемые RGB светодиодные светильники</summary>
  
![image](https://user-images.githubusercontent.com/64090632/203877488-9a497c8e-e171-4b6b-b3d2-c1cd6c4e800f.png)
![image](https://user-images.githubusercontent.com/64090632/203877522-753f2b87-1744-4478-af47-e08d086b3f1d.png)
</details>

<details>
  <summary>14) Дозатор для жидкого мыла для создание пены</summary>
  
![image](https://user-images.githubusercontent.com/64090632/203877661-acb3ff4f-6c31-49a0-9002-e1d74dd5e26b.png)
!![image](https://user-images.githubusercontent.com/64090632/203877689-87e4bb94-de79-4d88-9a56-d1e7825062f0.png)
</details>

<details>
  <summary>15) Умный автоматический выключатель Wi-Fi (Black with metering и Номинальная сила тока 10A)</summary>
  
![image](https://user-images.githubusercontent.com/64090632/203878317-1fdb70c9-fe10-445e-80d4-3c7b9df02adc.png)
![image](https://user-images.githubusercontent.com/64090632/203878353-7c6a4a11-de47-4112-bb7f-5ac052164d0b.png)
</details>

<details>
  <summary>16) Корпус пластиковый ЩУРн-П 1/8 IP66 PC LIGHT IE </summary>
  
![image](https://user-images.githubusercontent.com/64090632/203879020-69830bfe-a10a-4863-ae44-48cd6c047678.png)
![image](https://user-images.githubusercontent.com/64090632/203878353-7c6a4a11-de47-4112-bb7f-5ac052164d0b.png)
</details>

<details>
  <summary>17) Счетчик горячей воды Ителма WFW23.D080.1L с импульсным выходом НАМУР (L 80 мм, Ду 15 мм, вес импульса 1 л)</summary>
  
![image](https://user-images.githubusercontent.com/64090632/203879120-a62e9da2-572c-48c4-a6b1-beebca45a368.png)
</details>

<details>
  <summary>18) Шина нулевая в корпусе (2х7) EKF PROxima </summary>
  
![image](https://user-images.githubusercontent.com/64090632/203879179-6362642a-89cd-4826-a88e-2325660330a5.png)
![image](https://user-images.githubusercontent.com/64090632/203878353-7c6a4a11-de47-4112-bb7f-5ac052164d0b.png)
</details>

<details>
  <summary>19) Автоматический выключатель 1P 10А (C) 4,5kA ВА 47-63, EKF PROxima </summary>
  
![image](https://user-images.githubusercontent.com/64090632/203879262-502dbb28-1d8f-4bc0-8a40-a2403bbc5d7c.png)
![image](https://user-images.githubusercontent.com/64090632/203878353-7c6a4a11-de47-4112-bb7f-5ac052164d0b.png)
</details>

<details>
  <summary>20) Устройство защитного отключения УЗО ВД-100 2P 16А- 10мА (электромеханическое) EKF PROxima</summary>
  
![image](https://user-images.githubusercontent.com/64090632/203879310-1fe71995-e9cb-4ae5-87eb-97ca8c785ec7.png)
![image](https://user-images.githubusercontent.com/64090632/203878353-7c6a4a11-de47-4112-bb7f-5ac052164d0b.png)
</details>

<details>
  <summary>21) Источник питания Mean Well MDR-40-5 </summary>
  
![image](https://user-images.githubusercontent.com/64090632/203879355-1879a6cd-47f0-451e-8874-6689c67a4795.png)
![image](https://user-images.githubusercontent.com/64090632/203878353-7c6a4a11-de47-4112-bb7f-5ac052164d0b.png)
</details>

<details>
  <summary>21) Zigbee RGB контроллер Gledopto GL-C-007-2ID для управление подводными светодиодами </summary>
  
![image](https://user-images.githubusercontent.com/64090632/210140992-d51d825f-06ad-4ec4-aecf-3093721a6403.png)
</details>



## Стоимость комплектующих. Указаны цены, которые я потратил на комплектующие в сентябре- декабре 2022 года
1) 8 канальное реле zigbee 1шт. - 3900 руб.
2) Программатор для реле SmartRF04EB 1шт. - 990 руб.
3) Электропривод поворотный TIM M030101DAB для трехходового клапана 1шт. - 2 420 руб.
4) Трехходовой клапан BL3803 3/4 1шт. - 1 430 руб.
5) Сервопривод MG945 1шт. - 518 руб.
6) Датчик допплера MH-ET LIVE HB100 X 1шт. - 607,75 руб. Ссылка на [товар](https://aliexpress.ru/item/4000322455586.html)
7) Бесконтактный датчик воды XKC-Y25-V 2шт. 330,72х2 = 661,45 руб. Ссылка на [товар](https://aliexpress.ru/item/1005003652845339.html)
8) Электрический моторизованный шаровой кран для регулировки напора воды Tuya 1шт. - 5 267,26 руб. Ссылка на [товар](https://aliexpress.ru/item/1005003224042573.html)
9) Датчик температуры воды DS18B20 и адаптер питания 1шт. - 221,95 руб. Ссылка на [товар](https://aliexpress.ru/item/32467815969.html)
10) Сифон для ванны AlcaPlast click/clack с плоским переливом A564CRM1-80 1шт. - 10447 руб. Ссылка на [товар](https://alcaplast.com.ru/sifony/sifony-dlja-vanny/c-napuskom-vody-cherez-pereliv/a564crm1/)
11) Фитинг резьба тройник косой VALTEC VTr.136.N.0504 3/4"x1/2"x3/4" 1шт. - 833 руб. 
12) Гильза для погружного датчика температуры 1/2" х 90 мм Valtec 1шт. - 756 руб.
13) Модуль ESP8266-12F NodeMcu WeMos D1 mini 1шт. - 499 руб.
14) Водонепроницаемые RGB светодиодные светильники - 3704,59 руб. Ссылка на [товар](https://aliexpress.ru/item/32230854483.html)
15) Дозатор для жидкого мыла для создание пены - 308,30 руб. Ссылка на [товар](https://aliexpress.ru/item/1005004515025463.html)
16) Умный автоматический выключатель Wi-Fi (Black with metering и Номинальная сила тока 10A) - 1 124,18 руб. Ссылка на [товар](https://aliexpress.ru/item/1005004323726897.html)
17) Корпус пластиковый ЩУРн-П 1/8 IP66 PC LIGHT IEK - 1579 руб.
18) Счетчик горячей воды Ителма WFW23.D080.1L с импульсным выходом НАМУР (L 80 мм, Ду 15 мм, вес импульса 1 л) - 2038 руб.
19) Шина нулевая в корпусе (2х7) EKF PROxima - 405 руб.
20) Автоматический выключатель 1P 10А (C) 4,5kA ВА 47-63, EKF PROxima - 186 руб.
21) Устройство защитного отключения УЗО ВД-100 2P 16А- 10мА (электромеханическое) EKF PROxima - 1585 руб.
22) Источник питания Mean Well MDR-40-5 - 1615 руб. Ссылка на [товар](http://www.mean-well.ru/store/MDR-40-5/)
