---
title: "Как одни фантазируют на тему типов в JavaScript ,  а другие с удовольствием верят в эти фантазии."
date: 2021-10-10
tags: []
videoId: "LyQzyrZRNXs"
duration: "3:06:37"
views: 17680
likes: 588
comments: 171
---
# [Как одни фантазируют на тему типов в JavaScript ,  а другие с удовольствием верят в эти фантазии.](https://www.youtube.com/watch?v=LyQzyrZRNXs)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 10.10.2021 09:24  
**Тривалість:** 3:06:37  
**Перегляди:** 17680 · **Лайки:** 588 · **Коментарі:** 171
![thumbnail](https://i.ytimg.com/vi/LyQzyrZRNXs/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=LyQzyrZRNXs)
## Коментарі (81 · відповідей: 90)

**[@DmytroShapovalovUA](https://www.youtube.com/channel/UC5L1MRBYsO1ocuEePNUEydw)** *[11.10.2021 18:13](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugz52tWeo64pwFhFlz54AaABAg) · 👍 1*

Спасибо, очень интересно! А как с числами? Читал, что под строки память в куче выделяется, а числа, мол прям в стеке хранятся. Я запомнил это, но пока что не понял в чём прикол.

> **[@demimurych2008](https://www.youtube.com/channel/UCq1SafSfdHwQEfQ5tMCsTCg)** *[01.11.2021 22:13](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugz52tWeo64pwFhFlz54AaABAg.9TMz-pY70up9UDUC0ostZh) · 👍 13*

> с числами все ровно точно также, с одним акцентом: если число помещается в размер текущей архитектуры, и при этом вы используете это число в рамках текущей области видимости, то число постараются разместить в регистре процессора. 
> Например, вы используете целое число в пределах 64 бит, то оно будет с высокой долей вероятности размещено в регистре, как на уровне байт кода, так и на уровне машинного кода. 
> При этом важно помнить, что  если архитектура вашей машины 32 битная, а число не помещается в 32 бита ( больше 4млрд) то все будер ровно также как и со строками. 
> аналогичная ситуация и с дробями (числами с плавающей запятой)
> 
> *Вообще важно помнить следующее*
> практически все, за редким исключением, оптимизации делаются на уровне одной функции. из чего следует, что если вы внутри функции используете любое значение из внешней области видимости, то тем самым сильно можете ограничивать работу оптимизатора. 
> 
> я запишу пару практических примеров, чтобы было нагляднее

> **[@leilaoskanova7557](https://www.youtube.com/channel/UCewBC1BiwQ901Iol8b1aWOg)** *[02.12.2023 11:25](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugz52tWeo64pwFhFlz54AaABAg.9TMz-pY70up9xoq-edAnqD)*

> Спасибо за информацию.
> Подскажите, что будет оптимальней работать.
> Есть функция, которая вызывается тысячи раз в ходе работы приложения и которая всегда должна возвращать один и тот же объект
> Что оптимальней, вынести объект за пределы функции, чтобы он не создавался заново каждый раз, когда мы вызываем функцию (но тогда эту функцию будет сложно оптимизировать из-за того что объект берется из внешнего блока?)
> Или создавать объект внутри функции (да, он будет тысячи раз пересоздаваться, но зато оптимизирующий компилятор сможет легче оптимизировать функцию)

---

**[@DmytroShapovalovUA](https://www.youtube.com/channel/UC5L1MRBYsO1ocuEePNUEydw)** *[11.10.2021 18:38](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzEqR7Y7y0PFyXlHZR4AaABAg) · 👍 3*

Насчет задачи про массивы на 2:40:32. Можно задать резервный массив как прототип первому. Правда на MDN пишут, что такое переопределение ведет к непредсказуемым потерям в производительности. Но думаю, что ожидаемое решение было именно таким, потому что оно демонстрирует, что даже индексы в массивах в ЖСе - надстройка над ключами объектов, насколько я понимаю.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[02.11.2021 00:43](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzEqR7Y7y0PFyXlHZR4AaABAg.9TN0v5BBTTc9UDkKGxoGu_) · 👍 4*

> Да, смысл задачи именно в том, чтобы напомнить что такое прототипное наследование, зачем оно создавалось, и чем являются Array в JS.
> 
> _> Правда на MDN пишут, что такое переопределение ведет к непредсказуемым потерям в производительности_
> Не просто предсказуемое, но и самое производительное в рамках V8. 
> Конечно в рамках Spider Monkey может быть совсем иначе. Только кого интересует SpiderMonkey с 5% рынка, то есть с долей в рамках статистической погрешности.
>   
> _>потому что оно демонстрирует, что даже индексы в массивах в ЖСе - надстройка над ключами объектов, насколько я понимаю_
> С одной стороны  -  к сожалению, 
> С другой стороны к счастью  - нет. 
> 
> В рамках V8 реализована особая машинерия для работы с целыми числовыми ключами, в рамках обьекта Array. Которая (ирония просто), работают в полтора раза медленнее чем единичный доступ по строковому ключу, но показывают себя с лучшей стороны в случае, когда происходит обработка Array обьекта, где все значения соответсвуют одному типу, и отсутствуют дырки.  
> То есть доступ вида
> myArr[0]  + myArr[1] 
> будет значительно медленее чем
> myObj.myPorperty1 + myObj.myProperty2
> 
> но  значительно быстрее в случае map reduce и т.д.

---

**[@Ruslan-x7i](https://www.youtube.com/channel/UCQNsY3gt4JdhnNhUXdIPFMw)** *[21.10.2021 19:39](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugy8XChM5J7tI-Ehwlt4AaABAg)*

Расскажите, пожалуйста, про решение задачи с arr1 и arr2 в одну строку?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[02.11.2021 00:34](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugy8XChM5J7tI-Ehwlt4AaABAg.9TlskfMoD0_9UDjKRIRB6K) · 👍 7*

> Любой способ назначить прототипом один Array другому. Например так:
> Reflect.setPrototypeOf(arr1, arr2)
> 
> или так
> Object.setPrototypeOf(arr1,arr2)

> **[@Ruslan-x7i](https://www.youtube.com/channel/UCQNsY3gt4JdhnNhUXdIPFMw)** *[02.11.2021 06:06](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugy8XChM5J7tI-Ehwlt4AaABAg.9TlskfMoD0_9UEKJpdywz6) · 👍 2*

> @AsForJS Спасибо! У Вас классный и очень нужный канал в наше время.

---

**[@bukanaka](https://www.youtube.com/channel/UClwPjU0S-_hiTbH1JsoS-rg)** *[15.11.2021 15:29](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxSAfB4b6YrflnOCPp4AaABAg) · 👍 1*

Пересматриваю второй раз для закрепления.

---

**[@bukanaka](https://www.youtube.com/channel/UClwPjU0S-_hiTbH1JsoS-rg)** *[15.11.2021 16:42](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwVzBmQJ6cJwKQx8zx4AaABAg) · 👍 18*

У Вас отличный канал. Люблю такие глубокие темы, особенно, в верном русле. Буду ждать ещё больше лекций!

---

**[@ilnurryazhapov](https://www.youtube.com/channel/UCtYFp3Wt6nZR33NNwvmNYpw)** *[15.11.2021 19:02](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzrMgPNuUHwjHStd7Z4AaABAg) · 👍 1*

Отличное видео, давайте еще))

---

**[@theone3120](https://www.youtube.com/channel/UCgoJS1sWzArVDbrYMn__2bw)** *[16.11.2021 18:32](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwftXJyUGcIRK8DofJ4AaABAg) · 👍 4*

Спасибо большое за очень интересный контент, очень жду еще. 

Но в защиту Тимура скажу, что в он знает и использует заморозку объектов. 
Почему он говорит такое в видео, я хз. Возможно много запары было и как-то понесло и напутал. Возможно он подразумевал, что либо другое.

> **[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[03.06.2023 15:06](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwftXJyUGcIRK8DofJ4AaABAg.9UohlXR-rP39qVaYfdfuMO) · 👍 1*

> Тимур вообще - толковый мужик.

---

**[@bukanaka](https://www.youtube.com/channel/UClwPjU0S-_hiTbH1JsoS-rg)** *[19.11.2021 21:01](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxLxriPj_6a_jmppHd4AaABAg) (ред. 22.11.2021 22:13) · 👍 31*

0:52 - начало
2:37 - вступление
5:00 -  про типы в JS ( как их понимают и какие они на самом деле )
9:35 - копируются ли "примитивные типы" по значению? Проверяем в редакторе и в инструментах разработчика Chrome
30:30 - открываем спецификацию JS и смотрим описание типов | разбираемся в типах
51:00 - что же такое этот ваш "Объект" в JS?
52:46 - что же такое "ссылка" в JS и как идентификаторы обращаются к данным и снова немного про объекты
01:07:30 - немного про let и const
01:13:30 - возвращаемся к сути "ссылки"
01:18:47 - немного истории про JavaScript
01:20:56 - возвращаемся к нашему коду
01:31:43 - есть ли в спецификации что-нибудь о передаче по "ссылке" и/или о ссылочном типе данных?
01:48:38 - как происходит присваивание
02:08:22 - есть ли возможность запретить изменять объект третьим лицам в JS?
02:18:10 - про методы для массивов и for/forEach
02:26:40 - ответы на комментарии

---

**[@GoshaakaScooby](https://www.youtube.com/channel/UCNBeKP-oexgAeR_kvcjv05g)** *[16.12.2021 10:35](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugw50jhvCZL3OTBlPKB4AaABAg)*

Большое спасибо за видео.

> **[@GoshaakaScooby](https://www.youtube.com/channel/UCNBeKP-oexgAeR_kvcjv05g)** *[16.12.2021 15:08](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugw50jhvCZL3OTBlPKB4AaABAg.9W062wVBZxd9W0aHGhc7Ge) · 👍 1*

> 41:20 вы говорите что 8081 это undefined, могли бы вы подсказать в каком файле исходника v8 это можно посмотреть.

---

**[@vissper1](https://www.youtube.com/channel/UC_eZvVjKvCnXJBJektZUESQ)** *[16.12.2021 22:46](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugzx3jl54CXxkFVFNJx4AaABAg) · 👍 1*

Все по фактам

---

**[@ToumaStage](https://www.youtube.com/channel/UCG-Zgk2XexdxWoEMRI_ooPg)** *[17.12.2021 20:53](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxnigtvp7cr5XK88Dl4AaABAg)*

Спасибо большое ! А вы случайно не проводите уроки / курсы ? Думаю после таких видео уроков к вам будет наплыв желающих учиться у вас

---

**[@alexup7437](https://www.youtube.com/channel/UCaVJoJKeWCWonbRtn6NVQYg)** *[18.12.2021 14:41](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyGplAr0e9nZFqol4h4AaABAg) (ред. 18.12.2021 14:42) · 👍 1*

А почему если я объект определяю через var, то  к нему я могу достучаться через window.obj , а если через const/let то нет?

> **[@bukanaka](https://www.youtube.com/channel/UClwPjU0S-_hiTbH1JsoS-rg)** *[27.12.2021 21:55](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyGplAr0e9nZFqol4h4AaABAg.9W5gq83aDDM9WTdfVHg9YJ)*

> Может Вы стучитесь до их объявления?

> **[@maksym7094](https://www.youtube.com/channel/UCVWtzv69C2a--CEozyxNhTA)** *[19.04.2022 00:53](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyGplAr0e9nZFqol4h4AaABAg.9W5gq83aDDM9_zLzlDNWLu) · 👍 1*

> На верхнем уровне скриптов и функций let, в отличии от var, не создаёт свойства на глобальном объекте. (MDN)

---

**[@alexup7437](https://www.youtube.com/channel/UCaVJoJKeWCWonbRtn6NVQYg)** *[18.12.2021 18:31](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwdfaI6sUASgpiznRl4AaABAg) · 👍 9*

Тип данных - булинг - это топ!

---

**[@klubkov](https://www.youtube.com/channel/UC8bWQNj-vH7kzUJAO05GaKg)** *[19.12.2021 08:25](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxlXshcrh-BY-TJ-Bx4AaABAg) · 👍 2*

И земля плоская)

---

**[@maddev8](https://www.youtube.com/channel/UCCRRd50MKiK4AjyAhylULbA)** *[23.12.2021 12:28](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx8aYBbus0cfI_vXSt4AaABAg) · 👍 2*

На счет заморозки, то вы не правы. В JS, нет глубокой заморозки, например:
var obj = {
  prop:{ }
};
Object.freeze(obj);
obj.prop.age=666 // объект изменится. Если свойство объекта является объектом, то его всегда можно изменить, это относится и к Object.seal
Ваш канал очень нравится, действительно уникальная информация, не забрасывайте 👍

> **[@kujojotaro3464](https://www.youtube.com/channel/UCv3mHAG3KErQY9wltyyVLCg)** *[11.08.2022 19:31](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx8aYBbus0cfI_vXSt4AaABAg.9WIKa0u8My99eatZlgPp-B)*

> Лол, рекурсивно заморозить проблема?

> **[@maddev8](https://www.youtube.com/channel/UCCRRd50MKiK4AjyAhylULbA)** *[11.08.2022 20:15](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx8aYBbus0cfI_vXSt4AaABAg.9WIKa0u8My99eaygGdTAQR)*

> @kujojotaro3464 покажи как :)

> **[@kujojotaro3464](https://www.youtube.com/channel/UCv3mHAG3KErQY9wltyyVLCg)** *[11.08.2022 20:21](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx8aYBbus0cfI_vXSt4AaABAg.9WIKa0u8My99eazMFNXhzH)*

> @maddev8 На 
> 
> const deepFreeze = obj => {
>   Object.keys(obj).forEach(prop => {
>     if (typeof obj[prop] === 'object' && !Object.isFrozen(obj[prop])) deepFreeze(obj[prop]);
>   });
>   return Object.freeze(obj);
> };

> **[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[03.06.2023 18:27](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx8aYBbus0cfI_vXSt4AaABAg.9WIKa0u8My99qVx_6TzetS) · 👍 1*

> ​@maddev8 Фор ином пройтись)

> **[@alexanderberman9629](https://www.youtube.com/channel/UC2FvReto32-IBhu3wtJkrIw)** *[14.12.2023 15:18](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx8aYBbus0cfI_vXSt4AaABAg.9WIKa0u8My99yJ9Cuh4QVg) (ред. 14.06.2024 00:32)*

> @maddev8 var deepFreeze = (obj) => {
>         Object.getOwnPropertyNames(obj).forEach(function (name) {
>             let prop = obj[name];
>             if (typeof prop === object && prop !== null)
>                 deepFreeze(prop);
>         });
>         return Object.freeze(obj);
>     };

---

**[@aleksandr2245](https://www.youtube.com/channel/UCk_nD0EDscNtiWPaJgRPPGw)** *[03.01.2022 20:17](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzX0Z9DyZIwM8gI4pV4AaABAg) (ред. 03.01.2022 20:24)*

2:25:20

я, к слову, попробовал сравнить время выполнения для for и reduce c помощью такого кода

const arr = [1, 4, 3, 5, 7, 10, 2, 9, 7, 8, 10, 666, 12485187424, 15, 98736];

let sum = 0;

console.time('reduce');
sum = arr.reduce((acc, curr) => acc + curr);
console.timeEnd('reduce');
console.log(sum);

sum = 0;

console.time('for');
for (let i = 0; i < arr.length; i++) {
    sum += arr[i];
}
console.timeEnd('for');
console.log(sum);

sum = 0;

по крайней мере в этом случае for на порядок быстрее

> **[@venom5583](https://www.youtube.com/channel/UCS-LcIabpqieVCv2yDkpxyA)** *[10.02.2022 07:39](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzX0Z9DyZIwM8gI4pV4AaABAg.9WkV1Xuzv5Q9YFzOzTrmxo)*

> Пробую сравнивать в бенчмарках и разница колеблется в пределах 5% в обе стороны. Непонятно почему в консоли for в 2 раза быстрее, может какие-то оптимизации не работают.

---

**[@ФедорГоловин-с8к](https://www.youtube.com/channel/UCHaHYOZuSv3CYq0Jhi9SORw)** *[20.01.2022 14:14](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwTHlb9kaNtNzp7dOB4AaABAg)*

До просмотра этого видео "передача по ссылке" для меня означало тоже что "передача ссылки на модифицируемый объект".
Век живи, век учись

---

**[@georgespringbach2062](https://www.youtube.com/channel/UCYV38rwJYNDA8dCsb3L4hNw)** *[05.02.2022 14:25](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwhjS65MuTvhWIG5r14AaABAg)*

Даёшь больше ассемблера!

---

**[@ДониёрАзизов-о8ц](https://www.youtube.com/channel/UCoKQvhcwlbmBtx_2Eg-VW6w)** *[18.02.2022 23:47](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxEwFrARRfd_GimJPR4AaABAg) · 👍 1*

Замечательное видео!

Пожалуйста продолжайте вести канал!

---

**[@timmur4672](https://www.youtube.com/channel/UC-ucgTuS69kJj44YTTQbVow)** *[19.02.2022 03:45](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzaTcjMTruwRDmcOm54AaABAg)*

Тимур - дурак упоротый, пламенный патриот Гулага и всех радостей социализма. Его лечить надо а не цитировать.

> **[@theban2517](https://www.youtube.com/channel/UCMumHzJR30nz1QxNeUU0DQg)** *[02.07.2022 13:41](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzaTcjMTruwRDmcOm54AaABAg.9YbjrnVaU_d9czGjkq1hn7)*

> "фашизм очень недооценен" (с) Тимур

---

**[@andranikhambardzumyan6264](https://www.youtube.com/channel/UCVMs-tP2Exp7kaxQxKk0nAw)** *[13.05.2022 02:18](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyYH5gcSJ7oqiJfY-F4AaABAg)*

Thanks

---

**[@ivank.2040](https://www.youtube.com/channel/UCJhIVVMdQjww5Xo6SZjON1g)** *[03.07.2022 18:33](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxhlkvUykbobHUX4bd4AaABAg)*

Охрененный контент! А то как-то раз глаза выкатались после фразы одного "лектора" , что "просто строки - это такая "сущность(!!!)", к которой можно применить оператор спред от массива"))))

---

**[@anishchenko](https://www.youtube.com/channel/UCB-qep9CiL7iZljv_fdNW8A)** *[07.07.2022 22:02](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxC6iCw4lkg2t4651h4AaABAg) · 👍 1*

Чувак! ты крутой!!! Очень полезно !!

---

**[@RedkeiGost](https://www.youtube.com/channel/UCIeHc_8j36pnj-_lqws_2Kw)** *[11.08.2022 20:08](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzE5kCEm6BnWelu7Tp4AaABAg) · 👍 2*

1:50 - 2:00 чтение невидимой спецификации. Даже когда Мурыч вроде бы рзобрался, что читает другую вкладку и вроде бы открыл перевод, то все-равно читает что-то другое.
Сделаль опыть - var my_var создет переменную в window, а let/const - нет.

> **[@AvigdorKatz](https://www.youtube.com/channel/UCk6X3w_IO90tJpulmBkPE9w)** *[08.12.2023 22:05](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzE5kCEm6BnWelu7Tp4AaABAg.9eaxqxTmWFc9y4QyZ_CqQ0) (ред. 08.12.2023 22:06) · 👍 1*

> var создает свойство в  object environment record а let и const создают свойства в declarative environment record. напрямую обратится к declarative environment record невозможно.
> 
> В своих конспектах по статьям другого автора подробно разбирающего внутренее устройство языка встретил такое утверждение, что var x = 10 создает именно "переменную" которая в результате приводит и к созданию идентификатора в глобальном объект, но x = 10 не создает "переменную" хоть и создает свойство глобального объекта. Главными отличиями "переменной" называется:
> 
>   1. хойстинг, то есть свойство объявленное через var существуют уже до самого его объявления со значением undefined
>     console.log(a) // undefined
>     var a = 10;
>     -----
>     console.log(a) // Uncaught ReferenceError: a is not defined
>     a = 10;
> 
>   2. Переменную нельзя удалить из глобального объекта
>     var a = 10;
>     delete window.a            // false
>     console.log(window.a) // 10
>     -----
>     a = 10;
>     delete window.a            // true
>     console.log(window.a) // Uncaught ReferenceError: a is not defined

> **[@RedkeiGost](https://www.youtube.com/channel/UCIeHc_8j36pnj-_lqws_2Kw)** *[09.12.2023 06:40](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzE5kCEm6BnWelu7Tp4AaABAg.9eaxqxTmWFc9y5LvwrNfKg) (ред. 13.06.2024 21:25)*

> @AvigdorKatz а что за статья, какого автора?

> **[@AvigdorKatz](https://www.youtube.com/channel/UCk6X3w_IO90tJpulmBkPE9w)** *[10.12.2023 18:22](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzE5kCEm6BnWelu7Tp4AaABAg.9eaxqxTmWFc9y9B4U1Of1X) (ред. 13.06.2024 21:25)*

> @RedkeiGost Мои комментарии вам тут уже удалили 5 раз.

> **[@AvigdorKatz](https://www.youtube.com/channel/UCk6X3w_IO90tJpulmBkPE9w)** *[10.12.2023 18:23](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzE5kCEm6BnWelu7Tp4AaABAg.9eaxqxTmWFc9y9BBtEwtfm) (ред. 13.06.2024 21:25)*

> @RedkeiGost Гуглите: dmitrysoshnikov Тонкости ECMA-262-3. Часть 2. Объект переменных.
> 
> И там параграф: О переменных

> **[@AvigdorKatz](https://www.youtube.com/channel/UCk6X3w_IO90tJpulmBkPE9w)** *[10.12.2023 18:39](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzE5kCEm6BnWelu7Tp4AaABAg.9eaxqxTmWFc9y9CwG9bO2T) (ред. 13.06.2024 21:25)*

> @RedkeiGost dmitrysoshnikov ECMA-262-5 in detail. Chapter 3.2. Lexical environments: ECMAScript implementation.
> 
> "There are two kinds of environment records in ES5 specification: declarative environment records and object environment records.
> 
> Declarative environment records are used to handle variables, functions, formal parameters, etc. appeared in function scopes (in this case this is very activation object which we know from ES3 series) and catch clauses."
> 
> "The consequence from this fact is that declarative environment records are not assumed to be exposed directly to the user-level, which means we cannot access these bindings as e.g. properties of the record."
> 
> Но это статья 2011 года, а предыдущая на которую указал вообще 2009. Я их читал в 2015-2016 годах.

> **[@RedkeiGost](https://www.youtube.com/channel/UCIeHc_8j36pnj-_lqws_2Kw)** *[10.12.2023 19:05](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzE5kCEm6BnWelu7Tp4AaABAg.9eaxqxTmWFc9y9FzZfV7-0) (ред. 13.06.2024 21:25)*

> @AvigdorKatz Спасибо за Сошникова, посмотрю. Прям вот указания названия-автора статьии 2009 года не видел. Видимо вы имели ввиду само содержание статьи и упоминание конспекта.

> **[@AvigdorKatz](https://www.youtube.com/channel/UCk6X3w_IO90tJpulmBkPE9w)** *[10.12.2023 19:22](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzE5kCEm6BnWelu7Tp4AaABAg.9eaxqxTmWFc9y9HxMlvM-C) (ред. 13.06.2024 21:25) · 👍 1*

> ​@RedkeiGost  та не я просто ссылки оставлял, в последний раз забрал http, разбил адрес пробелами вокруг точек и слешей и все равно комментарий пропал.

---

**[@СеменСавлук-ш9л](https://www.youtube.com/channel/UC64Dd9XRhWD4B0O-7aWS3CA)** *[12.08.2022 11:06](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwH-eRZSbJj9YMIJel4AaABAg) · 👍 1*

Автор когда будут новые видео? Очень понравился ваш подход.

---

**[@stepanmikhailiuk4571](https://www.youtube.com/channel/UCzfcsYNE13Hngw8s-lAAUNg)** *[28.10.2022 05:56](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxBD6Lws2ZiRs8QeQ14AaABAg)*

Жаль что при объяснении того что такое константа, а что такое идентификатор, объявленный с помощью const фигурирует фраза "как в других языказ" Хотелось бы увидеть пример, машинный код, подсветка очевидной разницы в свойствах. 
Спасибо!

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[01.05.2023 05:03](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxBD6Lws2ZiRs8QeQ14AaABAg.9hiHLqwqf479p9YNHOcjG_) · 👍 1*

> На одном из старых моих видео, про разницу в var let и const там как раз детально и для байт кода и для машинного кода это показано

> **[@stepanmikhailiuk4571](https://www.youtube.com/channel/UCzfcsYNE13Hngw8s-lAAUNg)** *[04.05.2023 07:04](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxBD6Lws2ZiRs8QeQ14AaABAg.9hiHLqwqf479pHUYlTOXdi)*

> @AsForJS Ознакомлюсь, спасибо!

---

**[@brains-UP1](https://www.youtube.com/channel/UCPSRs1WODXodiiY0KpUkW0w)** *[06.02.2023 03:33](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxXCC9rsVs18Wr9u154AaABAg)*

всем рекомендую, автор - профессионал своего дела

---

**[@Fodintsov](https://www.youtube.com/channel/UCvIUqC8hxvctYDNWG-GeC5A)** *[08.05.2023 01:45](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwxtD1VlWUBi_Ycc554AaABAg)*

1:26:00 Вот все, чего показано, говорит о том, что объекты и строки передаются по ссылке. Идентификатору параметра функции присваивается адрес передаваемого объекта/строки. При присваивании в теле функции он теряется и заменяется новым. Понятно, что при чтении разыменовывание автоматом происходит и адрес памяти, как в Си, никто не даст. Но по сути передача по ссылке. Да, в сишном понимании. А какое еще есть-то? )

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[08.05.2023 02:28](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwxtD1VlWUBi_Ycc554AaABAg.9pRDCRCd1I99pRIACB0mc0) · 👍 1*

> > При присваивании в теле функции он теряется и заменяется новым. 
> Нет. Он не теряется. Будет присвоен ровно тот же адрес обьекта описывающий строку или число что и раньше. 
> 
> Изменение может возникнуть только в одном случае - если на момент нового связывания, старый обьект, не имел никаких ссылок на себя, и при этом Garbage Collector -у потребовалось освободить дополнительный обьем памяти, что привело к уничтожению обьекта который когда то ранее где-то использовался.

> **[@alexperemey6046](https://www.youtube.com/channel/UCchNS6618CdinWR5iznDcAQ)** *[07.12.2023 06:40](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwxtD1VlWUBi_Ycc554AaABAg.9pRDCRCd1I99y0CL8-6zJt)*

> В си ничего не теряется. В си ты пишешь ref A, присваиваешь в функции А хоть 5, хоть что угодно, и снаружи переданная переменная меняется. В жс у фиг так выйдет.

---

**[@vadimgiveToMeAccessPlease](https://www.youtube.com/channel/UCFsHfqXm65WIHi2QihNtL5Q)** *[29.05.2023 23:12](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugyl2vaYlGQLWuXE53F4AaABAg) · 👍 1*

Большое спасибо!

---

**[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[03.06.2023 15:33](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyN7ApSTg9Zf2a0HTt4AaABAg) · 👍 2*

А какой смысл копировать строки по значению, если мы не можем сделать что- то типа:

var str = 'VasyoK';
var str2 = str;

str2[3] = 'd'; // can't be done in JS to change character with index 3 to 'd'

Смысла нет в копировании. Рантайм поэтому и не копирует. str и str2 указывают на одну и ту же строку в памяти.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[04.06.2023 22:31](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyN7ApSTg9Zf2a0HTt4AaABAg.9qVddvJSaJ89qYyFFb3-bY) · 👍 1*

> Совершенно верно. И Вы только лишний раз подчеркнули тот факт, что фантазии людей на тему типов в JS являются ни чем иным кроме их фантазий. Потому, как в реальности это работает совершенно иначе.
> 
> В случае V8 все еще сложнее. Когда изменение части строки не обязательно приведет к ее копированию с изменениями. А приведет к созданию сложного обьекта с инкрементным его изменением. 
> 
> Но главное не это. Главное как раз то, что Вы и подчеркнули. Типы в JS не то, чем их описывают в типичном гайдлайне JS за 30 минут.

---

**[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[03.06.2023 15:41](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugz6sraz4OGsUwGVDnV4AaABAg) · 👍 1*

arr[] = str;

))) На PHP наверное кодил перед этим)

> **[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[03.06.2023 15:41](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugz6sraz4OGsUwGVDnV4AaABAg.9qVeXEvrd5d9qVebf8kC1Y) · 👍 1*

> Хорошо, хоть $ машинально не вставлял)

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[04.06.2023 22:28](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugz6sraz4OGsUwGVDnV4AaABAg.9qVeXEvrd5d9qYxwLnFJrQ) · 👍 1*

> И на PHP. И на Basic. И на Pascal. И на Fortran. И на Рапире.
> Подобная запись характерна для десятков диалектов.

---

**[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[03.06.2023 18:25](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxZj2Pejgp5behvEfZ4AaABAg) · 👍 1*

Если мы зафризим объект и передадим его в функцию, то после выхода из функции объект можно расфризить?

Если нет - то плохо))) Шемсединов прав, мы не можем временно зафризить объект.

А если у объекта есть вложенные объекты?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[04.06.2023 22:24](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxZj2Pejgp5behvEfZ4AaABAg.9qVxOqow59y9qYxXXEDf0W) · 👍 2*

> Это очень интересный вопрос, который на пальцах в комментарии не разобрать. Однако у него есть ответ. Я попробую сейчас описать его, но не уверен что у меня получится.
> 
> Сначала нужно задать себе вопрос - зачем мне нужно фризить обьект, при передачи его в функцию? Если мы касаемся типичных формулировок Тимура, то речь идет о том, что мы передаем в стороннюю функцию наш обьект, и хотим быть уверенными в том, что сторонний код не сделает ничего _плохого_
> 
> Если я прав в своем предположении то:
> JS давно предоставляет возможности проксирования обьектов. То есть передачи в функцию не самого обьекта, а прокси, которое позволит проконтролировать ВСЕ возможные манипуляции с ним. И, соответственно, выбрать только те, которые Вам нужны.  Не нравится Proxy? Используйте геттеры и сеттеры с тем же успехом. 
> 
> Как вероятно для Вас очевидно, совершенно все равно, при подобной схеме, сколько там вложенных обьектов. Потому что, теже Proxy можно генерировать вложенными сколько угодно, сохраняя полный контроль над каждый вложенным прокси. 
> 
> Это универсальное решение, которое никаким образом обойти сторонний код не сможет. Недостатком которого, служит только просадка в производительности в два раза по сравнению с тем, как если бы Вы передали просто обьект который бы не контролировали Proxy. 
> 
> Но и это еще не все.
> Вам же никто не мешает, предоставить в функцию пустой обьект, у которого прототипом является нужный изначально. Чего будет достаточно для того, чтобы сторонняя функция, могла получить нужные данные, а свои модификации записала как проперти того пустого обьекта который вы передали.  Вы же наверняка знаете как работает прототипное наследование.
> 
> Я могу Вам предложить еще 3 варианта решения этой задачи с разной степенью контроля за происходящим и соотвественно разным уровнем производительности, каждое из кототрых даст ответ на Ваш вопрос. 
> 
> Иными словами, при всем моему Уважении к Тимуру - он не прав. И если хочет этот оспорить, я готов на челендж, где я передаю в его функцию свой обьект, а он посторается сделать с ним что захочет таким образом, чтобы мой код не смог после этого корректно с этим обьектом работать. 
> 
> Все просто.

---

**[@SERGIUS_ORIGINAL](https://www.youtube.com/channel/UCorE8HdQ4HputSutpZpphFg)** *[18.06.2023 03:05](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzHshWRgpgz7s0lkZR4AaABAg)*

Спасибо за труд...

---

**[@thesunrock](https://www.youtube.com/channel/UCRjvmVEjQZpJO1tSEkCufig)** *[20.07.2023 14:17](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwYokmlwrt5esuytMN4AaABAg) (ред. 20.07.2023 16:10)*

1:04:42 - тут какой-то lexical environment выскочил при создании функции.
1:34:33 - каких таких переменных языка ECMAScript?

---

**[@alexjohnson4270](https://www.youtube.com/channel/UCcJpSU01QIH_QaT6putHJsQ)** *[25.09.2023 06:26](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyiNALT6novNhM_sUJ4AaABAg) (ред. 25.09.2023 06:36) · 👍 1*

43:59 что такое Коллекция в контексте JS ? В спеке определение объекта - коллекция свойств. Collection of properties. Как это правильно понимать?

---

**[@nikitalukashuk2978](https://www.youtube.com/channel/UCDElgvef4tF1N-QpDHytDRw)** *[04.10.2023 17:58](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyCFrCFhTkRoyZNUJ94AaABAg) · 👍 3*

шикарное видео, благодарю за контент)
единственное что , после использования лет и конст, не получается применять вот эту древообразную структуру, читаю спецификацию, пытаюсь снова построить себе всё это в голове, надеюсь где-то в последующих видео раскрою для себя этот момент

---

**[@radist126](https://www.youtube.com/channel/UCEUu730PG01zixc2DBd7QXQ)** *[27.10.2023 12:54](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyvJYMRXDRleoEbd114AaABAg) · 👍 3*

А GPT тоже умный😅
Вот, что пишет
—————
Если вы создаете переменную `s` и присваиваете ей значение `"slava"`, это действительно занимает некоторый объем памяти. При этом, если затем создать еще одну переменную `s2` и присвоить ей значение `s`, это не приведет к увеличению объема памяти, так как `s2` просто будет хранить ссылку на тот же самый участок памяти, где хранится значение `"slava"`. Новое пространство под это значение не выделяется.

Другими словами, `s` и `s2` ссылаются на один и тот же кусок памяти, поэтому нет необходимости выделять дополнительное пространство.

Если же вы создадите новую строку (например, `let s3 = "hello"`), то это уже будет занимать дополнительное пространство.

Надеюсь, это прояснило ситуацию. Если у вас есть еще какие-то вопросы, не стесняйтесь задавать их!

> **[@deniszh6688](https://www.youtube.com/channel/UCyAB29DoVGwFuLTe3RNGG1A)** *[06.12.2023 08:29](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyvJYMRXDRleoEbd114AaABAg.9wNIXvtaUXL9xyoxkvWrbQ)*

> А почему тогда, при изменении значения s2, например, на «slava2», переменная s продолжает содержать «slava»?

> **[@alexperemey6046](https://www.youtube.com/channel/UCchNS6618CdinWR5iznDcAQ)** *[07.12.2023 06:30](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyvJYMRXDRleoEbd114AaABAg.9wNIXvtaUXL9y0B8jc-q7U) · 👍 2*

> Потому что строки не изменяются (иммутабельны) и попытка присвоить новую строку переменной приводит к созданию новой строки отдельно в памяти и установке адреса на новый участок. Помним что написание в коде чего то в кавычках - это тоже выражение, а не просто отображение данных

> **[@sergey8366](https://www.youtube.com/channel/UC40kzB1rA5ELLzg98FI37Qw)** *[20.12.2023 19:37](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyvJYMRXDRleoEbd114AaABAg.9wNIXvtaUXL9yZ3XjU-bqS) (ред. 18.04.2024 02:34)*

> @deniszh6688 мм ,а должна что?

---

**[@РоманМ-й5ш](https://www.youtube.com/channel/UCpYKvj2Z-GzTBetoS8JYDKw)** *[31.10.2023 17:12](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzjvD_S6gXOI9Lk0J94AaABAg)*

не спорю с самой идеей, но эксперимент с памятью в браузере не показателен, потому что если мы создадим второй идентификатор и присвоим ему точно такую же строку, то память тоже не увеличится, тут, похоже,  в действие вступает какая-то другая оптимизация, что под одинаковые значения память в принципе не выделяется

> **[@alexperemey6046](https://www.youtube.com/channel/UCchNS6618CdinWR5iznDcAQ)** *[06.12.2023 11:26](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzjvD_S6gXOI9Lk0J94AaABAg.9wY3DeAa9IJ9xz8CubwlS6) · 👍 4*

> Она не увеличится потому как будет ссылка на ту же область памяти. Именно потому примитивы сделали иммутабельными, иначе изменяя строку через одну переменную мы бы ее меняли везде, и в других переменных.

> **[@alexperemey6046](https://www.youtube.com/channel/UCchNS6618CdinWR5iznDcAQ)** *[06.12.2023 11:29](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzjvD_S6gXOI9Lk0J94AaABAg.9wY3DeAa9IJ9xz8_Xm6_t_) · 👍 2*

> Это не оптимизация браузера, это js так работает

---

**[@nihttoter3240](https://www.youtube.com/channel/UC2hVOUPwfFwW5pCny8Ndd9g)** *[27.11.2023 23:33](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg) · 👍 2*

Мужик, если ты ищешь термин для того, чтобы описать адрес ячейки в памяти и тебе не нравится "ссылка", то можно использовать термен "указатель" :) Наслаждайся :)

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[30.11.2023 23:33](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9xkzeVE8bx_) · 👍 1*

> Спасибо мужик!!!
> Одна проблема, как теперь сделать так, чтобы программисты на других языках точно поняли о чем я говорю. Потому, что "указатель" это нихуа не аналог адреса доступа к ячейке памяти. 
> По крайней мере для всех и всегда.

> **[@nihttoter3240](https://www.youtube.com/channel/UC2hVOUPwfFwW5pCny8Ndd9g)** *[01.12.2023 07:22](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9xlpKfMFZYf) (ред. 13.06.2024 21:35)*

> @AsForJS в плюсах это называется указатели. А плюсы учат все.

> **[@alexperemey6046](https://www.youtube.com/channel/UCchNS6618CdinWR5iznDcAQ)** *[06.12.2023 11:56](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9xzBijRSOh2)*

> Все дело в том, что передача по ссылке работает не так. Кто с++ учил, это знает. Я бы сказал наоборот, все передается только по значению, но все значения в жс - это указатели. Т.е. возле каждого var если поставить * то будет видно как оно работает, для тех кто си учил

> **[@alexperemey6046](https://www.youtube.com/channel/UCchNS6618CdinWR5iznDcAQ)** *[06.12.2023 12:00](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9xzC9CtvMfF)*

> Т.е. я согласен с твоим термином указатель, но похоже ты считаешь, что передачей по ссылке это тоже корректно назвать, но имхо нет

> **[@nihttoter3240](https://www.youtube.com/channel/UC2hVOUPwfFwW5pCny8Ndd9g)** *[06.12.2023 12:12](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9xzDUCASAi3) (ред. 13.06.2024 21:35)*

> @alexperemey6046 Буду рад, если вы поподробнее объясните тем отличается перадача объекта в функцию в условном C#, Java и т.д. от стандартной передачи объекта в функцию в JS. Имхо, одно и тоже. Но мб, я C# забыл.

> **[@alexperemey6046](https://www.youtube.com/channel/UCchNS6618CdinWR5iznDcAQ)** *[06.12.2023 12:35](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9xzG59MfdWS)*

> Указатели тоже не сильно подходят. Указатели явно задают адреса, переменные жс неявно. Т.е. технически это скорее ссылки, а не указатели. Круг замкнулся. В общем, терминология вроде в спецификации правильная и говорят учителя правильно, только они говорят абстрактно, без привязки к железу. А мурыч переводит эти термины на железо и потому его бомбит. Просто программирование стало такое высокоуровневые, что при передаче по значению физически никакого по значению не происходит

> **[@nihttoter3240](https://www.youtube.com/channel/UC2hVOUPwfFwW5pCny8Ndd9g)** *[06.12.2023 12:44](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9xzH8GZriJg) (ред. 13.06.2024 21:35)*

> @alexperemey6046 Короче, я повспоминал. Передача объекта в функцию в JS работает также, как передача объекта в функцию в C# c ключевым словом ref. ref - ссылка.

> **[@alexperemey6046](https://www.youtube.com/channel/UCchNS6618CdinWR5iznDcAQ)** *[07.12.2023 06:12](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9y0953zBxif) · 👍 2*

> В том то и дело, что есть принципиальное отличие. Когда ты пишешь ref A, ты можешь потом в функции написать А = 5 и значение внешней А изменится, за пределами функции. В этом весь смысл передачи по ссылке. Чтобы не локально внутри функции только менять, но чтобы изменения оставались, в каком то смысле это аналог return. А в js вот ни фига не так. Передавая А, и делая потом в функции А = 5, ты никак не влияешь на ту А, что передал, если только не обратишься к внутреннему свойству. Я помню как меня это удивляло, когда я ждал, что переменные будут передаваться по ссылке, как мне рассказали... И я интуитивно начал представлять передаваемую переменную как адрес, по которому можно обратиться вглубь, но который перетираешь при прямом присваивании... Ближе всего это указатель, но указатель можно посмотреть, с ним можно оперировать как с указателем. А тут к нему доступа нет и прямое обращение даёт сразу значение на которое он указывает. Т.е. чтение автоматом даёт операцию *А, как в ссылках, а вот запись идёт как А*

> **[@alexperemey6046](https://www.youtube.com/channel/UCchNS6618CdinWR5iznDcAQ)** *[07.12.2023 06:16](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9y09W0RSLHC)*

> Ютуб съел * и выделил жирным должно быть (звездочка)А вначале и А(звездочка) в конце жирного выделения

> **[@AvigdorKatz](https://www.youtube.com/channel/UCk6X3w_IO90tJpulmBkPE9w)** *[08.12.2023 21:04](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9y4JzHT52I2) (ред. 13.06.2024 21:35)*

> ​@alexperemey6046Спасибо, теперь, кажется, стало понятнее о чем Мурыч говорит. А то в его речи он сам постоянно норовит назвать значение идентификаторов ссылками и тут же ругает формулировку о передаче по ссылке. Звучит на первый взгляд это словно лишь филологические придирки.

> **[@alexperemey6046](https://www.youtube.com/channel/UCchNS6618CdinWR5iznDcAQ)** *[08.12.2023 21:27](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9y4MagcPXa3) (ред. 13.06.2024 21:35)*

> @AvigdorKatz Их может и можно считать ссылками в некоем смысловом значении, и спецификация вроде как этим термином оперирует, но классического механизма "передача по ссылке" нет. Как нет и передачи по значению.

> **[@sergey8366](https://www.youtube.com/channel/UC40kzB1rA5ELLzg98FI37Qw)** *[19.12.2023 21:51](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9yWj8MmMyPz) (ред. 13.06.2024 21:35)*

> ​@alexperemey6046 
> все равно не понял принципиальной разницы
> > Когда ты пишешь ref A, ты можешь потом в функции написать А = 5 и значение внешней А изменится, за пределами функции. 
> 
> ближайший аналог ** - указатель на указатель
> оффоп: вроде всях есть const& которой и локально ничего не присвоишь? давно это все было - забыл))
> 
> >Передавая А, и делая потом в функции А = 5, ты никак не влияешь на ту А, что передал, если только не обратишься к внутреннему свойству
> 
> так же с# работает для типов со ссылочной семантикой без ref
> 
> >Ближе всего это указатель, но указатель можно посмотреть, с ним можно оперировать как с указателем. 
> 
> внутрь через точку - по смыслу аналог разыменования указателя, просто синтаксического шума нет. а от "посмотреть адрес" и адресной арифметики абстрагировано и слава яйцам. еще не хватало segmentation fault ловить в таких высокоуровневых языках.
> 
> >тем отличается перадача объекта в функцию в условном C#, Java и т.д. от стандартной передачи объекта в функцию в JS.
> 
> ничем. тоже самое как в C# Java передаются объекты по-умолчанию без модификаторов ref/out (в даже их и нету вроде). в js особенность это окружения и области видимости. в C#, Java они работают по-другому + от реализации больше абстрагировано (хоть на стек ложи, хоть в кучу, хоть в корзинку с волшебными бобами - лишь бы семантика соблюдалась). в js это отчасти вытащено наружу. а дальше люди в словах запутались. боюсь спрашивать а что такое вообще в принципе "тип"? тут таки кампутерсаенс глубины можно открыть, что лучше не педалировать тему (вы молодые, смешливые...))) а словом все бросаются не задумываясь
> 
> вот как раз аналога value семантики из c# в js не видно (и в java тоже). иммутабельные значения не предлагать - для них ссылочная прозрачность, которая обессмысливает вопрос

> **[@sergey8366](https://www.youtube.com/channel/UC40kzB1rA5ELLzg98FI37Qw)** *[19.12.2023 22:40](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9yWokbUbsV-) (ред. 13.06.2024 21:35)*

> @AvigdorKatz 
> 
> >А то в его речи он сам постоянно норовит назвать значение идентификаторов ссылками 
> 
> и правильно норовит.  он слышит "передача по ссылке" и представляет 
> func(object& x) //адреса не видно,  присваивания вида  x = new object() видны снаружи
> или
> func(object* х)
> //адрес видно, присваивая x = new object() снаружи не видно(сам указатель по значению пришел). 
> //но сам объект можно менять. то есть писать по адресу памяти, в который х указывает. то есть (*x) = new object() снаружи таки видно
>  //(*x).Prop = someValue тоже видно если обьект мутабельный
> или упаси господь
> func(object** x)//ваще анархия караул - можно вызывающего на другой адрес переслать и положить туда что хочешь
> 
> и всё это не то как в js
> 
> а шарпист вроде меня представляет reference семантику из c# и все работает. это как если в случае с func(object* х), но (*x)= запрещено, но (*x).Prop = someValue можно. но адреса не видно как и в func(object& x). получается а-ля "всегда разыменованный  указатель" с которым можно только через ->. а сам он (*x) или если не путаю есть такое x->*. не знаю можно ли такое с сях изобразить - подскажите кто если в треде крестоебы есть.
> 
> короче, после семестра c/c++ все просто и понятно. а здесь запутались в словах + фронтенд-макаки (сорян если что - это не про человеческие качества) зачастую вайтивайтишники без бэкграунда и им вообще хз на каком языке обьяснять

---

**[@Boortwint](https://www.youtube.com/channel/UC1f_N0jDDOe992KFLVbDk9Q)** *[28.11.2023 04:41](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugy-CmkNFhimMB9nUqJ4AaABAg) (ред. 28.11.2023 05:55)*

Мурыч толкает спич на 35:20 про отсутствие любой информации о примитивах в спецификации, а в это время на экране открыта спека, в которой красуется таблица с описанием символа Symbol.toPrimitive

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[30.11.2023 23:31](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugy-CmkNFhimMB9nUqJ4AaABAg.9xdo_kPFiCT9xkzPgVXvA1)*

> Это функция приведения не к  Primitive Type, НО к Primite Value.
> Смотрите видео я тип простой я говорю стихами.
> 
> или разберитесь наконец что такое Primitive Value в  JS.

> **[@Boortwint](https://www.youtube.com/channel/UC1f_N0jDDOe992KFLVbDk9Q)** *[01.12.2023 00:36](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugy-CmkNFhimMB9nUqJ4AaABAg.9xdo_kPFiCT9xl5q4IFQr0) (ред. 18.04.2024 01:43) · 👍 2*

> @AsForJS В спецификации JS5 написано, что toPrimitive свой приводит аргумент к *примитивному типу*
> Пункт 9.1. спецификации:
> ToPrimitive # Ⓣ 
> Абстрактная операция ToPrimitive (К примитиву) принимает аргумент input (входной) и необязательный аргумент PreferredType (Предпочтительный тип). Абстрактная операция ToPrimitive *преобразует* свой аргумент input *в тип, не являющийся объектным.* Если объект может быть преобразован более чем к одному *примитивному типу,* то для выбора может быть использована необязательная подсказка PreferredType.

---

**[@Boortwint](https://www.youtube.com/channel/UC1f_N0jDDOe992KFLVbDk9Q)** *[28.11.2023 05:54](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugzv5L8ByBr1NGqQjHJ4AaABAg)*

1:02:27 а что там с let и const? Назначив идентификаторы с помощью этих ключевых слов, у разработчика ведь нет возможности обратиться к ним как к свойству объекта. Такие объявления не создают свойства в глобальном объекте. 
Да и к var внутри функции раньше можно было обратиться как к свойству объекта, представляющего из себя некое подобие контекста исполнения функции в отдельных браузерах, но теперь такой возможности давно уже нет.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[30.11.2023 23:29](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugzv5L8ByBr1NGqQjHJ4AaABAg.9xdwwH5EBK69xkzGyEfRLL)*

> Свойства в глобальном обьекте создаются только для идентификаторов создаваемых в Global Enviroment.
> 
> Это единсвенное место где let может конкурировать с var в производительности и то только в случае, когда RunTime не оптимизирует работу var для этого случая.
> 
> Если говорить о практике, то ни один нормальный код не формирует работу своей логики в Global Enviroment, но изолирует ее образом чтобы не оказывать на него влияние. 
> 
> Как следствие, даже если по каким то причинам не работает оптимизация var для Global Env, если программист знает что он делает, то он будет работать ВНЕ GLOBAL,  что автоматически говорит о том, что let будет медленнее var.
> 
> С третей стороны, проигрыш let перед var это чепуха в сравнее с тем, как программисты используют rest, spread, async что перекрывает с точки зрения потребления ресурсов любые вопросы про let vs var

---

**[@КимЧенОрк](https://www.youtube.com/channel/UCVsJ5IlcPWwrrNtepcGGYYw)** *[03.12.2023 10:31](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwoJj5aggrqNxIdZht4AaABAg)*

так, каждая ссылка занимает около 8бит в globalObject?

---

**[@germanburdin743](https://www.youtube.com/channel/UCckwJJl0-ayIIaxkaxdJl1w)** *[04.12.2023 20:43](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyaYF16aa22SQYMQGl4AaABAg)*

The abstract operation ToPrimitive takes argument input (an ECMAScript language value) and optional argument preferredType (string or number) and returns either a normal completion containing an ECMAScript language value or a throw completion. It converts its input argument to a non-Object type. If an object is capable of converting to more than one primitive TYPE, it may use the optional hint preferredType to favour that type. 
Объясните тогда пожалуйста, почему в спецификации в 7.1.1 ToPrimitive ( input [ , preferredType ] )
говорится про примитивный ТИП?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[04.12.2023 21:11](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyaYF16aa22SQYMQGl4AaABAg.9xuzNk8tDdJ9xv1edeuizT)*

> нет.
> говорится про выбор по умолчанию для абстрактной операции то примитив. 
> 
> єто абстрактная операция, приводит передаваемый аргумет к primitive value.
> 
> читайте внимательно.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[04.12.2023 21:15](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyaYF16aa22SQYMQGl4AaABAg.9xuzNk8tDdJ9xv21qyOasF)*

> речь идет о предпочитаемое типе - prefered type.
> 
> какой именно type для primitive value должен быть выбран.
> 
> єто не имеет никакого отношения к примитивным типам.

> **[@germanburdin743](https://www.youtube.com/channel/UCckwJJl0-ayIIaxkaxdJl1w)** *[04.12.2023 23:51](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyaYF16aa22SQYMQGl4AaABAg.9xuzNk8tDdJ9xvJx6d0hQL) (ред. 14.06.2024 01:15)*

> @AsForJS
> 
> Понял ваши тезисы, но цитирую:
> «If an object is capable of converting to more than one primitive *type*,…» 
> Именно type написано в спецификации, а не value… 
> Других сочетаний primitive type в спецификации действительно нет, но тут всё-же присутствует

> **[@SerzhNesteruk](https://www.youtube.com/channel/UCvSxoIuRvinnq_mbU2KDTPA)** *[06.12.2023 11:59](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyaYF16aa22SQYMQGl4AaABAg.9xuzNk8tDdJ9xzC2QEldWf) (ред. 14.06.2024 01:15)*

> ​@AsForJS Вопрос другого порядка: Можно ли называть типы данных примитивными (primitive data type), если значения этих типов являются примитивами (primitive value)?.. Или вы отказываете JS-сообществу в праве использовать понятие «примитивные типы данных», основываясь на том, что этого понятия нет в официальной спецификации? Будьте тогда последовательны: запрещайте использовать и понятие «JavaScript», его ведь тоже нигде нет в спецификации. 😏
> 
> Вот, что о примитивных типах данных (коих, по-вашему, в JS якобы не существует) сказано в MDN Web Docs Glossary:
> «Primitive
> In JavaScript, a primitive (primitive value, primitive data type) is data that is not an object and has no methods or properties. There are 7 primitive data types: string, number, bigint, boolean, undefined, symbol, null... This page was last modified on Jun 8, 2023 by MDN contributor»

> **[@alexperemey6046](https://www.youtube.com/channel/UCchNS6618CdinWR5iznDcAQ)** *[07.12.2023 06:45](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyaYF16aa22SQYMQGl4AaABAg.9xuzNk8tDdJ9y0Cr13NB1u)*

> Использовать можно что угодно, проблема когда человек воспринимает эти термины так, как он привык (и как оно и есть) в компилируемых языках, где примитивные типы - действительно содержат только данные. То, что в программировании отсутствует единая однозначная терминология

> **[@SerzhNesteruk](https://www.youtube.com/channel/UCvSxoIuRvinnq_mbU2KDTPA)** *[15.12.2023 13:02](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyaYF16aa22SQYMQGl4AaABAg.9xuzNk8tDdJ9yLUQX06nPY) (ред. 14.06.2024 01:15)*

> @alexperemey6046 Согласен. Но всё же лучше использовать терминологию, которая является общепринятой в конкретном языке программирования. В разных языках одни и те же понятия могут иметь совершенно другие значения. Например, тип данных в некоторых языках программирования может быть у классов, переменных, операторов. В JavaScript же тип есть только у значений. Согласно пункту 6.1 спецификации ES2023, тип соответствует значениям, а значения характеризуются типом. Таким образом, утверждение, что value в JS не имеет никакого отношения к type, является в корне ошибочным, поскольку не соответствует спецификации. А если мы обратимся к определению типа в той же спецификации (пункт 4.4.4), то окажется, что тип данных в JavaScript — это всего лишь множество допустимых значений. Поэтому характеристика primitive, применимая ко всем значениям некоего типа, вполне корректно может быть применена и к самому этому типу. Таких типов в JS аж целых 7, согласно самой спецификации (пункты: 4.4.5, 4.4.13, 4.4.15, 4.4.18, 4.4.20, 4.4.23, 4.4.28, 4.4.31). А в пункте 7.1.1 (который нам приводит German Burdin) как раз есть упоминание о преобразовании в примитивный тип (primitive type), значение которого не является объектом. Что полностью согласуется с определением примитива в MDN Web Docs Glossary.

---

**[@POEOneLove](https://www.youtube.com/channel/UCYwf194nU1OOcOgrdxp_STw)** *[05.12.2023 05:41](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxf9DPoZlAVEJFclQV4AaABAg) (ред. 05.12.2023 05:42) · 👍 6*

Раньше, чтобы выкопать большую яму нужно было пол дюжины рабочих, лопат, еда и вода. Сейчас всего 1 рабочий, но умеющий управляться с многовесящей абстракцией на лопату - экскаватором. И знающий базовые принципы копания ям лопатами. Но не сильно глубокими. По этому все эти eax ebx в прошлом. Да и 16гб оперативки это также доступно как и ранее 512килобайт. Все это скорее немного познавательно, чем полезно

> **[@northwest569](https://www.youtube.com/channel/UCf3gBcrnYkbAXgsl6dZkVSA)** *[11.06.2024 17:33](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxf9DPoZlAVEJFclQV4AaABAg.9xvwxg_QRaXA4Ysjc9S2rL) · 👍 1*

> В корне не согласен! Вы исходите из неверной предпосылки, что копать дурацкую яму - тоже самое что писать высокопроизводительный код.

> **[@POEOneLove](https://www.youtube.com/channel/UCYwf194nU1OOcOgrdxp_STw)** *[11.06.2024 17:53](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxf9DPoZlAVEJFclQV4AaABAg.9xvwxg_QRaXA4YuydCAUsi)*

> @northwest569 Высокопроизводительный код это очень узкая ниша. 99.9 случаев в жизни это простое программирование разных приложений под бизнес задачи. Остаётся только выбрать качественный оптимизированный экскаватор, чтобы выкопать нужную яму. Пускай не с идеально ровными краями, однако задача будет выполнена. И быстрее, чем писать на низком уровне.

> **[@northwest569](https://www.youtube.com/channel/UCf3gBcrnYkbAXgsl6dZkVSA)** *[11.06.2024 18:13](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxf9DPoZlAVEJFclQV4AaABAg.9xvwxg_QRaXA4YxGc0ndQt) · 👍 1*

> @POEOneLove "простое программирование" - опасный термин. Не поймите меня неправильно, но речь идёт именно о ямах с идеально ровными краями. Конечно, делать качественно или делать посредственно - выбор каждого, но это не отменяет того факта, что есть качество и есть посредственность. Все верно, кривая и косая яма, которая обсыпается через 2 недели - тоже яма, но именно в этом и проблема. Сегодня большая часть ям именно такие. Это факт, но факт печальный. Экспертиза драматически падает.

> **[@POEOneLove](https://www.youtube.com/channel/UCYwf194nU1OOcOgrdxp_STw)** *[11.06.2024 18:49](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxf9DPoZlAVEJFclQV4AaABAg.9xvwxg_QRaXA4Z0KqZZUnZ) (ред. 11.06.2024 18:49)*

> @northwest569 я говорю в широком понимании. Есть узкие ниши, где нужно точечно оптимизировать каждую строку и не только. Такое бывает. Но В плане js это просто придаток браузера. Там на коленке все работает

> **[@northwest569](https://www.youtube.com/channel/UCf3gBcrnYkbAXgsl6dZkVSA)** *[11.06.2024 18:54](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxf9DPoZlAVEJFclQV4AaABAg.9xvwxg_QRaXA4Z0vlyOOL_) · 👍 1*

> @POEOneLove Это не придаток браузера, а полноценный язык программирования, со своими правилами и нюансами, которые (коль скоро вы считаете себе профессионалом) НАДО знать. Об это канал.

> **[@POEOneLove](https://www.youtube.com/channel/UCYwf194nU1OOcOgrdxp_STw)** *[11.06.2024 19:13](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxf9DPoZlAVEJFclQV4AaABAg.9xvwxg_QRaXA4Z36LBN1YD)*

> @northwest569 С бородатых времён, на моей памяти с 2004 года, js это скриптовый придаток браузера. Нужен для работы с html тегами. И сейчас он делает тоже самое по сути и не самостоятелен без браузера.

> **[@northwest569](https://www.youtube.com/channel/UCf3gBcrnYkbAXgsl6dZkVSA)** *[12.06.2024 04:16](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxf9DPoZlAVEJFclQV4AaABAg.9xvwxg_QRaXA4_1HZspNqw)*

> @POEOneLove 🫡🫡🫡

> **[@Ivan-l1d8c](https://www.youtube.com/channel/UC17uUtQI-y24MKpxFSpXBwQ)** *[15.06.2024 05:34](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxf9DPoZlAVEJFclQV4AaABAg.9xvwxg_QRaXA4gtZc2XvRv) · 👍 1*

> ⁠​⁠@POEOneLoveчто ты несешь? Как ты понял, что это скриптовый язык, из слова «script» в наименовании? Какой тебе 2004, ты либо бездарь, либо еще одно молодое дарование. Думаю говорить про твои тейки «не самостоятелен» и «нужен для html тегов», нет смысла, даже само определение пахнет слабостью

> **[@Ivan-l1d8c](https://www.youtube.com/channel/UC17uUtQI-y24MKpxFSpXBwQ)** *[15.06.2024 06:05](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxf9DPoZlAVEJFclQV4AaABAg.9xvwxg_QRaXA4gx4iOPS1n)*

> @POEOneLoveвот еще пару тейков с моей стороны. Что определят полноценный язык программирования, если сам язык это набор спецификаций и правил, а компилятор/интерпретатор может быть написан вообще на другом языке программирования (например GCC для C изначально был написан на ассемблере и только спустя время он смог выполнять сам себя)? И получается по твоей логике, люди работающие на Spring — скрипт-киди разработчики, а не Java?

> **[@POEOneLove](https://www.youtube.com/channel/UCYwf194nU1OOcOgrdxp_STw)** *[15.06.2024 09:10](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxf9DPoZlAVEJFclQV4AaABAg.9xvwxg_QRaXA4hHMNOSFwa) (ред. 15.06.2024 09:17)*

> @Ivan-l1d8c сейчас какого только мусора нет. Миллионы абстракций на языки и языки новые наверное уже каждый день появляются. Берём столпы. Java - да. C# да, php - тоже скриптовый язык, однако может запускаться самостоятельно из консоли операционки. В отличие от js - просто придатка браузеров. Js не возможно установить отдельно, это просто скриптовый описательный прикол для html манипуляций, чтоб менеджеры продуктов балдели от анимаций и плавных загрузок. И кстати на ассемблере написано по сути всё, это уже прямой язык общения с компьютерным железом. Нет ничего удивительного в этом. До ассемблера остаётся писать нулями и единицами или в шестнадцатиричной системе

> **[@POEOneLove](https://www.youtube.com/channel/UCYwf194nU1OOcOgrdxp_STw)** *[15.06.2024 09:25](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxf9DPoZlAVEJFclQV4AaABAg.9xvwxg_QRaXA4hJ13jJjco)*

> @Ivan-l1d8c php - скриптовый. Js - скриптовый. У них нет компилятора. Есть интерпретаторы. И в случае с js - это придаток браузера (только браузер его понимает и интерпретирует только "в себя"). Бездарь ты, пытающийся сказать что-то про ассемблер, даже не понимая что это платформа всего сущего.

> **[@POEOneLove](https://www.youtube.com/channel/UCYwf194nU1OOcOgrdxp_STw)** *[15.06.2024 09:37](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxf9DPoZlAVEJFclQV4AaABAg.9xvwxg_QRaXA4hKQ0-X-Ng)*

> @Ivan-l1d8c Изначально уже потерян смысл моего тезиса. Повторю ещё раз. В упрощённом виде. В современном мире в большинстве случаев не нужно знать ассемблер и другие совсем низкоуровневые приколы, чтобы спокойно работать в области программирования. Не думаю что университетские знания ассемблера и программирования микроконтроллеров дадут вам+ 100к к зарплате js разработчика.

---

**[@noname-tm](https://www.youtube.com/channel/UCfHqM6Pwyg3UE_35ehh-pwg)** *[05.12.2023 18:27](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwHjRr9vgxwX9Bv3Hx4AaABAg)*

в пункте 4.4.5 primitive value указано что это член одного из типов Undefined, Null, Boolean, Number, BigInt, Symbol, or String

---

**[@anton5988](https://www.youtube.com/channel/UCnehPn4-iCLIabpEF3Kqk4w)** *[07.12.2023 17:17](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzFcrXd2gbM9bavOVJ4AaABAg) · 👍 2*

Мурыч, жениться тебе надо ) А вообще интересно смотреть, харизма есть ) У Тимура был на лекции, лично видел как к концу лекции 1/3 зала осталось, очень скучно, монотонно, не понятно. У тебя же иногда тоже не понятно, исключительно из-за моего скудного уровня, но интересно ) Продолжай !)

---

**[@artemlobanchikov2270](https://www.youtube.com/channel/UChru55x00cH0RBxFqD6FVww)** *[08.12.2023 06:15](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzNViI65KnJsbggltl4AaABAg)*

28:20 - :DDDD , действительно смешно))

---

**[@AvigdorKatz](https://www.youtube.com/channel/UCk6X3w_IO90tJpulmBkPE9w)** *[08.12.2023 22:22](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwD7FTgxHxjA2xwCJZ4AaABAg) (ред. 10.12.2023 18:03)*

Я что-то не понял почему var str3 = s + s; не должно привести к трехкратному увеличению снимка. Можете пояснить?

Еще есть вопрос к методике проверки. Мне кажется, тут как в тестировании нужно было бы сначала продемонстрировать инварианты - случаи когда создаются копии строки приводящие к кратному увеличению размера снимка памяти. А уже после этого демонстрировать поведение отличное от этого. Если я правильно понял, то примеры кода
var str2 = str.slice(3); 
или
var str2 = 'aaaaaabcb' + str.slice(9);
ввиду иммутабельности значения должны создавать измененные копии строки в памяти и размер снимка должен увеличится. Но этого не происходит. Почему так и можно ли тогда в таком контексте говорить о том, что пример со снимками памяти вообще что-то доказывает? Если что, я не пытаюсь доказать, что ваше утверждения неверны.

PS. Благодаря статье iliazeus . github . io  *  articles  *  js-string-optimizations-en  стало понятно почему слайсы с конкатенациями не работают. Они не копируют данные а лишь содержат ссылки на оригинальные данные и метаданные о смещении от начала строки, длинне и тд. Удалось добится нужного результата с помощью функции инверстирования строки с помощью Array.prototype.reduce.call(str, (reverseStr, char) => reverseStr += char, '')) и применил её дважды подряд var str2 = reverseString(reverseString(str));

Вообще в своём варианте кода я не вставлял строковый литерал, а написал функцию которая генерирует строку необходимой длинны наполняя её произвольными символами из массива возможных символов. Например в моём наборе символов отсутствует звездочка. И можно использовать дважны замену символа var str2 = str.replaceAll('x', '*').replaceAll('*', 'x');

Любопытно так же, что если в кода двум переменным присвоить одинаковые строки var str = 'abcd...'; и var str2 = 'abcd...'; то в размер занятой памяти не будет в два раза больше. Эта оптимизация так же описана в статье под заголовком Internalized. Строковые литералы помещаются в некое подобие внутреннего хеша строковых литералов. И если вы где-то в коде будете присваивать точно такую же строку, то это будет оптимизированно ссылкой на соответсвующее значение в "хеше" строковых литералов вместо создания данных новой копии строки в памяти.

---

**[@havrilyk4115](https://www.youtube.com/channel/UCOoeGRsHq4tjSnWjr8-Nndw)** *[11.12.2023 20:01](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwVB_tO5aHIUHEAC914AaABAg) · 👍 5*

Ого, пан Мурич, розбирає частини лекцій Шемседінова.
Це можна дивитись як серіал.
(Але з важливим контекстом)
Дякую)))

---

**[@it-coding](https://www.youtube.com/channel/UC45uzC-zp5ZnGY9Iy9iuQIw)** *[17.12.2023 18:07](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyBZ__Jumf8HHfmUjt4AaABAg)*

В Chrome devtools видны адреса и все так, строки передаются в фукцнию и в другие переменные с тем же адресом, но вот с числами не получается этого увидеть в devtools

> **[@it-coding](https://www.youtube.com/channel/UC45uzC-zp5ZnGY9Iy9iuQIw)** *[17.12.2023 18:13](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyBZ__Jumf8HHfmUjt4AaABAg.9yRAsIq2WBs9yRBWG-lOwI)*

> хотя получилось , если установить число 0.02 , то в DevTools получается увидеть эти значения и их адреса "::heap number@6427"  и @6427 совпадает с оригиналом и внутри функции , экспериментально подтверждается ))

---

**[@asifabbasov3801](https://www.youtube.com/channel/UCJq12iicPMYDbJr_1OGr4qQ)** *[17.12.2023 20:00](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzL9wNGoLMzLOkB4xh4AaABAg)*

Спасибо за ваши выпуски

---

**[@yomo1abh586](https://www.youtube.com/channel/UCoCgTB0pDpma-m1KK4j6dqA)** *[18.12.2023 14:37](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzBfufUdYwIKYfrt2V4AaABAg)*

Не совсем понял, что происходит с числами. 
Если а = 2 и мы перезапишем на 3, то поменяется ссылка на область памяти?

> **[@AlexeyPack](https://www.youtube.com/channel/UChNb-mCtzhLbDCt9yVsvoGg)** *[05.01.2024 20:12](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzBfufUdYwIKYfrt2V4AaABAg.9yTNchjv9wJ9zCKFaGX4QL)*

> нет. адрес в памяти поменяется только если одна переменная присвоит другую (обе переменных будут ссылаться на один адрес в памяти) и после одна из переменных изменяет вое значение. если вы просто будете менять значение в переменной то, по адресу в памяти поменяются данные

---

**[@WewasKangs-bd9eb](https://www.youtube.com/channel/UCYLIpcmQ6QoFk2KWGx1BLrg)** *[19.12.2023 20:03](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxRBwxdOzldBFhXyVh4AaABAg) · 👍 1*

В спеке написано куча лабуды, необходимой для корректной имплементации компилятора, но не дающей пользователю языка никаких преимуществ и даже запутывающей пользователя до такой степени, что он может и впрвду подумать, что в "JS нет передачи по значению".
В JS может и нет, а в скриптах, написанных на JS - есть. И для юзера есть только такая:
function Test(a){a++};
var b = 1;
test(b)
b==1 //true
Зачем юзеру знать или думать про регисторы процессора, про иммутабельные объекты, переданные по поинтеру?

> **[@sergey8366](https://www.youtube.com/channel/UC40kzB1rA5ELLzg98FI37Qw)** *[20.12.2023 19:43](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxRBwxdOzldBFhXyVh4AaABAg.9yWXkw8ZqXt9yZ4DsNcq5k)*

> что это по-вашему должно доказывать и каким образом?

> **[@sergey8366](https://www.youtube.com/channel/UC40kzB1rA5ELLzg98FI37Qw)** *[20.12.2023 19:49](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxRBwxdOzldBFhXyVh4AaABAg.9yWXkw8ZqXt9yZ4wwV6CAV)*

> >иммутабельные объекты, переданные по поинтеру
> 
> иммутабельность дает ссылочную прозрачность. про них вопрос по ссылке/по указателю имеет ровно нихуя смысла и ваш пример показывает ровно нихуя кроме иммутабельности. да и про стек/кучу нормальные языковые спеки не говорят. хоть через астральный образ в супрематическом подпространстве передавай. если предписанная семантика выполняется, то кого ебет

> **[@WewasKangs-bd9eb](https://www.youtube.com/channel/UCYLIpcmQ6QoFk2KWGx1BLrg)** *[20.12.2023 20:28](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxRBwxdOzldBFhXyVh4AaABAg.9yWXkw8ZqXt9yZ9PmmIIWv) (ред. 13.06.2024 22:18)*

> @sergey8366 очевидно, что пример должен продемонстрировать, что хоть "примитивные" параметры и передаются по референсу, для пользователя языка это будет выглядеть, как будто они всегда передаются по значению. И писать программы намного проще держа в голове простое правило: примитивы - по значению, объекты - по референсу. Хоть мы и знаем, что в JS абсолютно всё объект. Даже null.

> **[@sergey8366](https://www.youtube.com/channel/UC40kzB1rA5ELLzg98FI37Qw)** *[20.12.2023 21:23](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxRBwxdOzldBFhXyVh4AaABAg.9yWXkw8ZqXt9yZFicUAkkw) (ред. 13.06.2024 22:18)*

> @WewasKangs-bd9eb а как бы выглядело, если бы иммутабельные значение передавались "как будто" по ссылке?

> **[@WewasKangs-bd9eb](https://www.youtube.com/channel/UCYLIpcmQ6QoFk2KWGx1BLrg)** *[20.12.2023 21:29](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxRBwxdOzldBFhXyVh4AaABAg.9yWXkw8ZqXt9yZGKdEc-g6) (ред. 13.06.2024 22:18)*

> @sergey8366 По-моему вы не понимаете, что я пишу. Извините, если проблема в моем косноязычии, но смысла писать 3 раза одно и то же не вижу.

> **[@sergey8366](https://www.youtube.com/channel/UC40kzB1rA5ELLzg98FI37Qw)** *[20.12.2023 22:23](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxRBwxdOzldBFhXyVh4AaABAg.9yWXkw8ZqXt9yZMZBxpVsx) (ред. 13.06.2024 22:18)*

> ​@WewasKangs-bd9eb мне кажется понимаю, просто вы хотите странного. по-моему под "передачей по значению" в js подразумевают непонятно что потому-что никто не может сказать как бы это выглядело, если бы существовало. вот вы говорите "обьекты передаются по референсу". ок, создадим для обьекта аналогичную ситуацию как и для инта
> 
> function Test(a)
> {
> //a .name = ''tt" не аналогично тк это мутация,  ++ же вычисляеет новое значение беря за основу старое из а и присваивает его идентификатору а 
> a={name="tt"}
> };
> var b = {name: "gg"};
> test(b)
> console.log(b);
> //видим {name: "gg"}
> 
> >. И писать программы намного проще держа в голове простое правило: примитивы - по значению, объекты - по референсу
> 
> выходит разницы между мифическим "по значению" и "по референсу"не прослеживается. или приведите пример где ее можно увидеть. ну или забейте на спор с душнилой в инете;). 
> 
> зачем эти понятия вообще вводить? лично мне еще проще писать программы, не держа ничего в голове а тем более бессмысленного
> 
> >для пользователя языка это будет выглядеть, как будто они всегда передаются по значению
> 
> оно выглядит ни так и ни так, тк невозможно сформулировать как бы оно выглядело, если бы выглядело иначе (привет виттгенштейн) - снова смотрим ссылочную прозрачность.
> 
> зачем вообще что-то в голове держать? 
> поймите правильно, я не против если вы это держите и вам это помогает лучше кодить. у каждого свои ментальные "хелперы". просто когда эту бессмыслицу преподают и спрашивают на собесах выдавая за что-то осмысленное это уже другой расклад.
> 
> в моем родном шарпе есть такая штука как "value семантика". и там разница видна. например.
> 
> struct S {string Name};
> 
> void Test(S s) { s.Name = "tt";}
> S b = new {Name = "gg"};
> Test(b);
> Console.Write(b.Name);
> // увидим таки gg
> так как value семантика подразумевает копирование. в жаргоне тоже называют "передача по значению" и само значение мутабельное. в js насколько знаю такого нет и никто ни разу не показал как посмотреть что там  имеют ввиду под "передачей по значению".
> в с# числа это иммутабельные структуры, а строки - иммутабельный обьект(передается по ссылке). и разницы в семантике по изменениям не увидишь. можно было бы увидеть при ==, но у строк он переопределен и тоже не увидишь
> 
> у мурыча кмк есть свой брейнлаг сишника когда дело доходит до передачи по ссылке.
> я тут свою токсичную душноту вчера писал если интересно https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugx2HebPnBfRIvnEoth4AaABAg.9xdGHehP5Sk9yWokbUbsV-

> **[@sergey8366](https://www.youtube.com/channel/UC40kzB1rA5ELLzg98FI37Qw)** *[20.12.2023 22:39](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxRBwxdOzldBFhXyVh4AaABAg.9yWXkw8ZqXt9yZOMw6aGsn) (ред. 13.06.2024 22:18)*

> @WewasKangs-bd9eb еще минутка духоты перед сном
> на деле разработчики рантайма вполне могут числа копировать на стек (и вероятно так и делают где могу ибо нах лишний переход по указателю за данными, которые помещаются в машинное слово и регистр). и строки могут копировать,  если дебилы. но с точки зрения семантики языка из-за иммутабельности разницы не увидеть. а жор памяти и тайминги спека языка не регламентирует.

> **[@WewasKangs-bd9eb](https://www.youtube.com/channel/UCYLIpcmQ6QoFk2KWGx1BLrg)** *[20.12.2023 22:56](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxRBwxdOzldBFhXyVh4AaABAg.9yWXkw8ZqXt9yZQJT_uqAN) (ред. 13.06.2024 22:18)*

> @sergey8366 с чего вы взяли, что я чего-то хочу?
> Я всего-лишь пытаюсь сказать, что совершенно нет причины забивать голову спеками, а нужно всего-лишь запомнить какие переданные параметры могут быть изменены внутри функции (какие мутабельны, а какие нет). Куча вопросов по этой теме в чате показывает, что народ только путается больше после этого группового чтения спека.
> Есть языки вроде ПХП или С# где условные "примитивы" можно передавать как по значению, так и по референсу. А в JS - нет. Там все по референсу, только примитивы  имутабельны и поэтому для юзера во всех смыслах этого слова они работают как переданные по значению.

---

**[@fredengls](https://www.youtube.com/channel/UC2NlWbz5xhD_NQ_TgEdB2ag)** *[20.12.2023 20:03](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzJngBM3ICUkeoahCF4AaABAg) · 👍 1*

https://youtu.be/LyQzyrZRNXs?t=3328 хороший пример, того что грамотный человек замкнувшись в собственных мыслях начинает нести чушь. У типов данных действительно есть value и reference семантика. То что Murych этого не понимает является проблемами Murych-а. Стример  не слышал и/или не понимает как работает copy-on-write в современных ЯП. Что позволяет оптимизировать выделение паямяти при копирование объектов с типами данных с value семантикой. Это много говорит о кругозоре данного гражданина.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[22.12.2023 12:33](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzJngBM3ICUkeoahCF4AaABAg.9yZ6Y0w1Nqj9ycScNmZBf5)*

> Конечно мурыч не понимает. Кто он вообще такой чтобы понимать это.
> 
> А Еще оказывается в V8 есть маркер Cope On Write. 
> А вы о нем не знаете.  Потому, что иначе бы показали бы Вы его.
> 
> Но кто я такой чтобы мешать Вам хаять Мурыча?
> Я думаю от Вашего, необоснованного хая, все равно одна польза.

---

**[@fredengls](https://www.youtube.com/channel/UC2NlWbz5xhD_NQ_TgEdB2ag)** *[20.12.2023 20:15](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxUn-b6f_dTiVl_nuF4AaABAg)*

Оптимизация [через кеширование] строк, была реализована в Java еще в 2000-х годах. А теперь, внимание, секрет того как подавляющем большинстве языков программирования реализованы строки с использованием value семантики: 
- на стеке выделяется область фиксированного объема под структуру данных
- в данной структуре данных есть уникальный идентификатор и ссылка на область памяти в куче где хранится строка
- далее при копировании исходной структуры данных создается новая структура с новым идентификатором и со ссылкой на первоначальный объект в куче. 
- Опционально. Можно обойтись без идентификатора, в языках с подсчетом ссылок. Там объект при изменение будет проверять счетчик ссылок "строки" в куче. Если refCount > 1, то при изменении структура на стеке заведет новый объект в куче.
- При изменении объект на стеке сравнит свой идентификатор и тот что в куче. Если совпадают - изменит in-place. Если не совпадает, то структура на стеке заведет новый объект в куче.

Все. Я не знаю JS. Но я знаю что стример несет чушь. И ссылки на спецификацию с последующим флудом этого не меняют

---

**[@fredengls](https://www.youtube.com/channel/UC2NlWbz5xhD_NQ_TgEdB2ag)** *[20.12.2023 20:30](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwV7IjvvYsnTaiRx8R4AaABAg)*

01:31:43 - есть ли в спецификации что-нибудь о передаче по "ссылке" и/или о ссылочном типе данных?
Нет, этого нет. А почему? Потому что спецификация носит абстрактный характер и не несет в себе целью диктовать детали реализации разработчикам среды исполнения JS. Значит ли это что разработчики V8 и пр. отказались от value и reference семантики? Нет, не значит. Это важные детали реализации которые необходимо знать разработчику и учитывать при написании кода. Странно что человек мнящий себя специалистом в разработке, не понимает разницы между абстракцией и реализацией.

P.S.: от данной ахинеи у меня подгорело очень сильно.

---

**[@grip1720](https://www.youtube.com/channel/UCFIvyqQC5ByturccHLJUXOQ)** *[22.12.2023 09:46](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwOIcNEF5EVjLhf1Fp4AaABAg)*

Шик! Спасибо!

---

**[@vdbxxx](https://www.youtube.com/channel/UClsjzAwVoVWWQEpnJE8pDJg)** *[23.12.2023 11:29](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugxy9gjd9-XJsQ8wuhF4AaABAg)*

Если в спецификации что-то придумано для упрощения понимания, а в реальности никто не может понять отличие выдумки от реальности, когда во всём мире есть только один человек, который это "упрощение" понял, что оно - упрощение, то... имеет ли право на жизнь такое "упрощение"? Много лет назад, когда я впервые увидел синтаксис и работу джаваскрипта, я сразу подумал, что такое могли создать только люди, у которых очень большие тараканы в голове.

---

**[@AlexeyPack](https://www.youtube.com/channel/UChNb-mCtzhLbDCt9yVsvoGg)** *[05.01.2024 19:52](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxzfPrViLNI3qBanH94AaABAg)*

бесит когда говорят - объект передают по ссылке. Люди даже не знают что такое передача по ссылке.
хотя происходит присвоение (копирование) идентификатора обьекта.
Передача по ссылке это значит две переменные ссылаются на одно и тоже значение (адрес в памяти)

> **[@radunov.a](https://www.youtube.com/channel/UCrIj6egUVWwFSME9V_6gc1A)** *[07.01.2024 19:09](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxzfPrViLNI3qBanH94AaABAg.9zCI0wboxiK9zHMecYHlxm) · 👍 1*

> А что бесит то? С точки зрения осмысления прочитанного так и есть. Ты передаёшь ссылку на объект. Да, формально это ссылка на область памяти, но упрощенно это ссылка на объект. Ты имеешь как бы ярлык, поменяй что-то в ярлыке поменяется везде

---

**[@AlexeyPack](https://www.youtube.com/channel/UChNb-mCtzhLbDCt9yVsvoGg)** *[05.01.2024 20:03](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxTcCk_z9QMYaXZJtp4AaABAg) (ред. 05.01.2024 20:06) · 👍 2*

по по поводу эксперимента.
Если происходит присвоение, то они ссылаются на одно и тоже значение(адрес в памяти). Если хоть какая то переменная изменить, то произойдет сначало копирование значение в памяти и потом его изменение.
Если мы сделаем это в функции то после завершения функции память лишняя освободится.

> **[@AlexanderBorshak](https://www.youtube.com/channel/UCcY6GQl77kuMf2BjIB-HjhQ)** *[08.01.2024 12:59](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxTcCk_z9QMYaXZJtp4AaABAg.9zCJDFRzOOr9zJH5spoJEr) · 👍 1*

> +1. Copy On Write

---

**[@AlexeyPack](https://www.youtube.com/channel/UChNb-mCtzhLbDCt9yVsvoGg)** *[05.01.2024 20:16](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgydWj0ZxjzkL6Dm3Wp4AaABAg) · 👍 1*

по поводу примитивов - это теже обьекты которую хранят в себе значение на низком уровне, но являются не изменяемыми.

---

**[@radunov.a](https://www.youtube.com/channel/UCrIj6egUVWwFSME9V_6gc1A)** *[07.01.2024 18:25](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxWoFAPJ2MU4Cvyu3F4AaABAg) (ред. 07.01.2024 18:30) · 👍 2*

Автор просто называет то же поведение другими словами и делает из этого открытие. Да, по первому пункту «копирование значения» - отличается от сказанного лектором. По второму «копирование по ссылке» сказал ровно то же самое заменив слово «ссылка» на слово «значение идентификатора в оперативной памяти». Если я не прав, извините. Я вижу это так, может позже  поумнее и пойму идею.

> **[@AlexanderBorshak](https://www.youtube.com/channel/UCcY6GQl77kuMf2BjIB-HjhQ)** *[08.01.2024 13:39](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxWoFAPJ2MU4Cvyu3F4AaABAg.9zHHarkdSTw9zJLihaMLCi) (ред. 08.01.2024 13:40) · 👍 2*

> Да все так. Автор видео просто максималист, придирается к словам, игнориует широко распространенную технику оптимизации Copy-On-Write, а в тестовой функции тестирует непонятно что (вместо модификации переданного в функцию объекта непонятно зачем создает новый из литерала). В общем, программирует на одном уровне абстракции учитывая при этом детали реализации на один или даже два уровня ниже (то есть, программирует на JS, но постоянно держит в голове движок JS или даже сам процессор).

---

**[@AlexanderBorshak](https://www.youtube.com/channel/UCcY6GQl77kuMf2BjIB-HjhQ)** *[08.01.2024 12:08](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyFZp5t_0kZ-v84lcF4AaABAg)*

Было бы намного лучше записать обычное видео длиной в 5-10-15 минут, где конденсированно раскрыть проблему. Смотреть видео на 3 часа - ну, такое... :(

---

**[@AlexanderBorshak](https://www.youtube.com/channel/UCcY6GQl77kuMf2BjIB-HjhQ)** *[08.01.2024 12:55](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugyy1v9jhtKWtc4ChhN4AaABAg) · 👍 2*

Совершенно непонятно, почему вас так бомбит? Вы же профи, а профи не должны бомбить. Ну и по сути. Вам знакома концепция Copy-On-Write? Персистентные структуры данных? Если у нас есть строка s1 = "1xx...xxx", которая занимает N мегабайт, то при создании нового значения, типа const s2 = s1; движок JS вполне себе вправе создать [умный] указатель на то же самое значение в памяти. Но как только мы напишем const s3 = s1.replace("1", "2"), движку придется создать копию - так как изначальный слепок данных не подходит одновременно и для s1 и для s3, и необходимо внести изменения. Вполне себе в рамках Copy-On-Write. И до сих пор - в рамках концепции "примитивных" (скалярных) типов [данных]. Кстати, движок может действовать и более хитрым способом - к примеру, хранить только измененные части, то есть прямо как в персистентных структурах данных. 

Только вот зачем _прикладному программисту на JS_ заботится о таких нюансах? Ведь сам JS как раз и есть абстракция над низкоуровневым вычислителем, и создана данная абстракция как раз для того, ЧТОБЫ ТАКИЕ НЮАНСЫ СКРЫВАТЬ. В противном случае лучше сразу взять C/C++ или Rust, и писать низкоуровневый код - или даже сразу на Асме, непосредственно в терминах [аппаратного] вычислителя. Так что с точки _прикладного программиста на JS_ все выглядит именно так - есть примитивные типы, есть ссылочные. 

И проверяется это как два байта написать - создаем 2 функции, что модифицируют исходный аргумент - одна модифицирует и возвращает примитивный тип [данных], вторая - ссылочный. Вызываем первую на числе или строке, вторую на массиве или объекте; а затем проверяем значение начального аргумента и возвращенного функцией. В случае с примитивным типом [данных] мы получим 2 разных значения, в случае ссылочных - одно и то же значение. Что и подтвердит нам нашу теорию, или интуицию, или как там еще назвать.

Конечно, с точки зрения движка JS все может быть по другому. Но прикладному программисту какая разница? Теория/интуиция позволяет писать код в абсолютном большинстве случаев. А то, что спецификация не оперирует такими терминами - ну а она должна? Наоборот, отсутвие [жестких] требований к реализации в спецификации позволяет проводить любые оптимизации на уровне движка, до тех пор, пока удовлетворяется ВНЕШНЕЕ ПОВЕДЕНИЕ, определенное спецификацией.

---

**[@AlexanderBorshak](https://www.youtube.com/channel/UCcY6GQl77kuMf2BjIB-HjhQ)** *[08.01.2024 13:17](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyGb4wYgr1robxhAwJ4AaABAg) (ред. 08.01.2024 13:17) · 👍 1*

На 1:20:59 вы внутри функции не модифицировали значение переданного внутрь функции объекта, а создали абсолютно новый через литерал (который будет отброшен после окончания работы функции и [когда-то] зачищен сборщиком мусора). Совершенно непонятно, что вы хотите этим доказать. Вполне возможно, что у вас высочайшая квалификация, но явно видно, что вы тяготеете к т.н. "микрооптимизации", то есть учету всех деталей более низко лежащих абстракций при написании кода на более высоком уровне абстракции. То есть - пишем на JS, но учитываем, как работает движок (а какой именно V8? или Rhino? или что-то другое), и даже процессора (а какой именно? x86? или AMD? или RISC-V?). Иногда такой подход может быть оправдан - но только в очень ограниченном круге (под)задач, когда требуется максимум производительности по времени или по памяти. Но в общем случае - он скорее вреден, так как язык программирования - в данном случае JS, в общем случае - любой другой - как раз создан для того, чтобы скрыть от прикладного программиста все низкоуровневые детали, и позволить ему сконцентрироваться на более высоком уровне абстракции, то есть ПРОГРАММИРОВАТЬ В ТЕРМИНАХ ЗАДАЧИ, а не движка или процессора. Возможно, для ваших задач лучше просто использовать чистый С.

---

**[@EABabenko](https://www.youtube.com/channel/UCwVXZSS_eJrb8W9f03Egdww)** *[11.01.2024 11:11](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyKQDLokYnTiPPMTc14AaABAg)*

Не согласен с автором, что данные не передаються по ссилке. Для  примера: 
{
    let str = "ghjgjhjghjghjghjghj";
    let num = 5;
    let obj = {
        str: "name obj",
        num: 10,
    };

    console.log("str: ", str);
    console.log("num: ", num);
    console.log("obj: ", obj);

    myFunc(str, num, obj);

    console.log("str: ", str);
    console.log("num: ", num);
    console.log("obj: ", obj);

    function myFunc(funcStr, funcNum, funcObj) {
        console.log('In function');
        console.log("str: ", str);
        console.log("num: ", num);
        console.log("obj: ", obj);
        console.log("funcStr: ", funcStr);
        console.log("funcNum: ", funcNum);
        console.log("funcObj: ", funcObj);
        
        funcStr = "dsfdsfds";
        funcNum = 3;
        funcObj.str = "modify name object";
        funcObj.num = 20;
        
        console.log("str: ", str);
        console.log("num: ", num);
        console.log("obj: ", obj);
        console.log("funcStr: ", funcStr);
        console.log("funcNum: ", funcNum);
        console.log("funcObj: ", funcObj);
    }
}

---

**[@СергейПанасюк-и3ф](https://www.youtube.com/channel/UCV7VaeE6BAGbd0YN6uOEV8A)** *[12.01.2024 20:38](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugyt3BIGJfxnK1QYcqd4AaABAg) · 👍 1*

Посоветуйте книгу для изучения JavaScript с детьми.

> **[@computercomputer3293](https://www.youtube.com/channel/UCMwqst-QsNwF-WWrdwhpdTw)** *[13.11.2025 19:21](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugyt3BIGJfxnK1QYcqd4AaABAg.9zUOqqiXVY8APU1My82ZxN)*

> Не помню автора, но помню название, так и называется, JavaScript для детей

---

**[@КириллЛимонов-з7в](https://www.youtube.com/channel/UCOpvGxRBlnG2zKUIs3iVvqA)** *[16.01.2024 20:33](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwQSVffaKz_k4KlaLt4AaABAg) (ред. 16.01.2024 22:26)*

Добрый день!
Помогите разобраться, пожалуйста!
на 1:59:30 вы говорите что GetValue это получение primitive value, а PutValue это помещение ссылки или primitive value.
Далее вы говорите что rval как бы становится эквивалентным ссылкой на primitive value.
Я решил посмотреть в спецификации как реализуется этот абстрактный метод GetValue:

 1. ReturnIfAbrupt(V).
 2. If V is not a Reference Record, return V.
 3. If IsUnresolvableReference(V) is true, throw a ReferenceError exception.
 4. If IsPropertyReference(V) is true, then
   a. Let baseObj be ? ToObject(V.[[Base]]).
   b. If IsPrivateReference(V) is true, then
     i. Return ? PrivateGet(baseObj, V.[[ReferencedName]]).
   c. Return ? baseObj.[[Get]](V.[[ReferencedName]], GetThisValue(V)).
 5. Else,
   a. Let base be V.[[Base]].
   b. Assert: base is an Environment Record.
   c. Return ? base.GetBindingValue(V.[[ReferencedName]], V.[[Strict]]) (see 9.1).

насколько я понял при таком присваивании:
var a = '123'
По пункту 2, V не является Reference Record, поэтому нам вернется '123', которое будет являться primitive value.
В то же время в момент присваивания создастся Reference Record на 'a', которая будет иметь [[Base]] глобальный объект, [[ReferencedName]] 'a',
[[Strict]] допустим у нас false, и [[ThisValue]] на этом этапе пока что пустое.
Далее выполняется абстрактная операция PutValue(lref,rval)

Я так же посмотрел его реализацию:

 1. ReturnIfAbrupt(V).
 2. ReturnIfAbrupt(W).
 3. If V is not a Reference Record, throw a ReferenceError exception.
 4. If IsUnresolvableReference(V) is true, then
   a. If V.[[Strict]] is true, throw a ReferenceError exception.
   b. Let globalObj be GetGlobalObject().
   c. Perform ? Set(globalObj, V.[[ReferencedName]], W, false).
   d. Return unused.
 5. If IsPropertyReference(V) is true, then
   a. Let baseObj be ? ToObject(V.[[Base]]).
   b. If IsPrivateReference(V) is true, then
     i. Return ? PrivateSet(baseObj, V.[[ReferencedName]], W).
   c. Let succeeded be ? baseObj.[[Set]](V.[[ReferencedName]], W, GetThisValue(V)).
   d. If succeeded is false and V.[[Strict]] is true, throw a TypeError exception.
   e. Return unused.
 6. Else,
   a. Let base be V.[[Base]].
   b. Assert: base is an Environment Record.
   c. Return ? base.SetMutableBinding(V.[[ReferencedName]], W, V.[[Strict]]) (see 9.1).

Как я понимаю мы проваливаемся в 6 пункт поскольку
'a' это Reference Record, а IsPropertyReference(V) вернет false из-за пункта 2 ниже (V.[[Base]] Это глобальный объект
а значит Environment Record)
1. If V.[[Base]] is unresolvable, return false.
2. If V.[[Base]] is an Environment Record, return false; otherwise return true.

base в таком случае будет являться глобальным объектом.
Попадаем в выражение base.SetMutableBinding(V.[[ReferencedName]], W, V.[[Strict]]).

SetMutableBinding выполняет два метода:
CreateMutableBinding и InitializeBinding.
Первый создает новую изменяемую привязку для имени V.[[ReferencedName]]. 
Привязка не должна существовать в этой записи среды для V.[[ReferencedName]].
InitializeBinding он используется для установки привязанного значения текущей привязки
идентификатора, имя которого является значением аргумента V.[[ReferencedName]], к значению аргумента W.
Но тут я натыкаюсь на странную штуку, если третий параметр в SetMutableValue будет true, то

 a. If S is true, throw a ReferenceError exception. (взято из спецификации)
Я понимаю так, что если мы будем пытаться выполнить var a = '123' в 'use strict', то
будет ReferenceError exception, чего на деле не происходит.

Помогите разобраться в этом механизме правильно, что я не так понимаю?
И как выполняется реализация этих абстрактных методов в действительности, одинаковая ли она для всех движков?

---

**[@TahirDibirovII-uz5ll](https://www.youtube.com/channel/UCnqZc261N2UbEW5dGxKDujQ)** *[23.01.2024 08:15](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgycbZm2SaZGZmyF7Xx4AaABAg)*

Своего время подобных тупых заявлений и противоречий я часто встречал в учебниках по химии и по физике

---

**[@johngalt9494](https://www.youtube.com/channel/UCULcuPJ1SALjUpSli2PMNyA)** *[09.03.2024 16:38](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugw-zmWCDZbdBFWT0Bx4AaABAg) · 👍 1*

Комментарий в поддержку деятельности автора и продвижения канала !

---

**[@Гооол-й4ч](https://www.youtube.com/channel/UCI_uKeDGw-qUumxR37GgSLA)** *[13.03.2024 17:58](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwB5sVUhbTltfC6fO54AaABAg) · 👍 2*

Если при обращение в глобальном окружение к какому-либо идентификатору мы как бы обращаемся к глобальному объекту по ключу = имени этого идентификатора, то почему написав window.qwe мы получаем ожидаемый undefined, а написав qwe - ReferenceError?

Как объяснить поведение при котором {} === {} возвращает false, но 5 === 5 возвращает true? В рамках мейнстрима, где теория про ссылочные и примитивные типа живее всех живых это легко объясняется тем, что объект - ссылка, а 5 - значение, ссылки всегда разные, если не было прямого присваивания, значения тут очевидно идентичны. Я конечно же попытался найти ответ на своё вопрос в спеке и понял, что у меня нет не единого шанса понять, о чём там идёт речь.

> **[@Гооол-й4ч](https://www.youtube.com/channel/UCI_uKeDGw-qUumxR37GgSLA)** *[23.03.2024 10:25](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwB5sVUhbTltfC6fO54AaABAg.A0wB37Fkd3mA1K78vcyx--) (ред. 28.11.2024 00:55) · 👍 1*

> ​@user-es9dx3lo7n , а как по-твоему определяется что {} и {} это разные объекты, если не по ссылке?

> **[@computercomputer3293](https://www.youtube.com/channel/UCMwqst-QsNwF-WWrdwhpdTw)** *[13.11.2025 19:40](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwB5sVUhbTltfC6fO54AaABAg.A0wB37Fkd3mAPU3bDx1FnD)*

> Я так себе это объясняю, при {} === {} ссылаются на разные ячейки в памяти, на разные адреса, так как последовательность адресов не совпадает, поэтому false. При 5 === 5, оба идентификатора ссылаются на одну ячейку в памяти, на один адрес, число адреса совпадает поэтому true.

> **[@Гооол-й4ч](https://www.youtube.com/channel/UCI_uKeDGw-qUumxR37GgSLA)** *[13.11.2025 20:14](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwB5sVUhbTltfC6fO54AaABAg.A0wB37Fkd3mAPU7VMydkzX)*

> @computercomputer3293 в целом мне тоже кажется что это так, но я не уверен. Ну то есть то, что примитивные значения существуют в единственном экземпляре, а объекты имеют так называемую 'identity' и являются уникальными это да, а вот как именно происходит сравнение не уверен, так и не нашёл в себе силы в этом досконально разобраться.

---

**[@Sergei546](https://www.youtube.com/channel/UCkIbOOnDXfE32PYAsMQs6Qg)** *[10.04.2024 16:01](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugz-U7TsHrc-JDWf0C14AaABAg)*

ваши видео супер полезные спасибо

---

**[@FrankBakulov](https://www.youtube.com/channel/UC73lSQURf81UCdJHJ884tJA)** *[13.05.2024 07:35](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzGhyBy6uhFU_awvJN4AaABAg) · 👍 1*

Спасибо большое! Из этого бы хайлайты смонтировать. Но и так фоном зашло отлично. Да уж, знатно я покраснел, ведь много раз и отвечал и спрашивал на собесах про примитивные и ссылочные типы данных... Но как говорится не страшно не знать, страшно не хотеть знать!

---

**[@marlenkaparov7735](https://www.youtube.com/channel/UCHPg788SMOxpRf2JtJago0g)** *[20.05.2024 04:43](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwZ_Ybw-Huiyi2hUzx4AaABAg)*

Там написано primitive value

---

**[@northwest569](https://www.youtube.com/channel/UCf3gBcrnYkbAXgsl6dZkVSA)** *[11.06.2024 13:12](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgwdZH0dKIfjU34v5PF4AaABAg)*

Хочу футболку с Мурычем 😂

---

**[@sjdjjsjsjs3991](https://www.youtube.com/channel/UCXGfhoqdgreVsVKIfbiJGbQ)** *[07.08.2024 05:36](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgzHsHmORfkTPm1shLt4AaABAg)*

Мурыч, берёшь менторство?

---

**[@ЕвгенийБондаренко-с5е](https://www.youtube.com/channel/UCUiOYFnALQWx2njrm8QLgMA)** *[29.08.2024 09:28](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgyLMXPOlTP9TbPY_c94AaABAg) · 👍 2*

нихренасе быстренько - 3 часа с лишним

---

**[@АлександрВидин-с6я](https://www.youtube.com/channel/UCEDy_EJsn0QxuJGGx9QnNbQ)** *[22.10.2024 18:46](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugw1aYSxIULIaz7e1NV4AaABAg) · 👍 1*

Спасибо

---

**[@hasst9261](https://www.youtube.com/channel/UCql4WyYU2-tI_k1KArhLvSQ)** *[02.02.2025 01:29](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxPYRIvXbfgkSNG5dt4AaABAg)*

Я дізнався нове для себе і повеселився)

---

**[@kodirovbaiaman6137](https://www.youtube.com/channel/UCnr-H0-a9PneOVBr4869iaA)** *[27.04.2025 12:41](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxvTKHT0HscZ6PQabh4AaABAg) · 👍 3*

Краткий пересказ 1.5 часа видео:

Объекты — мутабельные, а строки, числа и другие примитивы — нет.

При передаче переменных в функцию создаются новые указатели на те же области памяти, что и у оригинальных переменных (новые данные не копируются).

Поэтому если внутри функции присвоить, например, obj = null, оригинальный объект не изменится — меняется только локальный указатель.

Но если изменить свойства объекта, то они изменятся и у оригинала, потому что параметры и в func => obj и obj указывают на одни  и те же блоки памяти.

С примитивами так сделать нельзя, потому что они имутабельны — их нельзя изменить напрямую, только заменить новым значением.

и это реально важная информация, потому что зная как работает базовая логика переменных никакие объяснения с ссылочными не ссылочными типами будет не нужон.
(сразу говорю я дебил, тапками не бейте, понял как понял)

> **[@Yan-777-ua](https://www.youtube.com/channel/UCZVIgiY5PDPotHAfjElKXvw)** *[10.06.2025 04:22](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxvTKHT0HscZ6PQabh4AaABAg.AHQKgSORP1cAJAjUB2nhyd) · 👍 1*

> Зачем вообще это знать? Это поможет в разработке или просто полезно для прохождения собеса?

> **[@computercomputer3293](https://www.youtube.com/channel/UCMwqst-QsNwF-WWrdwhpdTw)** *[13.11.2025 19:15](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=UgxvTKHT0HscZ6PQabh4AaABAg.AHQKgSORP1cAPU0mHxgXuT)*

> Нет, это полезно тем кто хочет понимать как это на самом деле работает. Просто некотором более интересно не зубрить, а понимать, ковыряться внутри, как оно там м устроено и работает. Это лишь и вопрос интереса.

---

**[@立入禁止](https://www.youtube.com/channel/UC2FXt1XFZ0ecpGWe92jn_og)** *[28.10.2025 13:01](https://www.youtube.com/watch?v=LyQzyrZRNXs&lc=Ugyjq3T-bhsaZc8j_nZ4AaABAg) · 👍 1*

Можно бесконечно смотреть на огонь, воду и на то, как Мурыч залипает в спеке.

---
