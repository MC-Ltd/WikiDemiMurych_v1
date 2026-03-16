---
title: "Почему NaN это диапазон из 9 квадриллионов чисел"
date: 2025-09-12
tags: ["spec", "11", "js", "ecma", "IEEE754", "NaN"]
videoId: "QxmS2ny5o3s"
duration: "1:44:18"
views: 1946
likes: 83
comments: 5
---
# [Почему NaN это диапазон из 9 квадриллионов чисел](https://www.youtube.com/watch?v=QxmS2ny5o3s)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 12.09.2025 07:54  
**Тривалість:** 1:44:18  
**Перегляди:** 1946 · **Лайки:** 83 · **Коментарі:** 5
![thumbnail](https://i.ytimg.com/vi/QxmS2ny5o3s/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=QxmS2ny5o3s)
## Коментарі (4 · відповідей: 1)

**[@krasnovdyn](https://www.youtube.com/channel/UCPbVTsu6Eo2BVg5B1vyjqOA)** *[12.09.2025 09:25](https://www.youtube.com/watch?v=QxmS2ny5o3s&lc=Ugx3Su_hjd0T5ihWMHp4AaABAg) · 👍 2*

Спасибо за то, что рассказали про стандарт IEEE 754, было интересно. Но с другой стороны сложно ожидать от устройства умеющего работать только с числами, чтобы оно (устройство) представляло что-то не в виде чисел. Например согласно ASCII символ 'A' представлен в виде числа 65, а символ 'B' это число 66. Так что такое 'A' ? символ или число? В ASCII ведь тоже есть не совсем символы, но это тоже числа от 0 до 31. Так и с NaN в стандарте IEEE 754, как по другому в стандарте описывающем формат представления чисел представить не число? если в рамках самого формата, то только как число. Поэтому NaN это не число (NaN: not a number - a symbolic floating-point datum.) даже не смотря на то, что внутри самого формата NaN представлен в виде числа из определенного диапазона чисел. А использование NaN для каких-то других целей мне напомнило про "сверхчисла" в советских калькуляторах МК-52/МК-61, в журналах статьи печатали как при помощи недокументированных действий получить числа со степенью больше 99, да еще и что-то считать с ними, но зачем???

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[13.10.2025 01:51](https://www.youtube.com/watch?v=QxmS2ny5o3s&lc=Ugx3Su_hjd0T5ihWMHp4AaABAg.AMyJyVU7LcaAOCKaFU8Pqq)*

> Прежде всего для того, чтобы отдавать себе отчет в том, как работает процессор или компилятор, который оперирует нашими аргументами.  
> 
> Зная и понимая это - мы точнее управляем той машиной, которая решает поставленные нами задачи.
> 
> Ну и вообще, прикольно по хулиганить. (;

---

**[@narek7281](https://www.youtube.com/channel/UCUa3U5-hu8KquLW_b1ubKbA)** *[12.09.2025 13:01](https://www.youtube.com/watch?v=QxmS2ny5o3s&lc=UgxEuRNTXKFW5U-g4LF4AaABAg) · 👍 1*

Great video

---

**[@mcltdtm420](https://www.youtube.com/channel/UCu4YeW9ZlE51GwOEbpAox3w)** *[12.09.2025 22:13](https://www.youtube.com/watch?v=QxmS2ny5o3s&lc=UgxmjYyh2J8MCfGSWm94AaABAg) · 👍 1*

Lecture Notes on the Status of
IEEE Standard 754 for Binary Floating-Point Arithmetic
Prof. W. Kahan
Elect. Eng. & Computer Science
University of California
people . eecs . berkeley . edu / ~wkahan / ieee754status / IEEE754.PDF

IEEE Std 754™-2019
(Revision of IEEE Std 754-2008)
IEEE Standard for Floating-Point Arithmetic
www-users . cse . umn . edu / ~vinals / tspot_files / phys4041 / 2020 / IEEE%20Standard%20754-2019.pdf

---

**[@dimitro.cardellini](https://www.youtube.com/channel/UCiCQBJtKpWMy3O3-NYNMorA)** *[26.09.2025 09:32](https://www.youtube.com/watch?v=QxmS2ny5o3s&lc=Ugwna6KSXDPxQely4gt4AaABAg)*

Пан Мурич,
Може вартувало почати з банального: що вважати числом, а що числом не вважати.
Бо не зрозуміло, що саме Ви намагаєтесь довести ...

Число -- це обʼєкт, що входить хоча б в одну з множин чисел: натуральні, цілі, раціональні, дійсні, комплексні і т.д.
NaN за визначенням в жодну числову множину не входить.

А те, що NaN має цифрове представлення -- так все, що представлено в компʼєтері, представлено саме в цифровому вигляді.

Включення певного значення до типу даних Number не робить це значення Числом -- воно робить його елементом множини значень цього типу даних.

І з точки зору сучасного IEEE 754 NaN -- це не те, що не число. Це навіть не "число з рухомою комою". NaN -- це "одиниця даних з рухомою комою" (floating point datum).

А з точки зору старого стандарту IEEE 754, binary floating point number -- це бітовий рядок, ..., числове значення якого, ЯКЩО ІСНУЄ, визначається за формулою ... і т.д. Тобто, навіть тут випадки NaN та нескінченностей виокремлено -- як ті, що не мають числового значення. А головне тут сказано, що floating point number -- це не число, а спосіб представлення чисел.

Спроба довести, що NaN є числом -- це теж саме, як довести, що цифри і числа -- то є одне й те саме. Казати, що NaN -- то число, це те саме, що побачивши ABBA на афіші, сказати, що то вартість квитка в шведських кронах, нащось записана в 16-ковому форматі.

Спроба визначити число, не через входженя до однієї з основних числових множин, взагалі завершиться тим, що числом можна нзавати ВСЕ, абсолютно все.

---
