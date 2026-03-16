---
title: "⎡msk⎦ JavaScript JSON как эффективный прием оптимизации холодного старта JS кода."
date: 2023-05-17
tags: []
videoId: "P3KQkLUvFFw"
duration: "24:55"
views: 1874
likes: 149
comments: 22
---
# [⎡msk⎦ JavaScript JSON как эффективный прием оптимизации холодного старта JS кода.](https://www.youtube.com/watch?v=P3KQkLUvFFw)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 17.05.2023 01:56  
**Тривалість:** 24:55  
**Перегляди:** 1874 · **Лайки:** 149 · **Коментарі:** 22
![thumbnail](https://i.ytimg.com/vi/P3KQkLUvFFw/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=P3KQkLUvFFw)
## Коментарі (14 · відповідей: 8)

**[@chikenmacnugget](https://www.youtube.com/channel/UCyWOOKPeKYrjDQcZqz0Gyiw)** *[16.05.2023 14:12](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=UgzsTX5uaYkmRAwJt8N4AaABAg)*

10кб это достаточно много кода должно быть

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[17.05.2023 16:02](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=UgzsTX5uaYkmRAwJt8N4AaABAg.9pm919x7ohE9povWboAWKW)*

> 10Кб это не только про код. Это про то, что может лежать внутри вашего обьекта. 
> Например у Вас есть текст, который связан с одним их Property. И обьем этого текста, в рамках UTF16 уже совсем выглядит не таким уж и большим.
> 
> Более того, то авторы V8, как люди которых критикуют все и вся, перестраховываются таким образом, что уже подкопаться нельзя никак. А такие люди как я, говорят - да любые данные, которые Вы можете описать JSON нотацией, должны быть так описаны.

> **[@chikenmacnugget](https://www.youtube.com/channel/UCyWOOKPeKYrjDQcZqz0Gyiw)** *[17.05.2023 23:41](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=UgzsTX5uaYkmRAwJt8N4AaABAg.9pm919x7ohE9ppjxYRPIXJ) (ред. 14.06.2024 00:56)*

> @AsForJS пон

---

**[@FedorBasmanof](https://www.youtube.com/channel/UC9wiSAQWG5Wml_bBomXMJYw)** *[16.05.2023 16:49](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=UgwPXqDFAgJuLQoHakJ4AaABAg) (ред. 16.05.2023 16:51)*

Cпасибо за видео! Если автор мне ответит, скушаю сырое яйцо. Если есть возможность, можно ли сделать чтобы вебка была не как слайдшоу))) Очень хочется наблюдать за живой реакцией и дикцией, но даже так круто, спасибо!

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[17.05.2023 16:05](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=UgwPXqDFAgJuLQoHakJ4AaABAg.9pmR5jGTg6o9povp-iXf1G)*

> Тут есть две проблемы. У меня нет вменяемой камеры чтобы ее использовать. И нет сейчас никаких средств чтобы ее купить. Поскольку благодаря действиям РФ освободителей, я уже дважды в своей жизни потерял все. 
> Впрочем, на микро-очке в углу экрана, может сгодиться и любое подделие. Я обязательно сделаю эксперимент.

---

**[@yurichihray8421](https://www.youtube.com/channel/UCpURvm0Sw7j24LiHOQ8pKyg)** *[17.05.2023 12:01](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=UgyCcWVh_2U73qyLuA54AaABAg)*

Цікаво, а я ж тоді бути з умовним react і setState в ньому?
Щоб він зрозумів, що щось змінилось, потрібно якраз створити нове звʼязування... Як в такому випадку "оптимізовано" копіювати/створювати обʼєкти?
Дякую

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[17.05.2023 17:27](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=UgyCcWVh_2U73qyLuA54AaABAg.9poUqmtt0569pp48lN8ojs) · 👍 2*

> По перше, щиро дякую що спілкуєтесь зі мною солов'їною.
> По друге, я не розуміюся на React, тобто я й гадки не маю про що ви питаєте. Та щоб порозумітися, що найкраще, було б надати приклад коду. 
> 
> Зроблю припущення, що ви запитуєте про те, яким чином у випадку, коли є умовний об'єкт який описує собою поточний вигляд чогось, відбувається вирішення питання, коли якесь проперти цього об'єкту буде змінено.
> 
> Це питання, є фундаментальним настільки, що саме для нього влаштовують особливі конференції. 
> 
> В JS це вирішується з одного боку дуже елегантно, а з іншого с купою проблем. 
> Вирішується це завдяки саме тому Prototype  наслідуванню. Наприклад:
> У Вас є об'єкт: {
>     name: "",
>     age: 0
> }
> 
> Надалі цей обь'єкт змінюється:
> {
>     name: "murych",
>     age: 0
> }
> 
> та змінюється ще раз:
> {
>     name: "murych",
>     age: 46
> }
> 
> Цей ланцюжок об`єктів можливо було б описаті так
> var theObj  = {
>     name: "",
>     age: 0
> };
> 
> Далі:
> theObj = Object.setPrototypeOf( {name: "murych"}, theObj);
> 
> Далі:
> theObj = Object.setPrototypeOf( {age: 46}, theObj);
> 
> У підсумку, мі маємо ланцюжок прототипів, які у поточному часі дадуть нам поточний стан об'єкту:
> theObj.name;
> theObj.age;
> 
> А якщо ми пройдемо по ланцюжку прототипів то ми отримаємо історію змін.
> 
> І це було б найкраще рішення, якщо б не обставини щодо того, як оптимізується код JS. 
> 
> Для оптимізуючого компілятора, theObj на кожному кроці  Object.setPrototypeOf буде зовсім іншим об'єктом а ніж до того. Тобто, увесь код, який був оптимізовано до моменту коли з'явилося нове Object.setPrototypeOf  буде позначено як код для деоптимізації. 
> 
> Тобто з одного боку, ми маємо дуже протий та ефективний механізм відстежування State для змін нашого Object. А  з іншого боку, це призводить до того, що сучасні алгоритмі оптимізації коду, не можуть такий код оптимізувати. Точніше можуть, але лише тоді, кодли цей код ніяк не змінюється.
> 
> Це призводить до того, що спробують робити теж саме Prototype наслідування, але не методами JS, а емулючи їх таким чином, щом, ланцуг прототипів не змінювався.
> 
> Це дуже цікава тема, особливо в площині того, що таке FP та що таке OOP.

---

**[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[03.06.2023 14:44](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=Ugx1agjVmPU1snkcLex4AaABAg) · 👍 1*

Писал я графический редактор, где нужно было копирование объектов на канвасе. Под капотом каждого графического объекта у меня был ЖС объект. Некоторые векторные объекты были сгруппированы из более простых объектов. Был функционал сгруппировать/разгруппировать.

И копирование групп объектов, выделил квадратом несколько объектов и надо их склонировать кнопкой на панели инструментов, или через контекстное меню.

Админку писал, где были датагриды с айтемами и был способ создания айтема путем копирования существующего айтема, с его дальнейшим редактированием и сохранением в БД.

Айтемы эти были сложными(некоторые из них), это были объекты с вложенными объектами. В некоторых случаях до 4 уровней вложенности было.

Задачи, где нужно клонировать объекты глубоко - бывают.

> **[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[03.06.2023 14:48](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=Ugx1agjVmPU1snkcLex4AaABAg.9qVZ5OyVmb69qVZVHWxqQQ) · 👍 1*

> Возможно, неграмотно организованы данные были, что такая вложенность. Но, тем не менее...

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[04.06.2023 22:36](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=Ugx1agjVmPU1snkcLex4AaABAg.9qVZ5OyVmb69qYyp-VbtcP)*

> Чтобы отметить предметно, нужно мне точнее понять суть разрешаемой задачи.
> Как бы то нибыло, я настаиваю на том, что говорил раньше - если Вам требуется копирование обьектов, то у Вас проблема с архитектурой приложения. 
> 
> Это очевидно предположение идет из того посыла, что коль у Вас есть данные, которые повторяются из раза в раз, то значит именно они должны и быть источником построения обьекта. Это и есть прототипы. Прототипное наследование. Когда вы поверх одного прототипа накладываете другой. Как следствие одинаковые данные остаются определенными единожды.

---

**[@gordoner5693](https://www.youtube.com/channel/UCmBrBHi1DKugtCFYAIcgeFg)** *[13.06.2023 15:34](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=UgyyUmEFIOEqlgyCAzN4AaABAg) (ред. 13.06.2023 16:16)*

Почему var пишите? И появился еще один вопрос: чтобы оптимизировать наш код, нужно создавать объекты с помощью Json.parse нежели с литералом объекта?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[26.06.2023 12:55](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=UgyyUmEFIOEqlgyCAzN4AaABAg.9quOjiKAR4V9rQ_pARWGRU) · 👍 1*

> Потому, что var это неотьемлемая часть языка JavaScript. 
> Потому, что var универсален и не влечет за собой дополнительных издержек с точки зрения потребляемых ресурсов.
> Потому, что я глупый, и мне намного проще контролировать окружение для  var, чем контролировать все пограничные условия для let и const не соблюдение которых прямо приводит к излишним накладным расходам.
> 
> Мне так проще.
> 
> Про JSON
> речь идет о том, что если у Вас есть какие-либо структуры данных на входе работы вашего проекта, обьемами от 10 килобайт текста, то выгоднее их создавать именно путем JSON.parse из JSON string, что подверждают сами инженеры V8.

---

**[@Eternal_Rise](https://www.youtube.com/channel/UCaiIxi4Bpc_6_EBye_HCjFg)** *[15.07.2023 09:58](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=Ugy3fkjIm5o-siS5D-d4AaABAg)*

Єдине, я не зовсім зрозумів за використання JSON.parse. Ми одразу визначаємо наші дані, використовуючи JSON.parse, чи визначаємо їх як рядок, а потім, в місці використання, виконуємо JSON.parse?

const config = JSON.parse(...)

vs

const config = "...."
const doThing = () => {
  const { timeout } = JSON.parse(config)
 ...
}

---

**[@gyglejid](https://www.youtube.com/channel/UCy-LzPS8rpgK9PptmHNEVvg)** *[09.12.2023 12:58](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=Ugw2_4fImr31Bbk3NHZ4AaABAg) · 👍 1*

Этот комментарий создан в знак уважения к автору, его трудам и для продвижения его канала.

> **[@fractalminding](https://www.youtube.com/channel/UC1PF4egUFAH2yY0uLo5dyxw)** *[09.01.2024 23:22](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=Ugw2_4fImr31Bbk3NHZ4AaABAg.9y61B4Y99Vg9zMyDM0HPTp)*

> Как-то бездушно. Можно ведь было написать "Спасибо за классное видео. Желаю дальнейшего развития. Очень вас уважаю".

---

**[@johngalt9494](https://www.youtube.com/channel/UCULcuPJ1SALjUpSli2PMNyA)** *[16.12.2023 21:05](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=Ugwv5bffjPb8YLZjMJt4AaABAg) · 👍 3*

Коммент в поддержку канала !

---

**[@diniszabrodsky8508](https://www.youtube.com/channel/UCkO7hEGdqVb-PPRUbU3pdJg)** *[27.12.2023 21:27](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=UgxHhFUVyNtC5yVKh954AaABAg)*

ось як мені відовіли на інформацю з відео "але блін, ми ж після парсінгу отримуємо той самий об'єкт, і зберігаємо тепер і стрічку і об'єкт". Можете, будь-ласка, дати розяснення?)

---

**[@rodigy](https://www.youtube.com/channel/UCDbVwcOGci1hdYziHyPYXzQ)** *[02.01.2024 19:08](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=Ugwz9uMa4rBOQmK4G4Z4AaABAg) · 👍 1*

В этом видео не хватало демонстрации внутренней структуры объекта созданного при помощи литерала.

---

**[@crypto-pro26](https://www.youtube.com/channel/UC-zJUlXMA-VsoowC1Z_9MpA)** *[19.01.2024 15:41](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=UgwWECiCkTySXukClYh4AaABAg)*

Да интересный кейс. Спасибо за видео

---

**[@khmerhan2748](https://www.youtube.com/channel/UCQY3nUwcprTrW9ny_D2RHHw)** *[14.03.2024 01:19](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=UgyQXOgK_7fThmROrPZ4AaABAg)*

любопытно

---

**[@raff_m_d6971](https://www.youtube.com/channel/UCdsqd4Phl6ebcHNL1p1B5eg)** *[02.04.2024 05:57](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=Ugx7R8CGYkoMHHfY3CF4AaABAg)*

Выражаю благодарность автору за контент

---

**[@SashaKuzikov](https://www.youtube.com/channel/UC8MPhuwYWm5qKyvzkODtJpw)** *[21.06.2025 11:57](https://www.youtube.com/watch?v=P3KQkLUvFFw&lc=UgwPwD2twBWSmnOeyot4AaABAg)*

В принципе, все логично - строгие правила обрабатываются быстрее.

---
