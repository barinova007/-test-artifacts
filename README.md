## Software Testing Theory Artefacts Learning
## Checklits | Test Cases | Test Plans | Guidelines
## [Example test mobile app](https://docs.google.com/spreadsheets/d/1YuOpm79UTRarMca3SJemUNqsV_EbuBto2jqiJwU_oJk/edit#gid=0)
## [Example test web form](https://docs.google.com/spreadsheets/d/1hQ2HydWC6TTq-EW03Oq4e7SlM1ttk5vdEoFIT0t6sJQ/edit?usp=sharing)
## [Example test security](https://www.notion.so/rmrhrcc/web-fd0c49b8644a4574a42502a7609e07f5)
## [Pairwise testing](https://docs.google.com/spreadsheets/d/1YzZ33UqtofIPG5CnsnrHnUxYlOzZW8xbFq9DXh7JhSI/edit#gid=0)


1. Чек лист проверок мобильного приложения, минимум 50 пунктов. Можете сделать отдельные чек листы для проверки конкретных мобильных приложений (Банковское приложение, игра, фитнес, фото, и т.п.)
2. Чек лист iOS App Store Review Guidelines, 15-20 кейсов - https://developer.apple.com/app-store/review/guidelines/
3. Список обновлений iOS release notes, 15-20 кейсов - https://developer.apple.com/documentation/ios-ipados-release-notes
4. Чек лист iOS guidelines, 15-20 кейсов -  https://developer.apple.com/design/human-interface-guidelines/ios/overview/themes/
5. Чек лист по дизайну Android приложений  15-20 кейсов - https://developer.android.com/docs/quality-guidelines/core-app-quality
6. Чек лист качества Android apps 15-20 кейсов - https://developer.android.com/quality



## Для ознакомления:
+ Политика Google Play по монетизации приложений - https://playacademy.exceedlms.com/student/collection/263275/path/345743/activity/345721
+ Политика Google Play по спаму -  https://playacademy.exceedlms.com/student/collection/263275/path/345743/activity/345720
+ Правила для мобильных Андройд приложений. (English) - https://play.google.com/about/developer-content-policy/

+ App Annie - сайт по аналитике мобильных приложений среди айос/андроид.

## Атрибуты:
1. Какой тип мобильного приложения.
2. Выбираем мобильные устройства, которые наиболее подходят.
3. Инструменты (эмуляторы, симмуляторы)
4. Особенности мобильного тестирования.
  
 # 1
+ ВЕБ - прижожение работает через вебсайт, адапритованый под девайс сайт (новостные). Могут функционировать на любой ОП их легче поддерживать. Нет доступа у устройству пользователя, ф-ции могут быть ограничены, через сеть, низкая безопастность Хром позволяет поставить оп в обход оф магазина. Контейнер. Установка на устройство.
+ ГИБРИДНОЕ- как и нативные, одна кодовая база на Джава Скрипт. Реакт, Пайтон Киви, Флаттер, какой то ф может не подднрживаться может отличаться ИФ; Как так? Разные версии одного и того же приложения - бранчи, ветвления.
Выглядят на как нативные, а работают в рамках веб. Их можно найти в сторах.
Все ф. не связанные с железом программируються на стороне сервера (вычисления), на стороне клиента только минимум (оболочка).
Соц.сети - инст, фб, тви.
Обладают большей ф, могут работать с несколькими платформами. Может не быть полного ф., необходимо соответствовать требованиям магазинов.
+ НАТИВНЫЕ - мп, которое создаёться для определенной платформы, когда нужна высокая производительность: кодировано под одну операционную систему (свифт - аййос), (котлин - андроид), со стора качаем, есть доступ к адрессной книге. (Блокнот, калькулятор) может работать без интернета. Стабильное, геоданные, помогают собирать статические данные. Недоставт: дороже в разработке, для поддержки надо выкладывать обновления. 
+ PWA - Progressive Web Application - то что можно открыть с помощью браузера, свайпнуть, отработывает логику мобилки;

+ Категории: игры, бизнес, образование, лайфстайл, развлеткательные, утилиты, путишевствия. От категории зависит объем проверок.

 # 2
