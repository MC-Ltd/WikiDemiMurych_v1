---
title: "Как работает this в javascript.  Разберемся на примерах. [Короткая версия]  [RU]"
date: 2023-05-07
tags: []
videoId: "fQ7_GT8_zeM"
duration: "27:46"
views: 10059
likes: 624
comments: 26
---
# [Как работает this в javascript.  Разберемся на примерах. [Короткая версия]  [RU]](https://www.youtube.com/watch?v=fQ7_GT8_zeM)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 07.05.2023 21:06  
**Тривалість:** 27:46  
**Перегляди:** 10059 · **Лайки:** 624 · **Коментарі:** 26
![thumbnail](https://i.ytimg.com/vi/fQ7_GT8_zeM/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=fQ7_GT8_zeM)
## Коментарі (18 · відповідей: 8)

**[@alexup7437](https://www.youtube.com/channel/UCaVJoJKeWCWonbRtn6NVQYg)** *[07.05.2023 12:23](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=Ugyh2aIVh7BL4KoDWE14AaABAg) (ред. 07.05.2023 12:24) · 👍 2*

А разве вызов функции  без дот нотации, не является дот нотацией window/globalObj.doLogThis()?

> **[@Fodintsov](https://www.youtube.com/channel/UCvIUqC8hxvctYDNWG-GeC5A)** *[07.05.2023 19:43](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=Ugyh2aIVh7BL4KoDWE14AaABAg.9pPmVHtg5rm9pQZo9h_Jq9) · 👍 1*

> Получается, что нет. Если хочется проверить в консоли браузера, нужно не забыть включить стрикт режим.

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[08.05.2023 01:48](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=Ugyh2aIVh7BL4KoDWE14AaABAg.9pPmVHtg5rm9pRDZR_THyr) (ред. 08.05.2023 01:51) · 👍 17*

> Очень правильный вопрос.
> Как Вам правильно написали выше, появления строгого режима (strict mode), привело к тому, что this связывается по умолчанию со значением undefined во всех неявных ситуациях. 
> Неявной ситуацией я называю вызов кода (это мой термин - не термин спецификации), когда мы по внешнему виду вызова кода (синтаксис) не можем точно сказать к чему это приведет для this.
> 
> И вот тут и происходит лексическая вилка:
> В спецификации от 1997 года (самая первая спецификация по JS) сказано что this это имутабельное значение которое по умолчанию связано с глобальным обьектом. Что очень логично, особенно если мы вспомним, что this это сущность которая по своему поведению похожа на типичный идентификатор. То есть, если в глобальном окружении this связан с глобальным обьектом, а сам this по своему поведению схож с идентификатором - то очеивдно, что если при запуске функции, нет явного определения this то он по цепочке окружений придет к global environment где this = global object.
> 
> Так в чем проблема? Почему в строгом режиме это поведение было изменено - ведь вроде бы все логично? Проблемы начались тогда, когда язык JavaScript из скриптового языка для обработки сценариев в браузере, стал скриптовым языком универсального назначения. То есть внедрять JS стало возможным куда угодно.  И тут произошел казус - когда в спецификации допустили, что при инициации кода из Global Environment, HOST система может установить this как ей хочется, а если ей никак не хочется - то тогда по умолчанию GLobal Environment. 
> 
> То есть мы попали в ситуацию, когда this теперь не имеет однозначного определения на стадии выполнения кода в Global Environment, так как это было в 1997 году. Появление strict mode обусловлено в том числе и попыткой решить накопившиеся проблемы подобного характера.  В результате приняли решение (на мой взгляд ОЧЕНЬ плохое), что в случае strict mode при формировании окружения ( а это любой вызов кода функции, и (еще одно ужасное решение)  при формировании блока {} ) устанавливать значение this идентификатора в значение undefined. Типа мы не в кугсе как оно там.
> 
> 
> *Вместо ИГОГО*
> На мой взгляд, было бы крайне логичным, не трогать this с его поведением от 1997 года. И решая проблемы встраиваемости в другие окружения, сразу предложить что-то подобие module - что и произошло потом в любом случае. Тем не менее, тогда такое решение показалось радикальным, и вместо этого сначала дали возможность HOST среде менять this как ей хочется, а только потом поняли как поломали логику. Потом ввели strict mode для того чтобы как-то все привести в порядок. А потом все равно сделали новое глобальное окружение module.
> 
> Вот за такие мансы, и можно называть JS - Weird языком. Но только именно потому, что в отличии от прочих языков, в JS такой архитектурный апокалипсис возможен, этот язык никогда не умрет. Будет оставаться мутантом и мимикрировать под происходящее вокруг, но будет жить.

> **[@__kawaii](https://www.youtube.com/channel/UC8D8tafBpWM7Vb4bU_MtYXw)** *[22.12.2023 13:09](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=Ugyh2aIVh7BL4KoDWE14AaABAg.9pPmVHtg5rm9ycWjcIT_pF) (ред. 13.06.2024 21:12) · 👍 6*

> @demimurych1Вот за такие комментарии я тебя и уважаю

---

**[@JoSmith0](https://www.youtube.com/channel/UCOkbwa2lb6-Tt_wPF4BbNcQ)** *[07.05.2023 14:23](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgzHQc8jrX8Q7d4AH9B4AaABAg) · 👍 25*

Обьяснение уровня Бог! Все так просто, респект тебе!

---

**[@alexandroppolus](https://www.youtube.com/channel/UCMuGh1mA8uzJeO-LLN8KdRw)** *[22.10.2023 22:52](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgyWlr0ttVH01gMrWMh4AaABAg) · 👍 1*

Не совсем правильно на 7:50 
new более приоритетно, чем bind, и ромбики лучше поменять местами

function fff() {
    console.log('this = ', this);
}
const bound = fff.bind([1]);
new bound(); // в V8 точно не [1]

---

**[@romankrytski8687](https://www.youtube.com/channel/UCNpBjjg-z3S_S-VcqwbpZyg)** *[07.12.2023 08:30](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgyezS9n6KiJj3vXioZ4AaABAg) (ред. 07.12.2023 08:33) · 👍 6*

Ты крутой дядька! Спасибо за короткую версию, очень хорошая компоновка материала, разжёванного в длинном видео. 

Очень пригодится, если, вдруг, понадобится напоминалка.

Дай знать, если тебе можно чем-нибудь помочь =3

> **[@ArtsiomMalyshev](https://www.youtube.com/channel/UCDU4WCYqc0y6HybGRZwy88g)** *[20.05.2024 23:25](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgyezS9n6KiJj3vXioZ4AaABAg.9y0OsK-VLNVA3frY2zXaWR) · 👍 1*

> Донатом на помощь ВСУ)

---

**[@toscaantosca4541](https://www.youtube.com/channel/UCiEbdIZsuGkgz9r0MiwIyVA)** *[16.12.2023 09:08](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgzAltvaG6LXS8H7M_54AaABAg) · 👍 4*

спасибо за видео! терпения и здоровья!

---

**[@СергейК-б6н](https://www.youtube.com/channel/UCpQBlI46nCKFTjVFpCCPxeg)** *[11.01.2024 20:20](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgwDiA0K_A3wrHgX9rd4AaABAg) · 👍 3*

Этож мурыч

---

**[@russell198309](https://www.youtube.com/channel/UCpazuGXHI-W42jdnYNSvzow)** *[25.01.2024 21:10](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgwSsbtWE7dIGZWRtaV4AaABAg) (ред. 25.01.2024 21:34) · 👍 3*

Видео супер, но про стрелочные функции не сказано

---

**[@_Good_Evening_](https://www.youtube.com/channel/UC9HBo0_7o8jROXlvkFcVfIg)** *[01.02.2024 13:57](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=Ugz-LjWTgxHQLOuwBDh4AaABAg) · 👍 2*

Очень крутой ролик!!!

---

**[@locktar-o-dark5664](https://www.youtube.com/channel/UCRoTCnxC3cPjE6WH2BAD6VQ)** *[28.02.2024 06:48](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgwG8xKbSmrg2cC3JcV4AaABAg) · 👍 1*

Не смотрел ещё, плющит от полной версии, в которой полно желчи нашего персонажа. Ему бы поучиться повествовать как это делает Ulbi, цены бы не было.

---

**[@locktar-o-dark5664](https://www.youtube.com/channel/UCRoTCnxC3cPjE6WH2BAD6VQ)** *[29.02.2024 20:24](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgzIKbok_YD1Qze1l5t4AaABAg) (ред. 29.02.2024 21:26) · 👍 1*

Узнал новое слово "аппли". Теперь я мастер жоес.
Upd: а, нет на 22:54, таки это эплэй. Мэджик пипл, вуду пипл.

---

**[@povdata](https://www.youtube.com/channel/UCOkMxxyqNhoJOyp6aDZ_kFQ)** *[11.04.2024 09:18](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgwLKRqJpX092AgmNE14AaABAg)*

function showThis() {
  console.log(this);
}

showThis(); 

почему это дает window если это вызов нормальный функции в консоли хром?

> **[@bebrick04](https://www.youtube.com/channel/UCWNWhXQ2v1Wswj2p3AtqV3Q)** *[15.04.2024 21:00](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgwLKRqJpX092AgmNE14AaABAg.A24vavMUqyNA2GU11gDBRS)*

> Могу ошибиться так как сам изучаю месяц два джс, но если вкратце, есть глобальный объект языка Js (window), он отвечает за окно браузера. И представь его как самый простой объект который ты инициализируешь с помощью  литерала {}, вот как это выглядит 
> var window = {}, так вот когда ты создаешь функцию ты создаешь метод объекта Window, тоесть наш объект теперь выглядит как 
> window = {
> showThis: function() {
> console.log(this)
>   }
> }
> Так же например для понимания, не используя use strict, ты можешь написать в своем коде например глобальную переменную не используя var let const, ты можешь просто написать a = 1 и можешь вывести значение вот таким образом console.log(window.a) // 1.
> Надеюсь понятно, а если заблуждаюсь и тот кто это прочитал буду рад услышать замечания.

> **[@JeroenMarsh](https://www.youtube.com/channel/UC4cbLoGdVna43ViamgoP8eQ)** *[31.10.2024 08:42](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgwLKRqJpX092AgmNE14AaABAg.A24vavMUqyNAAFZmvLGCte)*

> используй use strict и тогда выдаст undefined

---

**[@MrAirrussia](https://www.youtube.com/channel/UCIZb_CSfb6ArclgCkv5rG8w)** *[30.06.2024 02:38](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgzrLH2bSdrY8JdMY-R4AaABAg)*

правильно, когда задают такой вопрос, "console.log( this )" в таком примере, на этом всё заканчивается, нет смысла дальше общаться, дальше будет прогрессировать биполярка у интервьюера.

---

**[@АндрейСветлов-п5о](https://www.youtube.com/channel/UCZFhb5Ic3LgnysyNv0082Ow)** *[13.07.2024 08:36](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgyGjoKnRfPdACqgv8N4AaABAg) · 👍 4*

Если честно лучшего объяснения я не видел нигде, благодарствую

> **[@sjdjjsjsjs3991](https://www.youtube.com/channel/UCXGfhoqdgreVsVKIfbiJGbQ)** *[27.09.2024 09:28](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgyGjoKnRfPdACqgv8N4AaABAg.A5pJecTHj8tA8t62Evr_Iz)*

> У Кайла Симпсона тоже хорошее объяснение, как работает this

---

**[@annaumi](https://www.youtube.com/channel/UCgufsKBniBiz-BKptfd71MQ)** *[01.08.2024 06:48](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=Ugz6IMcKVWcpiu1kaAN4AaABAg)*

This is the object that function is a property of

---

**[@МихаилБоярский-о5м](https://www.youtube.com/channel/UCyfXK2LYD9LxHIPFD7dSupA)** *[28.03.2025 10:05](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgxELJwM_nABYwJbsGJ4AaABAg) · 👍 2*

Спасибо за такое крутое и доскональное объяснение

---

**[@kenobi6027](https://www.youtube.com/channel/UCsaAFsiz5yGJsBQumumTkDA)** *[31.03.2025 20:21](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgyXBo8YpUCOuOHcMiZ4AaABAg) · 👍 2*

Круто Мурыч! Спасибо

---

**[@konstantintanat4462](https://www.youtube.com/channel/UCst48J2iEcaB72k4OhLHxbg)** *[20.04.2025 17:37](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgxIsn6Iqn3RdOnekYx4AaABAg) (ред. 20.04.2025 17:48) · 👍 2*

если бы в яваскрипте было бы все логично и просто то не требывалось бы лезть периодичски в спецификацию чтобы понять что за фигня происходит

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[20.04.2025 17:45](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=UgxIsn6Iqn3RdOnekYx4AaABAg.AH8q-F-9zIEAH8qrqey7od)*

> Єто безусловно. 
> Только в других языках, история развития которых больше 5 лет, все точно так-же.
> 
> Разница в том, что кроме спецификации, есть официальный второй/третий/n-ый  документ поясняющий почему так.

---

**[@rublevalina](https://www.youtube.com/channel/UCI65Pam9wrBEAsfhx-GtUIA)** *[14.12.2025 09:43](https://www.youtube.com/watch?v=fQ7_GT8_zeM&lc=Ugyfu-6lZ45Nn6SLbyN4AaABAg)*

шикарное объяснение темы! благодарю за вашу работу ❤

---
