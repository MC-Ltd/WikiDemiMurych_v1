---
title: "JavaScript и идентификаторы. В рамках подкаста Tips and Tricks [Msk] [JavaScript шорты]"
date: 2023-05-13
tags: []
videoId: "biy50-ssgVQ"
duration: "15:08"
views: 3268
likes: 202
comments: 24
---
# [JavaScript и идентификаторы. В рамках подкаста Tips and Tricks [Msk] [JavaScript шорты]](https://www.youtube.com/watch?v=biy50-ssgVQ)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 13.05.2023 03:58  
**Тривалість:** 15:08  
**Перегляди:** 3268 · **Лайки:** 202 · **Коментарі:** 24
![thumbnail](https://i.ytimg.com/vi/biy50-ssgVQ/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=biy50-ssgVQ)
## Коментарі (16 · відповідей: 8)

**[@Fodintsov](https://www.youtube.com/channel/UCvIUqC8hxvctYDNWG-GeC5A)** *[13.05.2023 04:54](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgxezEHlc88XThx_xn54AaABAg) · 👍 3*

Короче, юзайте чистые функции без сайд-эффектов!

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[13.05.2023 07:12](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgxezEHlc88XThx_xn54AaABAg.9pdQriy8EhP9pdffGJPOMn) (ред. 13.05.2023 07:13) · 👍 5*

> Ты хотел сказать - используйте чистые функции, то есть это те функции, которые не содержат сайд эффектов. 
> И ты абсолютно прав.
> 
> Любой функциональный код, а именно этот код и характеризуется чистыми функциями, гарантировано оптимизируется любым компилятором. Это следует из парадигмы FP. И в данном случае V8 совершенно не исключение.
> У меня совсем это улетело из головы.
> 
> Большое спасибо за очень нужную ремарку.

---

**[@melonges7884](https://www.youtube.com/channel/UCjmS3b3jTdJ0i0Xaj4Kzhug)** *[13.05.2023 10:39](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgwnrVXjPQf5nTF6fOB4AaABAg) · 👍 1*

Я был в шоке!

---

**[@ThomasA-i7o](https://www.youtube.com/channel/UCIxcMQ8hsya5zRtRJxeiSFQ)** *[13.05.2023 15:36](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgyHZdNSJFr6Md8zCH14AaABAg)*

Интересно, можно ли оптимизировать транспиляцию наследования ES6 классов в babel, учитывая вышеизложенную информацию

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[14.05.2023 23:10](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgyHZdNSJFr6Md8zCH14AaABAg.9pe_FadJPSG9phy6fQHCFu) · 👍 1*

> Я бы мог бы ответить Вам предметно, если бы видел примеры кода. 
> Иными словами для меня слова - транспиляция наследования ES6 классов в babel звучит как абракадабра. 
> Тем не менее, с высокой долей вероятности могу сказать, что в условиях транспиляции, тем более babel там никто в серьез вообще не думал про производительность. Там в первую очередь думают про то, чтобы оно хоть как то работало.
> 
> Предметно можно сказать только тогда, когда Вы дадите пример кода.

> **[@ThomasA-i7o](https://www.youtube.com/channel/UCIxcMQ8hsya5zRtRJxeiSFQ)** *[15.05.2023 09:16](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgyHZdNSJFr6Md8zCH14AaABAg.9pe_FadJPSG9pj2MF3XTYT) (ред. 15.05.2023 09:16)*

> @AsForJS Условно вот такой код 
> 
> class A {
>     constructor(a) {
>         this.a = a;
>     }
> }
> 
> class B extends A{
>     constructor(a) {
>     	super(a);
>     } 
> }

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[16.05.2023 12:40](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgyHZdNSJFr6Md8zCH14AaABAg.9pe_FadJPSG9plz_cHcW88) · 👍 1*

> В том что Вы написали как пример, нет ничего чтобы касалось идентификаторов. То есть наследование в JS конструкции для классов, является ничем иным как типичным прототипным наследованием, которое лежит в фундаменте JS.
> 
> Иными словами, я пока не могу уловить суть вопроса. Напишите мне в телеграмм, если Вам не жалко времени, для того, чтобы пояснить мне-тугодуму суть вопроса.

---

**[@ixplo](https://www.youtube.com/channel/UCi1w3WhkVWha0BAIBEXL-bA)** *[15.05.2023 19:29](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=Ugx4hUOS63Y1ocYbImt4AaABAg) (ред. 15.05.2023 19:45) · 👍 1*

этот тот нечастый случай, когда ваш подход не только оптимизирует время выполнения, но и очень желателен для уменьшения связанности кода. А это один из основных принципов того, как не скатиться в легаси ) глобальные переменные - зло )) лайк

---

**[@JoSmith0](https://www.youtube.com/channel/UCOkbwa2lb6-Tt_wPF4BbNcQ)** *[16.05.2023 19:45](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgwHe79X1ZS5ew55tod4AaABAg) · 👍 3*

А есть ли разница в производительности при различных вариантах передачи параметров в функцию? Например: doSomeThing({ a: 1, b: 2}) или doSomeThing(1, 2) ? По ощущению при передаче по второму варианту должны создаться переменные const в контексте вызываемой функции, что приведет к дополнительным простыням байт-кода?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[17.05.2023 16:42](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgwHe79X1ZS5ew55tod4AaABAg.9pmk9b5u_1T9pozzSk5jpU) (ред. 17.05.2023 16:43) · 👍 11*

> Это прекрасный вопрос от человека, который стал(или и смотрел) смотреть в самый корень того, как работает язык. Я хотел бы пожать Вам руку.
> 
> Каждый раз, когда мы используем ту или иную синтаксисечкую конструкцию в языке JS, мы себя должны спрашивать - а чего это стоит. Что реально происходит под капотом? 
> 
> И что сложнее всего, это положить поверх вопросы - а как это умеет оптимизировать мой RunTime? 
> 
> Что является причиной фразы, которую я всегда повторяю - JS очень прост для начинающего и чрезвычайно сложен для профессионала.   Иными словами, начинающий даже бы не задумался по этому вопросу и жил бы счастливо, получив работающий код, а профессионал вынужден был бы потратить много времени чтобы выбрать наиболее оптимальный для его условий код.
> 
> Конкретнее по Вашему вопросу.
> Все будет сильно зависеть что именно передается в функцию. Потому, что есть большая разница между тем, чтобы передать в нее: 
> doThing (1); 
> и передать в нее же 
> doThing(1.0);
> 
> Если в первом случае, в рамках V8, ваша 1 будет частью внутреннего указателя, благодаря оптимизациями V8 которые используют свободную его часть для хранения целых чисесл, которые могут быть описанны при помощи 31 бита со знаком. То во втором случае, то есть передачи 1.0 это будет создание полноценного обьекта в куче, описывающего число с плавающей точкой.
> 
> При этом следует помнить, что формально, передача любого примитивного значения, будь то 1 или строка, приведет к созданию внутри RunTime структуры которая должна его описать. То есть в реальности, только благодоря оптимизациями конретного RunTime, передавая в функцию число 1, вы туда передадите именно единицу на уровне машшиного кода. Во всех прочих случаях, любое подобное значение будет являться ссылкой на структуру в рамках HEAP описывающей ее. 
> 
> Что это значит в рамках Вашего примера. Это занчит, что между передачей в doThing одного обьекта doThing( {a: 1, b:2} ) и двух параметров doThing( 1, 2); есть минимум одна промежуточная фаза, когда в первом случае RunTime будет вынужден создать промежуточный обьект {a: 1, b:2}; внутри которого он создаст два проперти со ссылками на другие обьекты описывающие 1 и 2. 
> 
> И тут казалось бы ответ очевиден - раз есть лишняя операция по созданию лишнего обьекта, то передача простых проперти всегда быстрее. И это почти всегда так. ПОЧТИ.
> 
> Вопрос всегда в том, что потом происходит с этими данными из этих проперти, и что и как умеет делать RunTime с таким промежуточным обьектом.
>  
>  
> *Вместо ИГОГО*
> Вы абсолютно правы в той части, когда думаете, что чем меньше мы используем синтаксических конструкций языка, тем это влечет за собой меньшие расходы.
> 
> Но, в рамках развитости современных оптимизирующих компиляторов, нередки случаи, когда использование избыточной конструкции на старте, приведет к более высокой производительности в процессе - тогда, когда этот код будет оптимизирован оптимизирующим компилятором. 
> 
> И это именно то, что делает программиста JS профессионалом. Когда он либо знает с самого начала что будет, либо умеет себе проверить.

> **[@JoSmith0](https://www.youtube.com/channel/UCOkbwa2lb6-Tt_wPF4BbNcQ)** *[17.05.2023 17:26](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgwHe79X1ZS5ew55tod4AaABAg.9pmk9b5u_1T9pp41DWd9f9) · 👍 1*

> @AsForJS Благодарю за развернутый ответ!

---

**[@anishchenko](https://www.youtube.com/channel/UCB-qep9CiL7iZljv_fdNW8A)** *[17.05.2023 19:17](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=Ugws_vVsKGZXXw1OJaB4AaABAg) · 👍 5*

Спасибо!! реально не встречал больше такого  глубокого понимания на ютубе

---

**[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[03.06.2023 09:08](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=Ugz5LeN-FAlXZSIzEvl4AaABAg) · 👍 4*

Головастые люди байткод разработали. И Мурыч - толково разбирается! Это ж надо - так глубоко копать.

---

**[@BorderInVais](https://www.youtube.com/channel/UC1qmXy2vQ-hICupQzU6Jgpw)** *[18.09.2023 06:21](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgxkOba5NXTRrtB03jF4AaABAg) · 👍 3*

00:00:00   Музыка
00:02:00   Вступление
00:02:10   Производительность идентификаторов в коде
00:12:10   Игого

---

**[@island1345](https://www.youtube.com/channel/UCS2aZI1ZW4j9keu0pnlbB6w)** *[04.11.2023 12:15](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgxPHUt-ENIGWeKbusp4AaABAg) · 👍 3*

круто ) як на мене то краще робить короткі відео як це, так набагато краще сприймається матеріал

---

**[@johngalt9494](https://www.youtube.com/channel/UCULcuPJ1SALjUpSli2PMNyA)** *[16.12.2023 14:31](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgwbXIvyWDb2yE36ovJ4AaABAg) · 👍 3*

Коммент в поддержку канала !

---

**[@АлександрТкачук-р4в](https://www.youtube.com/channel/UC3KNIVO-wNhgW-7UoLmUfig)** *[21.12.2023 17:09](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgzBC7c1aCzbRuffCh94AaABAg) · 👍 1*

Всегда приятно смотреть на специалиста, спасибо за твой труд.

---

**[@raff_m_d6971](https://www.youtube.com/channel/UCdsqd4Phl6ebcHNL1p1B5eg)** *[24.12.2023 09:35](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgybENuBFacC8sDFzCF4AaABAg) · 👍 1*

Выражаю безграничную благодарность автору за контент

---

**[@simonpolyakov8304](https://www.youtube.com/channel/UC8VswwaBN8zed1xLBbwIEQQ)** *[23.01.2024 05:35](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgyhlTKhn6-lVTw6D0N4AaABAg) · 👍 2*

Чем отличается в байт коде операция CreateFunctionContext от CreateClosure?

---

**[@khmerhan2748](https://www.youtube.com/channel/UCQY3nUwcprTrW9ny_D2RHHw)** *[13.03.2024 21:44](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=Ugy0H5kBSNLmbeyt_ah4AaABAg)*

благодарю, очень доходчиво

---

**[@raff_m_d6971](https://www.youtube.com/channel/UCdsqd4Phl6ebcHNL1p1B5eg)** *[02.04.2024 05:58](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=UgyTpSyMJhu-yzyPIHV4AaABAg)*

Выражаю благодарность автору за контент

---

**[@mcltdtm420](https://www.youtube.com/channel/UCu4YeW9ZlE51GwOEbpAox3w)** *[03.07.2025 17:01](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=Ugzv3oNyPD4bczw5K-B4AaABAg)*

а якщо замість зовнішньої змінної використати об'єкт з ключем, який буде використаний як змінна ?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[07.07.2025 01:12](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=Ugzv3oNyPD4bczw5K-B4AaABAg.AK7JhYZrG3KAKFvFoKDj2d)*

> Процесс оптимизации измениться. При этом серьезных плюсов или минусов сразу на вскидку не вспомню.
> 
> Кроме одного замечания - локальные "переменные" в V8, то есть те которые обьявлены внутри функции и существуют только для нее - оптимизируется чрезвычайно эффективно. Намного лучше любой другой формы.

> **[@mcltdtm420](https://www.youtube.com/channel/UCu4YeW9ZlE51GwOEbpAox3w)** *[07.07.2025 07:40](https://www.youtube.com/watch?v=biy50-ssgVQ&lc=Ugzv3oNyPD4bczw5K-B4AaABAg.AK7JhYZrG3KAKGbeGw7IVQ)*

> дякую ​@AsForJS

---