## Как выбрать мобильное устройство, на чём тестировать фичи и прогонять девайсы?:
+ Во внимание разрешения экрана, версии и платформы, производительность и вендоры.
+ Актуальная статистика, если приложение уже релизнуто, то лучшей статистой будет ст-ка. с самого приложения,какие девайсы и поддерживать такие же девайсы у себя. Или популярные девайсы на мировом рынке. (AppMetrica, statconnter, appsee, app annie, app Brain, Kantar)
+ Cоздать таблизу с девайсами.

 # 3 
 ## Эмуляторы и симмуляторы
 Проблема моб тестирования - большой выбор моб. девайсов. Эмуляторы - для ондроид. Симуляторы - для айос.
 Не учитывают нагревы батареи. Могут не корректно сработать.
 Мобильные фермы - удаленные станции.

# 4
## Стратегия по мобильному тестировнию:
I sliced up fun! 
+ Вводы на девайс с клавиатуры, синхронизация с другими приложениями, ориентация (подставка, лежит), жесты нажатия, портрет и лаандшафт. Юзер кейсы - крутим, носим, нативные клавиши, подключаемость кравиатуры.
+ Store - требования магазинов, что юзер был залогинен, логотипы для стора, корректная работа магазинов с сертификатами, проверка билдов, которіе в стори, обновления через магазин на новую вкрсию. Если сделали ребрендинг, то это новое приложение, делаем новые проверки даже если оно идентично. На соотрветсвие требованиям магазина: не должно распостонять контент для взрослых.
+ Location - смена вайфай на моб соединение, ограничения контента от страны нахождения, роуминги: симна одной страны, нахождение в другой (проверка через ВПН)Нюансы провайдеров. Смена часовых поясов 29 февраля. Лицензии. Конфигурации.
+  Interactions/Interruptions - проверка приложения, когда с ним работают другие приложения одновременно, запуск ютуб и запуск нашего приложения. Изменения настроек, уведомления, сможем ли вернуться в приложение. Если календарю разрешим уведомлять, то сможем ли кликнув на уведомление открыть приложение.
+  Communication - взаимодейсвие и интеграция с другими приложениями, с библиотеками, реакиция на звонки, голосовые, почты, видео, работа с микрофоном, подключения и оключения наушников, работа с браузерами, соцсети.
+  Ergonomics - нажания, не маленькие ли буквы, шрифты, не слишком маленькие, удобно ли нажимать. работа с данными (символы какие можно ввести), медиафайлы, форматы, обновления как часто. Например открыто два приложения на одном экране, кнопка съехала
+ Usability - дискомфорт юзера, это ротация девайся и съехали кнопки
+ Data - работа с данными, спецсимволы, работа с медиафайлама, формат данных, как приложение реагирует на обновления.
+ Платформы  - кнопка back у Андроида, на ней могут быть баги; у ios imessage как через эту ф предать в сообщение линк; работа с виджетами, что видит пользователь; разные версии платформ, может быть ограничеснный фуе.
+ Функции - проверка всех ф приложения, заполняем каждое поле, какие чаще истользуються, какие нет, какие не удобные.
+ Юзер сценарии - как юзер может пользоваться нашим приложением.
+ Работа с сетью - если сеть стабильна и нет, с вайфай на мобильную, что будет происходить с картинкой. Скачки, закономерности, подойти/отойти.
+ Ориентация - Что происходит когда меняеться ориентация? перерисовыеться графика, страрый экран в новом расположении.Каждая последующая кнопка, все экраны удаляються, и прорисовка экранов поновой. Когда не надо переворачивать? всегда надо чтобы проверить как сработает в портретном и горизонтальном, как работать приложухе когда ты лежишь? Инст только - вертикально, кроме видео; Гайдлай - сейзон (как размещать), кнопочки, чтобы попадали пальчики.Строка состоянияА должен ли он отрисовываться горизонтальный/портретную?Как себя поведёт если перейдет из портретного в альбомный. мобильные игры - только горизонтальные, кейс. когда тел в вертикаль, кейс = и там и там она должна открыться горизонтально. при отключенном кнопке ориентации - всё равно включиться горизонтально.при прерывании., перевороты переложения, на 180, 360 а если лежишь.как отрабптывают тесты с героскопом (тест по осям) Перерисовка активити.

