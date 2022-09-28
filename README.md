## Проект "Умная ванна"
> Проект только на стадии развитии, всю цепочку событии можно наблюдать в чате [Умный дом с диваном](https://t.me/smart_home_divan). Умная ванна проект сложный и будет множество задач, которые нужно решить. Готовые решения будут публиковаться здесь. 

Я выражаю благодарность людям в своем чате, которые принимали участие в проекте умная ванна и без них этот проект бы не появился


**1) Что такое умная ванна и зачем нужна умная ванна?**

Умная ванна это полностью автоматическая ванна, которая управляется через умный дом на платформе Home Assistant, а также может управляться через голосовой помощник Алиса. С развитием умного дома я ищу что-то новое, то, чего прежде не было у меня. Хочется, чтобы умный дом был по истинне настоящим умным домом и не хочется ограничиваться освещением, климатом и охранной системой. Умный дом должен расширяться во всех сферах насколько это возможно. Умная ванна это удобно и круто. Представьте, что вам надо искупать детей, сказали, Алиса, приготовь ванну детям и запустится процесс приготовления ванны. При наполнении ванны будет добавлена пена и вода наполнится до половины уровня ванны, а после сообщит детям, что ванна готова. Цветовой индикатор в ванне будет показывать какая температура воды, чтобы визуально можно было понимать какая температура воды. Если решили сами полежать в горячей ванне, то как только ляжем, ванна поймет, что человек лег в ванну и начнет наполнять воду.

Для понимания можете посмотреть [видео автора](https://youtu.be/_B7byL6H7NE), который собрал автоматизированную ванну и которым я вдохновился

**2) Что умеет умная ванна?**
* Автоматически смешивать горячую и холодную воду
* Автоматически закрывать и открывать клапан сливного горлышка
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

<details>
  <summary>1) 8 канальное реле zigbee </summary>

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
  <summary>3) Высоковольтный водонепроницаемый цифровой сервопривод для управления сливным клапаном</summary>

Сервопривод для управления сливным клапаном брал [здесь](https://www.ozon.ru/product/1-sht-vysokovoltnyy-vodonepronitsaemyy-tsifrovoy-servoprivod-dlya-1-5-rc-car-270-servo-472364958/?sh=LmakeEw5CQ)
  
![image](https://user-images.githubusercontent.com/64090632/192656635-4c047420-3049-45ad-9ed8-549f2db25a93.png)
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
  <summary>10) Сифон для ванны AlcaPlast click/clack с плоским переливом</summary>
  
![image](https://user-images.githubusercontent.com/64090632/192660484-38635c69-d8d7-4c42-8599-c589df34f7c1.png)

</details>








