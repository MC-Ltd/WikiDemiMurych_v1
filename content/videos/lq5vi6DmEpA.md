---
title: "⎡JSbook: 02.03⎦   JavaScript: От мифов к спецификации. Выражения"
date: 2023-09-07
tags: []
videoId: "lq5vi6DmEpA"
duration: "3:47:10"
views: 8361
likes: 268
comments: 36
---
# [⎡JSbook: 02.03⎦   JavaScript: От мифов к спецификации. Выражения](https://www.youtube.com/watch?v=lq5vi6DmEpA)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 07.09.2023 11:06  
**Тривалість:** 3:47:10  
**Перегляди:** 8361 · **Лайки:** 268 · **Коментарі:** 36
![thumbnail](https://i.ytimg.com/vi/lq5vi6DmEpA/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=lq5vi6DmEpA)
## Коментарі (30 · відповідей: 6)

**[@chikenmacnugget](https://www.youtube.com/channel/UCyWOOKPeKYrjDQcZqz0Gyiw)** *[07.09.2023 05:29](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgyzlkqciF3uAyUg_Nt4AaABAg) (ред. 07.09.2023 05:29)*

Начало: 1:12:18

---

**[@chikenmacnugget](https://www.youtube.com/channel/UCyWOOKPeKYrjDQcZqz0Gyiw)** *[07.09.2023 07:17](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgyQjWLe8mwx7POAwCV4AaABAg) · 👍 2*

2:41:31 про объединение в группу выражений следующих после && оператора звучит как оговорка. То что показано в качестве подтверждения в спецификации не вносит никаких прояснений на счет объединения в группу. Если бы происходило объединение после &&, то в таком случае логично было бы предположить, что последующие выражения также не выполнятся в силу выхода на моменте с false. Как мне видится это выражение выглядит для интерпретатора так ( ( (false) && (theThing = 10) ) || (theThing = 30) ). В таком случае все становится куда понятнее и поведение выглядит ожидаемым. Прошу разобрать этот вопрос более точно, ибо не понятно и складывается впечатление, что автор сам не уверен в произнесенном

> **[@cosecax](https://www.youtube.com/channel/UC5JcL1Ox8Ukj8Ma9-4DOm-w)** *[15.09.2023 10:57](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgyQjWLe8mwx7POAwCV4AaABAg.9uLxCk1plBx9ufwiu4fUym) (ред. 15.09.2023 10:57)*

> похоже на правду
> Если мы так напишем 
> var t = 0
> var a = [
>     1,
>     false && (t = 1) || true,
>     t
> ]
> console.log(a)
> 
> То t будет 0, т.е. не вычисляется. А в теории групп Мурыча, t =1 надо было бы вычислить, чтобы сравнить с правой частью

---

**[@Gazovchik](https://www.youtube.com/channel/UC2wZB1LFWK0E6RZA8wptKVQ)** *[07.09.2023 09:47](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgygATjYHLlrpyeHQQJ4AaABAg)*

Продолжение
Здорово



Всем Адекватности мира и добра

---

**[@kozlov_egor](https://www.youtube.com/channel/UCppmTn7mOa3WRkroYiPL81Q)** *[07.09.2023 10:35](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgyFTwJyMWR-rgxTsy94AaABAg)*

Шутка про "кто передаст" была очень к месту :)

---

**[@leon83935](https://www.youtube.com/channel/UCQWoq45oCaF2rcWStxBAnYA)** *[07.09.2023 14:28](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgxgfCBl35-zEg3Iaop4AaABAg) · 👍 8*

Мурыч - герой нашего времени

---

**[@Gazovchik](https://www.youtube.com/channel/UC2wZB1LFWK0E6RZA8wptKVQ)** *[09.09.2023 15:14](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgwsL0RIIJGHp7Ln6b14AaABAg) (ред. 09.09.2023 15:15)*

Всем привет

Макс, посмотрел 1-ый час, скажи
-
Ты в видео номер 2 собирался объяснять/показать
 структурирование данных
(вот эту нотацию, аналогии)
на практике
-
Ты забыл об этом и покажешь в одном из Следующих видео?
Или же ты передумал показать на практике?

(Или я что-то не так понял?)

---

**[@compampa](https://www.youtube.com/channel/UC-wCvZZ4lfzNR3PYRo-Cmtg)** *[10.09.2023 10:27](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgyoEVthRWhQMAxvUjl4AaABAg)*

Доброго времени суток. 
Раньше тоже мучался с вебками, камерами и прочими девайсами и софтинами. 
Очень помогла программка Camo studio, бесплатной версии более чем достаточно для того чтобы стримить видео с телефона. 
Попробуй скачать, да потыкать, может поможет) 
Будем чаще наблюдать твои лицевые заросли 😊

---

**[@Gazovchik](https://www.youtube.com/channel/UC2wZB1LFWK0E6RZA8wptKVQ)** *[12.09.2023 15:34](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgwvAdKYhxJWNhNBdRh4AaABAg) (ред. 12.09.2023 15:38)*

Максим,
услышал про спор с Тимуром (2:46)
и у меня вопрос - он ведь Не глупый парень....... -
Зачем ему что-то Доказывать - если можно /вместе/ Просто Посмотреть спецификацию языка??,,,,,,

---

**[@Gazovchik](https://www.youtube.com/channel/UC2wZB1LFWK0E6RZA8wptKVQ)** *[13.09.2023 13:20](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=Ugx6ZdcZzdI2rI368vl4AaABAg)*

Максим, после "завтра" прошло уже 6 дней,
Есть версии - когда будет Продолжение?.....

Сегодня ты в ТМ написал про день рождения
-
Сегодня, я так понимаю, однозначно нет,,,,,,,

Может посоветуешь Новичку 
(первый язык, и даже в js ещё плохо ориентируюсь)
пока что-то посмотреть /до Нового выпуска/
со своего или с чужого канала?......

---

**[@rgame_youtuber](https://www.youtube.com/channel/UC5s3H5CxnWzaStABgShgx7w)** *[13.09.2023 17:07](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=Ugxlhoe7lUE0aH-KCU54AaABAg) (ред. 13.09.2023 18:25) · 👍 2*

1:22:57 , считаю вопрос некоректен, в связи с тем что ответ строится на том какая последняя цифра присуще текущей системе исчисления, а поскольку за ранее о выбранной системе исчислении не было сказано то ответ может быть как  1, 2, 3, 4, 5, 6, 7, 8, 9, 10, A, B, C, D, E, F,  ...

> **[@sergeysizov4819](https://www.youtube.com/channel/UCCX7yIi9oetEcyg2GP_WJQg)** *[06.11.2023 07:22](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=Ugxlhoe7lUE0aH-KCU54AaABAg.9ubSYdvZXqP9wlSVgBDcTp)*

> ну он же сказал, что это шутка

---

**[@sovaz1997](https://www.youtube.com/channel/UCEmISd-h08N0MzukCz-HFGg)** *[30.09.2023 11:28](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgzqrC4x6JqtmN2ad-t4AaABAg) · 👍 1*

По поводу тараканов у края экрана - думаю можно изменить функцию направления, чтобы вероятности были не равными. И если таракан приближается к краям, вероятность движения за края должна быть минимальной, а на краю должна быть равна нулю. И вероятность должна постепенно меняться. Тогда возможно поведение тараканов будет достаточно естественным у краев. Думаю надо брать расстояние до края при выбранном направлении, каким-то образом строить вероятности для каждого направления (чтобы в сумме было 1) и выбирать направление исходя из этого.

---

**[@ArtemMindsurfer](https://www.youtube.com/channel/UCtApnkzZe-Bo6ZQd5CHeJXQ)** *[20.10.2023 05:42](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgyU4LItcMyy_nhxwQh4AaABAg) · 👍 2*

с одной стороны мне уже надоело слушать одно и то же, ибо ты повторяешь по 500 раз факты, с другой, я наверное их уже никогда не забуду)))

---

**[@ArtemMindsurfer](https://www.youtube.com/channel/UCtApnkzZe-Bo6ZQd5CHeJXQ)** *[20.10.2023 23:27](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgzIVshFUdlzYrDpwmV4AaABAg)*

офигеть, получается var do = (
() => (
(1)
 )
 ) 
это просто серия выражений ? меня это удивляет! 
это как шаги

---

**[@andreykrist5290](https://www.youtube.com/channel/UCSI5BmuBGxR5v4S_sodK0bA)** *[31.10.2023 21:19](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgxeU2JLcoWJnWC0LPZ4AaABAg) · 👍 1*

Дуже дякую за такий контент !

---

**[@sergeysizov4819](https://www.youtube.com/channel/UCCX7yIi9oetEcyg2GP_WJQg)** *[06.11.2023 15:56](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgyoOUapXgffOdO9xFB4AaABAg) (ред. 07.11.2023 04:26) · 👍 12*

Таймкоды:
00:00 - 07:38 - ожидание начала
07:39 - 8:05 - тема трансляции
8:05 - 21:28 - благодарности
21:29 - 23:52 - антидисклеймер
23:54 - 33:35 - О чем был первый раздел: js - скриптовый язык. js и хост среда
33:36 - 35:25 - js - скриптовый язык: что есть и чего нет
35:26 - 57:49 - О чем был второй раздел: js: структурирование информации
57:50 - 1:02:24 - музыкальная пауза
1:02:24 - 1:12:16 - вопрос про структурирование информации и прототипное наследование
1:12:17 - 1:17:54 - Второй раздел: выражения
1:17:55 - 1:19:45 - пауза
1:19:47 - 3:06:08 - выражения
3:06:09 - 3:11:48 - итоги по сказанному
3:11:49 - 3:18:20 - О чем будет третья глава
3:18:21 - 3:25:09 - вопрос про связывание внутри стрелочной функции
3:25:10 - 3:31:19  - общение
3:31:20 - 3:32:26 - java и javascript, почему от java тупеют
3:32:27 - 3:36:30 - проблема с каждым собеседованием
3:36:31 - тараканы мои тараканы

---

**[@AroseySairon](https://www.youtube.com/channel/UCx3PjUd8HV-rXyxAL6ONPtw)** *[28.11.2023 03:02](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgzaXtSxMFFBYQ_YV6x4AaABAg)*

хахахахахах найс жучки на заставке. я в нокауте 😂

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[30.11.2023 23:31](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgzaXtSxMFFBYQ_YV6x4AaABAg.9xddGH4uFLu9xkzS_4IQMA)*

> Это лучшая программа в моей жизни

---

**[@ccjx_space](https://www.youtube.com/channel/UC6fpsI8tX4S9RZy8vPhowxQ)** *[08.12.2023 07:34](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgyzZSNZcTy12hiKnUx4AaABAg) (ред. 08.12.2023 18:15) · 👍 1*

🙏🙏🙏🙏 исцеление любопытства ❤❤❤ На ваших трансляциях происходит что-то невероятное. Сейчас так очень мало кто рассказывает, если рассказывают вообще. Потому что не умеют конечно. Чтобы прийти к вашему уровню повествования или преподавания нужны качества, человеческие качества которых многим из нас не хватает. Спасибо, что пытаетесь нас поправить, мы постараемся

---

**[@raff_m_d6971](https://www.youtube.com/channel/UCdsqd4Phl6ebcHNL1p1B5eg)** *[21.12.2023 18:44](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgywrrEr25BClgcKywp4AaABAg) · 👍 3*

Выражаю безграничную благодарность автору за контент

---

**[@fil-os-of](https://www.youtube.com/channel/UC0g87Mm8gKNwtFrzTY8LDkA)** *[27.12.2023 07:28](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgyBK4f0c4qMpw9rv3Z4AaABAg)*

Привет. У Миядзаки есть минимум 2 картины в которых мелькают сгусти разумной сажи:
1. Унесенные призраками (про приключения девочки попавшей в мир духов)
2. Мой сосед Тоторо (про двух сестер и духа леса)

---

**[@ДенисКулёмин-э1д](https://www.youtube.com/channel/UCUVbFS9_W4zZGlCaBwiXsuw)** *[27.12.2023 12:38](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgyXWrmczBuMPUSVJ8V4AaABAg) (ред. 27.12.2023 12:41)*

2:40:50
Подскажите, почему не выполнился theThing = 30  ?

> **[@blackFortuna1358](https://www.youtube.com/channel/UCw67yg8KaUK-21e5U5eXDdA)** *[22.02.2024 00:59](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgyXWrmczBuMPUSVJ8V4AaABAg.9ypLC3kex8KA05rWv6EeTN) (ред. 22.02.2024 00:59) · 👍 1*

> Потому что оптимизация. Условие с  =10 вернёт true-результат и нет смысла выполнять следующее

> **[@ДенисКулёмин-э1д](https://www.youtube.com/channel/UCUVbFS9_W4zZGlCaBwiXsuw)** *[22.02.2024 15:36](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgyXWrmczBuMPUSVJ8V4AaABAg.9ypLC3kex8KA07QtAALFht) (ред. 13.06.2024 23:30)*

> ​@blackFortuna1358
> Ааа, ну точно, благодарю, теперь понял
> =20 продолжило вычисляться потому что слева false а у нас или
> а =30 не вычисляется, потому что уже есть true

---

**[@jean_zfc](https://www.youtube.com/channel/UC_GbATs4nUTnXLrvO9NpWTQ)** *[28.12.2023 15:21](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgxHLCAQaLE9GUq1avJ4AaABAg) (ред. 09.01.2024 16:21) · 👍 1*

Автор запутал переводом одного и того же несколькими разными способами.

В спецификации есть два понятия expression и statement. Я бы Expression перевёл как выражение, а Statement как инструкция.
Все программы на языке JS состоят из инструкций, и все инструкции кроме составных инструкций разделяются точкой с запятой(в т.ч есть правила когда это делается автоматически, см.12.10.1 в спецификации).

и console.log("text"); и "asd"; и 5+7; с точки зрения парсера являются ExpressionStatement. ExpressionStatement это инструкция выражения, вид инструкции который в конечном итоге просто должен вернуть значение т.к когда интерпретатор видит выражение, он его вычисляет и заменяет выражение его значением.
Автор на протяжении всего видео использует слова команда, оператор(! и плевать что обычно этим словом называется другое понятие), выражение, инсутрукция... по отношению к одному и тому же. Возможно удалось бы избежать таких сложностей с названиями если бы вещи назывались так, как они называются на английском или был бы выбран один вариант перевода.

---

**[@jean_zfc](https://www.youtube.com/channel/UC_GbATs4nUTnXLrvO9NpWTQ)** *[28.12.2023 16:26](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgycSozvuS4QZFEJx7d4AaABAg) (ред. 09.01.2024 21:41)*

2:41:38 Нет. Ну и парсер мне показывает что для LogicalORExpression левым операндом будет LogicalANDExpression (false) && (theThing = 10), т.е выражение которое нужно так же вычислить. Левый операнд для LogicalANDExpression (false), а правый это выражения типа Assignment (theThing = 10), поскольку левый операнд возвращает false, интерпретатор не вычислит правый и выражение (false) && (theThing = 10) заменит значением левого операнда - false. После этого шага полагаю наше выражение будет выглядить как false || (TheThing = 20)

Ну и (false) && (theThing = 10) || (TheThing = 20) является одним составным выражением, и это естетсвенно что парсер его считывает целиком пытаясь преобразовать к так скажем максимально полной форме для интерпретатора.

---

**[@jean_zfc](https://www.youtube.com/channel/UC_GbATs4nUTnXLrvO9NpWTQ)** *[09.01.2024 22:02](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=Ugz0_0oAER8C11BMY0V4AaABAg)*

2:50:30 Этот пример со стракой так же неплохо отражает что такое структурирование информации(как это в части 2.02 назвалось). Типо мы не смогли найти для нашей строки проперти 1, будем искать в конструкторе строки, т.е у любой строки есть служебное поле которое ссылается на "нативный" объект String...

---

**[@Et47](https://www.youtube.com/channel/UCYr9X1Zuzj6x0LwhKNAe3jA)** *[16.01.2024 21:10](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=Ugzve6D07Hawx0XnUOR4AaABAg) · 👍 1*

Спасибо за подробнейшее объяснение основ - вам бы в Университете преподавать

---

**[@EugeneKoshelev](https://www.youtube.com/channel/UCgSr74nurSDE8fbBiSSyBsg)** *[30.01.2024 14:48](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgwMBJRXuC1KnwQo7vN4AaABAg)*

Глубокие вещи говорите, господа!

---

**[@EugeneKoshelev](https://www.youtube.com/channel/UCgSr74nurSDE8fbBiSSyBsg)** *[30.01.2024 15:01](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=Ugy1B9EproxJ7fvecgl4AaABAg) · 👍 1*

"В языке JS всё не то, чем кажется" - золотые цитаты Демимурыча))

> **[@EvilYou](https://www.youtube.com/channel/UCmEdFUN2gODWCHvETEX2zEw)** *[04.03.2026 13:51](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=Ugy1B9EproxJ7fvecgl4AaABAg.A-C8_bpGLQKATwFuAOdeDd)*

> В языке JS всё не то, чем кажется потому что мы программируем на языке, который сам по себе не существует. (c) Великий Мудрилыч

---

**[@EugeneKoshelev](https://www.youtube.com/channel/UCgSr74nurSDE8fbBiSSyBsg)** *[30.01.2024 15:02](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=Ugw0Zh7a7OPEnNZafax4AaABAg)*

"Язык JS сам по себе не существует".

---

**[@narek7281](https://www.youtube.com/channel/UCUa3U5-hu8KquLW_b1ubKbA)** *[02.07.2024 07:35](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgzAlVRcAaiUeSYSuGF4AaABAg)*

great video

---

**[@CooperHarry92](https://www.youtube.com/channel/UCyyO35vfJa8CDbuLSIUVd6g)** *[09.09.2024 21:17](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgzgT2L0x-o_ceS_CXd4AaABAg) (ред. 09.09.2024 21:23) · 👍 1*

2:50:25 осмелюсь поправить) в случае языка Си здесь не ошибка, а undefined behavior, строго в соответствии со стандартом языка Си) А в реальности просто выведем мусор со стекфрейма

---

**[@ВячеславШабаев-з7ю](https://www.youtube.com/channel/UCFH2XYGz04ODsqKoSM4ZYzg)** *[08.10.2024 22:52](https://www.youtube.com/watch?v=lq5vi6DmEpA&lc=UgzIovJxp2wJdOG7o8l4AaABAg) · 👍 1*

Мурыч - прекрасное чувство юмора и самоиронии)), один из лучших маркеров думающего и доброго человека! Нет слов, одни положительные эмоции, спасибо Тебе за атмосферу!!!))

---