+ Ландшафтная/Портретная. Пеперисовка и сброс, как активити (графика) отработывает при смене ориентации; Например, особенности работы айос/андроид. 
  + Кейсы на ориентацию:
  + Запустить приложение на портретной ориентации
  + Запустить приложение на альбомной ориентация
  + Запустить приложение на портретной ориентации и поменять на альбомную
  + Запустить приложение на альбомной ориентация и поменять на портретную
  + Запустить приложение на портретной ориентации и поменять на альбомную при заблокированной портретной ориентации на уровне приложения
  + Запустить приложение на альбомной ориентация и поменять на портретную при заблокированной албомной ориентации на уровне приложения
  + Запустить приложение на портретной ориентации и поменять на альбомную при заблокированной портретной ориентации на системном уровне
  + Запустить приложение на альбомной ориентация и поменять на портретную при заблокированной албомной ориентации на системном уровне

+ Установки - с нуля, обновить, новую версию удалить, поставить старую версию-удалить, сохраниться ли прогресс после обновлений, +покупки из платного контента -УДАЛЕНИЕ-УСТАНОВКА-ПРОВЕРКА ОБНОВЛЕНИЙ- Уточнить какие оси ОП задействованы? напримео 15.1.1Кейс установки мобильного приложения: Чему дллжно соответствовать моб приложение перед релизом? Проверить лигал по безопасности? гайдлайны.разные оес, пуши, пририывание, обновы, фейс айди, поворот экрана подтвержение смс транзакции - автоматическая, предоставить доступ присылать сообщения, сенсоры, фотик, блокирование экрана.
+ Прерывания - пуши, звонок, сел заряд, будильник, подключение гарнитуры, включение фронтальной камеры, GPS,карта памяти отключилась, горизонтальное и вертикальная раскладка, сворачивание.
+ Реконнект - работа с 3 дж, 5 дж, вайфай, маршрутизатор, смена симок, переключение между вышками, работа в фоновом режиме.
+ Догрузки - какое событие вызывает догрузку, а в это время сел телефон, вай фай или моб интернет.
+ Покупки - Будут ли отображаться прогресс из бесплатной версии в платной? а если подписка закончилась не хватает денег на карте? если на карте нет денег, прийдет оповещение? надо проверить трекнуть и ему вернёться ему всё то, что было до оплаты?Платёжные системы, вернуть деньги (РЕФАН) Система оплат NFC- виртуальная карточка, как рамплачиваться; 7 дней бксплатно, а потом спишуться деньги, как тестить?Ответ: прокруть с программистом эти 7 дней..
+ Аутенфикации - почта, палец, фейс айди (как обмануть фейс айди - напечатать лицо), соушил логин, по номеру телефона, в приват есть: один раз регаешься и один пароль для всех, по кьюар коду в вайбере, секретный вопрос.
+ Валидация на чкловека: выбрать самолёты, роботы.
+ Тротлинг (чего?) торможение сети - менять нестабильное приложение, запросы на обновление ленты.
+ Тротлинг процессора - грееться, приложухи медленно, Почему это важно? ПЕРОМЕТР - померять это дело. Зачем проверять СКОРОСТЬ НАГРЕВА? чтобы понять как, денатурация белка 42 градуса, чтобы снизить нагрузку (понизить тактовую частоту - тротлить) Понимать средние ткмпературные режимы. В чехле или без чехла.
+ Проверка производительности - ФПС,какие девайсы какие чаще используються у конкурентов у Вас.
+ Снифинг - ('нюхать' трафик, перехватить поменяю и отправлю) зайти в нетворк, там увижу, что происхолит с нттп запросами. (прокси включить, ИР указать, режим разработчика включить, доверять дейсвиям, подкючиться к той же сети, включить сертификат, траффик пустить через прокси) Галочку поставить - чтобы отклавливать траффик со всех хостов (*.*) 
+ Если приложение спршивает дотуп к контактам? к камере? микрофон? - отдельно проверить
+ Тач айти - на задней крышке, У Андроида - три кнопки, У Аййос - одна/свайп вверх.
+ Тест камеры - Скан карточки через фотик и возможность пересылать денюжку .
+ Тема темная/светлая - как отработывает прорисовка.
