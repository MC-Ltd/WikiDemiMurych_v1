---
title: "Производительность JavaScript Array в V8. ⎡perf:5⎦"
date: 2024-04-06
tags: []
videoId: "fWqOswHMjEo"
duration: "3:04:30"
views: 6127
likes: 241
comments: 29
---
# [Производительность JavaScript Array в V8. ⎡perf:5⎦](https://www.youtube.com/watch?v=fWqOswHMjEo)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 06.04.2024 12:11  
**Тривалість:** 3:04:30  
**Перегляди:** 6127 · **Лайки:** 241 · **Коментарі:** 29
![thumbnail](https://i.ytimg.com/vi/fWqOswHMjEo/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=fWqOswHMjEo)
## Таймкоди

- [00:00:00](https://www.youtube.com/watch?v=fWqOswHMjEo&t=0)   Музыка
- [00:02:39](https://www.youtube.com/watch?v=fWqOswHMjEo&t=159)   Мнение Тучи про Java и про Python
- [00:06:39](https://www.youtube.com/watch?v=fWqOswHMjEo&t=399)   Начало - проблематика
- [00:08:20](https://www.youtube.com/watch?v=fWqOswHMjEo&t=500)   PACKED и HOLEY
- [00:10:40](https://www.youtube.com/watch?v=fWqOswHMjEo&t=640)   SMI, DOUBLE,  ELEMENTS
- [00:21:45](https://www.youtube.com/watch?v=fWqOswHMjEo&t=1305)   Dictionary elements
- [00:27:20](https://www.youtube.com/watch?v=fWqOswHMjEo&t=1640)   Промежуточные итоги по вышесказанному
- [00:30:15](https://www.youtube.com/watch?v=fWqOswHMjEo&t=1815)   Что такое slot
- [00:31:05](https://www.youtube.com/watch?v=fWqOswHMjEo&t=1865)   Что происходит при увеличении длины Array
- [00:40:55](https://www.youtube.com/watch?v=fWqOswHMjEo&t=2455)   Что происходит при уменьшении длины Array
- [00:48:05](https://www.youtube.com/watch?v=fWqOswHMjEo&t=2885)   Особенности поведения методов Array в плоскости Slots
- [00:52:05](https://www.youtube.com/watch?v=fWqOswHMjEo&t=3125)   Вопрос о том что быстрее push или fill
- [00:54:00](https://www.youtube.com/watch?v=fWqOswHMjEo&t=3240)   Пример поведения Array при уменьшении его длины
- [00:56:20](https://www.youtube.com/watch?v=fWqOswHMjEo&t=3380)   Что такое COW у Array или Copy on write
- [01:04:55](https://www.youtube.com/watch?v=fWqOswHMjEo&t=3895)   Почему Array типа SMI значительно быстрее чем Array из ELEMENTS
- [01:17:40](https://www.youtube.com/watch?v=fWqOswHMjEo&t=4660)   Гипотеза о том, что переход к  Dictionary требует непрерывного числа hole
- [01:29:50](https://www.youtube.com/watch?v=fWqOswHMjEo&t=5390)   Резюме вышесказанного
- [01:34:10](https://www.youtube.com/watch?v=fWqOswHMjEo&t=5650)   Вопросы/ответы
## Коментарі (14 · відповідей: 15)

**[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[05.04.2024 22:49](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=UgwaniwhHyZNIlBBWdt4AaABAg) · 👍 1*

00:00:00   Музыка
00:02:39   Мнение Тучи про Java и про Python
00:06:39   Начало - проблематика
00:08:20   PACKED и HOLEY
00:10:40   SMI, DOUBLE,  ELEMENTS
00:21:45   Dictionary elements
00:27:20   Промежуточные итоги по вышесказанному
00:30:15   Что такое slot
00:31:05   Что происходит при увеличении длины Array
00:40:55   Что происходит при уменьшении длины Array
00:48:05   Особенности поведения методов Array в плоскости Slots 
00:52:05   Вопрос о том что быстрее push или fill
00:54:00   Пример поведения Array при уменьшении его длины
00:56:20   Что такое COW у Array или Copy on write
01:04:55   Почему Array типа SMI значительно быстрее чем Array из ELEMENTS
01:17:40   Гипотеза о том, что переход к  Dictionary требует непрерывного числа hole
01:29:50   Резюме вышесказанного
01:34:10   Вопросы/ответы

---

**[@JivuvkitaeRu](https://www.youtube.com/channel/UCYQ-LcHK8Td8XwzCVrXv7TA)** *[05.04.2024 23:07](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=UgwKtjlk0K5HI2wGTHx4AaABAg)*

Туча про питон все верно подметил

---

**[@maksym7094](https://www.youtube.com/channel/UCVWtzv69C2a--CEozyxNhTA)** *[06.04.2024 09:08](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugx-mYisyqSzfeUoL714AaABAg)*

ті Тучу только берешь на руки, как он сразу відает про джаву и питон

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[06.04.2024 17:09](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugx-mYisyqSzfeUoL714AaABAg.A1t1OQXqUvgA1ttUCIvbNv)*

> Так это я его уже затилилинькал этими вопросами.

---

**[@Andrew-NaN](https://www.youtube.com/channel/UCvEyMg75ev6ICAbl2yxUBpg)** *[06.04.2024 09:45](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=UgzwsQ6YYOQngqzic1t4AaABAg) (ред. 06.04.2024 11:07) · 👍 3*

Давай побольше стримов в дуэте с Vondarm! Грамотные вопросы помогают раскрыть тему

---

**[@crutchmaster9637](https://www.youtube.com/channel/UCkdub5pSPh3B2q_TtpJidgQ)** *[06.04.2024 11:27](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=UgwsbP-B75V2GY-v1vN4AaABAg) · 👍 1*

А как создать массив на много элементов, чтобы он не копировался туда-сюда?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[06.04.2024 17:09](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=UgwsbP-B75V2GY-v1vN4AaABAg.A1tHJBHXxyAA1ttQjESTJD) · 👍 2*

> Использовать Typed Array. В случае Exotic Object Array - изменить это поведение в V8 сейчас невозможно. 
> 
> Отчасти этого можно избежать, если заранее знать обьем тех данных которые будут push-иться и pop-аться. Тогда можно искусственно расчитать capacity и под эти данные создать Array.

---

**[@Sergei546](https://www.youtube.com/channel/UCkIbOOnDXfE32PYAsMQs6Qg)** *[06.04.2024 12:49](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=UgyAbi8DkNQzYBKO_jJ4AaABAg)*

урааа любмый  канал выпустил видео спасибо

---

**[@khanchobai9748](https://www.youtube.com/channel/UCUnlaOBR1xDvxKE2TJ6-niA)** *[06.04.2024 22:21](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=UgwWs0ltdIAmBboZM0J4AaABAg)*

очень интересно, спасибо за видео !

---

**[@ScioNescio-b5l](https://www.youtube.com/channel/UCXxjLSpZtk3IEQ1VsAR84Cw)** *[08.04.2024 07:18](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugz6nnBJW1KkkJgGyNB4AaABAg)*

Объясните пожалуйста

Эту задачу из сквза
const isTrue = true == [];
const isFalse = true == ![];

console.log(isTrue + isFalse);

в их хелпе написано:

Let's break this up:
The comparison performed is the abstract comparison operation,
which uses type coercion under the hood, when necessary.

As the first parameter is a boolean, the following rule applies:
"If Type(x) is Boolean, return the result of the comparison ToNumber(x) == y."
And in the next round, the next rule applies,
"If Type(y) is Boolean, return the result of the comparison x == ToNumber(y)."

Which then boils down to:
Number(true) == Number([])
=> 1 == 0

Но почему 

"If Type(y) is Boolean, return the result of the comparison x == ToNumber(y)." ?
не понимаю почему Type(y) is Boolean, Y же = [] ?

> **[@vondarm](https://www.youtube.com/channel/UCg9zRBMgyrL4czuUWCyITpg)** *[08.04.2024 11:01](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugz6nnBJW1KkkJgGyNB4AaABAg.A1xzRB5fOGrA1yNx3-YGN_) (ред. 08.04.2024 11:01) · 👍 1*

> Прошлый мой коммент куда то пропал)
> повторю - согласно спецификации для true == [] происходят следующие шаги в рамках виртуальной функции IsLoosyEqual(x, y)
> 
> грубо обозначим вот такой вызов IsLoosyEqual(true, [])
> 
> 1) If x is a Boolean, return ! IsLooselyEqual(! ToNumber(x), y)
> ToNumber(true) дает 1
> 
> рекурсивно перевызываемся
> грубо говоря IsLoosyEqual(1, [])
> 
> 2) If x is either a String, a Number, a BigInt, or a Symbol and y is an Object, return ! IsLooselyEqual(x, ? ToPrimitive(y))
> ToPrimitive для массива в обычных условиях вызывает метод toString, который  для пустого массива (опять же в обычных условиях) возвращает пустую строку
> 
> рекурсивно перевызываемся
> грубо говоря IsLoosyEqual(1, "")
> 
> 3) If x is a Number and y is a String, return ! IsLooselyEqual(x, ! ToNumber(y))
> ToNumber для пустой строки даст 0
> 
> рекурсивно перевызываемся
> грубо говоря IsLoosyEqual(1, 0)
> 
> 4) If Type(x) is Type(y), then Return IsStrictlyEqual(x, y)
> дальше думаю очевидно

> **[@vondarm](https://www.youtube.com/channel/UCg9zRBMgyrL4czuUWCyITpg)** *[08.04.2024 11:06](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugz6nnBJW1KkkJgGyNB4AaABAg.A1xzRB5fOGrA1yOZKqFxB0)*

> "обычные условия", которые я упоминал - это важнейший пункт. Потому что хакнуть это стандартное поведение гигансткое множество способов - хотя бы подменить в прототипе valueOf, Symbol.toPrimitive или toString - и все - (true == []) будет истинно
> 
> именно поэтому то упрощение (пропуск шагов и сразу якобы выполнется ToNumber для пустого массива) которое допущено в ихнем описании - грубейшая ошибка

> **[@vondarm](https://www.youtube.com/channel/UCg9zRBMgyrL4czuUWCyITpg)** *[08.04.2024 11:51](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugz6nnBJW1KkkJgGyNB4AaABAg.A1xzRB5fOGrA1yTeLLkZ_0)*

> ! здесь не означает отрицание - в спецификации этот символ используется совсем для других целей - в данном случае "можно" его игнорировать

> **[@ScioNescio-b5l](https://www.youtube.com/channel/UCXxjLSpZtk3IEQ1VsAR84Cw)** *[08.04.2024 13:05](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugz6nnBJW1KkkJgGyNB4AaABAg.A1xzRB5fOGrA1yb8zh7Qh-)*

> @vondarm Благодарю! понял.

> **[@Гооол-й4ч](https://www.youtube.com/channel/UCI_uKeDGw-qUumxR37GgSLA)** *[08.04.2024 13:08](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugz6nnBJW1KkkJgGyNB4AaABAg.A1xzRB5fOGrA1ybTY4wkoV)*

> ​@vondarm, не подскажешь, как в принципе работает сравнение с объектами? Мол почему {} !== {} или [] !== [] отдаст нам true? 
> Просто не совсем понимаю, как определяется, что [] и [] - 2 разные сущности. Вроде понятно, что это 2 разных ссылки на разные места в памяти, но почему тогда 5 === 5 нам отдаст true? Мол в куче для каждого объекта хранится отедельный экземпляр, а для primitive value логика такова, что в куче только одна пятёрка? Я вот через память в хром тулах чекал, вроде там это так, мол создание в коде, например, отдельно новой строки, которая дублирует уже существующую, не приведёт к появлению новой строки в хипе, но является ли это базовым поведением js, или это просто проделки браузера. Ну а если всё что я выше написал - сущий бред, то я был бы рад просто услышать какое-то обяснения поведения объектов при сравнении. Потому что ранее для меня всё объяснялось мейнстримной байкой про ссылочные и примитивные типы, а потеряв веру в неё как-то и ответы пропали на некоторые вопросы, в том числе на текущий.​

> **[@vondarm](https://www.youtube.com/channel/UCg9zRBMgyrL4czuUWCyITpg)** *[08.04.2024 13:42](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugz6nnBJW1KkkJgGyNB4AaABAg.A1xzRB5fOGrA1yfNP3oKCc)*

> @Гооол-й4ч Здесь дело скорее не в том как они хранятся в памяти. Это как раз может быть вариативно в зависимости от оптимизаций.
> 
> если чекнуть спецификацию экма, а именно функцию IsStrictlyEqual, и далее погулять по ссылкам, то можно найти:
> 1) отдельные правила для сравнения null, undefined, string, BigInt, boolean и частично number описанные прямо в спецификации
> 2) выражение If x is y, return true; otherwise, return false. И пояснение что прочие значения сравниваются согласно их identity
> 
> Далее можно найти параграф Identity, который и поясняет что значит это is
> 
> там написано что то вроде "значения в js бывают с identity и без. Значения без identity (undefined, null, Booleans, Strings, Numbers, and BigInts) сравниваются по их внутренним характеристикам (number по его численному значению например), а значения с identity (Objects) всегда уникальны и равны только себе"
> 
> Это вольный пересказ с сокращениями и упрощениями, так то там сложнее - есть нюансы с number, Symbol да и c самим понятием identity

> **[@Гооол-й4ч](https://www.youtube.com/channel/UCI_uKeDGw-qUumxR37GgSLA)** *[08.04.2024 14:20](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugz6nnBJW1KkkJgGyNB4AaABAg.A1xzRB5fOGrA1yjg41cOdL) (ред. 08.04.2024 14:21)*

> ​@vondarm , благодарю, я в своё время читал и на identity натыкался, просто подобная информация будто бы ничего не объясняет. Мол, почему у нас объект равен лишь самому себе? Ну потому что у нас язык написан так, что объект равен лишь самому себе, а называем мы это поведение таким-то словом. Понятно, что, наверное, при детальном анализе можно найти какие-то более основательные ответы, но, как говориться, если б я был способен нормально читать спецификацию...
>   Мол если подумать всё так или иначе  упирается в вопрос, а как мы понимаем, что 5 и 5 это одно и то же, а {} и {} - нет?
> То есть допустим у {} есть identity и {} !== {}, но сравнивая эти структуры как-то должна определяться их уникальность.  Сравнение по ссылкам, которые у них разные, это единственное здравое предположение, которое я могу сгенерировать на основании своих знаний. А то что Number сравниваются по их числовому значению, ну эти значения ведь так или иначе хранится где-то в памяти и мы просто на них ссылаемся, поэтому я предположил, что вероятно у чисел нет дубликатов в хипе, поэтому все сравнения не объектов ( +символов) одинаковой структуры приводят к сравнению, где по обе стороны одна и та же ссылка, на одну и ту же область памяти.

> **[@vondarm](https://www.youtube.com/channel/UCg9zRBMgyrL4czuUWCyITpg)** *[08.04.2024 14:40](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugz6nnBJW1KkkJgGyNB4AaABAg.A1xzRB5fOGrA1ylyEav4BG)*

> ​@Гооол-й4ч
> 
> Физическим представлением identity объектов на уровне реализации является скорее всего действительно ссылка
> 
> В то время как числа в v8 как раз точно могут дублироваться.
> 
> А вот строки насколько я знаю не дублируются, поэтому их тоже можно сравнить по ссылке, однако identity у них нету. Поэтому можно сделать Рантайм, в котором они будут дублироваться, и это не будет противоречить спецификации.
> 
> Это вообще как тёплое с мягким. Ты можешь написать Рантайм в котором всё дублируется, а можнешь в котором ничего не дублируется. Главное соблюдать внешнее поведение, соответсвующее виртуальной машине ecma. 
> 
> Однако в любой из этих реализаций сравнения должны работать одинаково. Независимо от расположения и совпадения в памяти
> 
> Единственное что, не совсем ясно, как сделать дублирующийся объект с одной идентичностью, без противоречий спеке

> **[@vondarm](https://www.youtube.com/channel/UCg9zRBMgyrL4czuUWCyITpg)** *[08.04.2024 14:47](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugz6nnBJW1KkkJgGyNB4AaABAg.A1xzRB5fOGrA1ymonpuTdK) (ред. 08.04.2024 15:56)*

> ​​@Гооол-й4ч
> 
> Числа скорее всего напрямую сравниваются процессорной командой сравнения чисел. Это просто ни капли не дороже чем сравнивать ссылки
> 
> А вот для строк сравнивать ссылки дешевле чем значения.
> 
> При этом никто не мешает сделать Рантайм который каждый раз сравнивает строки посимвольно

---

**[@Гооол-й4ч](https://www.youtube.com/channel/UCI_uKeDGw-qUumxR37GgSLA)** *[08.04.2024 13:41](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugy66Z1xlaev7P78nDJ4AaABAg) (ред. 08.04.2024 13:56) · 👍 1*

Вот я гоняю тесты на d8 и разница в использованиии add и push, например, всегда явно прослеживается ( в сторону add  ).
  А попытки как-то ускорить работу кода указанием длинны массива, использованием Array(1000), или Array.from зачастую только ухудшают перфоменс. Давно уже слышал от вас о том, что эффективнее сразу указывать длинну массива, если есть такая возможность, перед тем как мы будем его заполнять. Тогда тестил - это никак не улучшало перфоменс, сейчас потестил, заметив существование метода Array.from - результат тот же.

Вот, например, код:

1)

// 1.95

const q = Array.from({ length: 500_000 }, () => Math.random())

const d = []

q.forEach(elem => d.push(elem))

console.log(d)



2)

// 2.3

const q = Array.from({ length: 500_000 }, () => Math.random())

const d = Array.from({ length: 500_000 }, () => 0.1)

q.forEach(elem => d.push(elem))

console.log(d)



В q присваиваю массив длинной в 500к, наполненный рандомными double-числами ( не уверен, имеет ли это смысл, подумал что так точно не будет какой-то оптимизации, мол не будет в массиве повторяться 10 раз один числовой ряд, как получилось бы при ctrl c + ctrl v вставке). 
И вот я прохожусь по нему и копирую его значения в другой массив ( d ).
Вроде как во 2ом случае я сразу задаю фиксированную длинну, наполняю его числами того же типа, у меня double packed, который не потребует дальнейшего расширения. Но вот по итогу среднее время работы такого кода - 2.3. А время работы первого варианта, с созданием обычного пустого массива - 1.95 ( указаны средние показатели за где-то 20 запусков для каждого варианта ). 

Я что-то упускаю в тестах ( в плане кода ) или может всё должно работать быстрее во 2ом случае, но просто проблема с настройкой тестовой среды?

Если вообще смысл заниматься всем этим ( попыткой оптимизировать работу с мутированием массива ), когда можно просто создать из массива Set ( при наличии уже существующего массива ), сделать вставки, удаления и преобразовать Set обратно в массив, будто даже так это всё будет быстрее?

> **[@artyomboyko8219](https://www.youtube.com/channel/UCQzmt-1-dk3Z6bWiThdyj4g)** *[12.04.2024 15:55](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugy66Z1xlaev7P78nDJ4AaABAg.A1yfHskeN9bA28CjBJUBej)*

> Ты сравниваешь пуш и пуш
> С той разницей, что во втором варианте у тебя массив из миллиона элементов получается
> 
> Во втором варианте нужно по индексу присваивать, а не пушить

> **[@Гооол-й4ч](https://www.youtube.com/channel/UCI_uKeDGw-qUumxR37GgSLA)** *[12.04.2024 18:44](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugy66Z1xlaev7P78nDJ4AaABAg.A1yfHskeN9bA28WAOFEPOw) (ред. 18.04.2024 02:44)*

> @artyomboyko8219 при чём тут это вообще, если вся суть теста - сравнить, как на производителность влияет изначальное состояние массива, который будет заполнен. С чего бы вдруг у меня способ добавление элемента в цикле должен как-то меняться во 2ом кейсе?

> **[@artyomboyko8219](https://www.youtube.com/channel/UCQzmt-1-dk3Z6bWiThdyj4g)** *[13.04.2024 09:31](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugy66Z1xlaev7P78nDJ4AaABAg.A1yfHskeN9bA2A5_8NvsN4) · 👍 1*

> @Гооол-й4ч ты говоришь «у меня double-packed, который не потребует дольнейшего расширения»
> Но как не потребует, если ты его расширяешь? Было 500000 элементов, а ты рушишь в него 500001, 500002 и так до миллиона
> Ты расширил второй массив своими пушами также как и в первом кейсе
> 
> У тебя нет разницы между первым и вторым кейсом, кроме той, что во втором кейсе массив изначально не пустой, а имеет длину 500000
> 
> Если ты хочешь «скопировать первый массив во второй» и при этом изначально задать второму массиву длину и наполнить его изначальными значениями, то нужно по индексу присваивать
> 
> d[0] = q[0]

> **[@Гооол-й4ч](https://www.youtube.com/channel/UCI_uKeDGw-qUumxR37GgSLA)** *[13.04.2024 10:08](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugy66Z1xlaev7P78nDJ4AaABAg.A1yfHskeN9bA2A9uX7o89S)*

> @artyomboyko8219 , дааа, есть такое, дошло, спасибо.

---

**[@narek7281](https://www.youtube.com/channel/UCUa3U5-hu8KquLW_b1ubKbA)** *[21.04.2024 11:57](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=UgxrApmPtUoVwnnDZ_l4AaABAg)*

great video

---

**[@Et47](https://www.youtube.com/channel/UCYr9X1Zuzj6x0LwhKNAe3jA)** *[29.05.2024 11:11](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=UgyWhaNZUnoGwuP5BG94AaABAg)*

А кто нибудь может мне объяснить (вопрос не по теме), недавно заметил, почему что Chrome, что Firefox, что Edge и даже Opera при включенном видео на Youtube потребляют больше ресурсов процессора, чем Яндекс? Последний не более 15-20%, на втором месте Chrome - 25-34%, далее остальные. Пробовал и в win 10 и в Linux (Ubuntu, Mandjaro, Fedora, Mint). Не могу понять, хоть и у всех практически движок V8.

---

**[@OlexanderParkhomenko](https://www.youtube.com/channel/UC6mG3Z3E8nGbepFJyr6YtXw)** *[04.07.2024 23:38](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugy1MZlf67XvPSD3HT94AaABAg) · 👍 3*

15:30 всё как на зоне - если уже стал "дырявым", то раздырявится уже нельзя

---

**[@valvetigu5207](https://www.youtube.com/channel/UC4hEa6vhI7hFePcFTb-pPSQ)** *[14.10.2024 18:05](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=UgxNoEGp5buEJtq0MzB4AaABAg)*

Кот научил человека програмировать. Очень грамотный котяра

---

**[@diniszabrodsky8508](https://www.youtube.com/channel/UCkO7hEGdqVb-PPRUbU3pdJg)** *[18.05.2025 14:50](https://www.youtube.com/watch?v=fWqOswHMjEo&lc=Ugz8uVx4ltTJ9Rgq_HN4AaABAg)*

Це правда для байт коду і коду асемблера? Чи в байт коді він діє згідно специфікації? [[Base]] .......

---
