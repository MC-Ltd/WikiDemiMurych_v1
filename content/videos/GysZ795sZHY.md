---
title: "Regular Function vs Arrow Function або відповіді на запитання для маленьких ДжаваСкриптерів"
date: 2022-08-17
tags: []
videoId: "GysZ795sZHY"
duration: "1:47:08"
views: 2193
likes: 95
comments: 10
---
# [Regular Function vs Arrow Function або відповіді на запитання для маленьких ДжаваСкриптерів](https://www.youtube.com/watch?v=GysZ795sZHY)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 17.08.2022 09:07  
**Тривалість:** 1:47:08  
**Перегляди:** 2193 · **Лайки:** 95 · **Коментарі:** 10
![thumbnail](https://i.ytimg.com/vi/GysZ795sZHY/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=GysZ795sZHY)
## Коментарі (9 · відповідей: 1)

**[@__-nr2pk](https://www.youtube.com/channel/UC8prB3C97jow-mBexje3q3g)** *[17.08.2022 17:22](https://www.youtube.com/watch?v=GysZ795sZHY&lc=Ugwd5mbaHyJZq7CFmLF4AaABAg) · 👍 2*

Спасибо!

---

**[@vancheloChanel](https://www.youtube.com/channel/UCoDrRhoSiUGJvJsmrVbKjOw)** *[18.08.2022 13:20](https://www.youtube.com/watch?v=GysZ795sZHY&lc=UgwzolGr97b3WM-eGOB4AaABAg) · 👍 2*

Вопрос в контексте "быстрых" свойств у объектов, есть ли смысл "замораживать" (Object.freeze()) объекты после создания, чтобы в рантайме было невозможно добавить в него свойства? Или Object.freeze накладывает дополнительные издержки на свойства такого объекта?

Спасибо!

---

**[@intellect-w4z](https://www.youtube.com/channel/UCrg_rwSydkmI7ZN__X6Shsg)** *[20.08.2022 00:59](https://www.youtube.com/watch?v=GysZ795sZHY&lc=Ugyy_VVtLRbHGi10VZV4AaABAg)*

Благодарю

---

**[@Андрей-м9с8ь](https://www.youtube.com/channel/UC1B21QPIR3-rLACmFMet17g)** *[25.08.2022 11:17](https://www.youtube.com/watch?v=GysZ795sZHY&lc=UgxQrG5sLexrgFIBLmN4AaABAg) (ред. 25.08.2022 11:18) · 👍 2*

Мурыч, если будет такая возможность, сделай, пожалуйста, видео с объяснением того, почему в JS нет такого общепринятого понятия, как "обертка над примитивными значениями", как этот механизм работает внутри (Reference Record, если я правильно понял и помню). Например: var test = 'abc'; test.charAt(1). Заранее благодарю!

---

**[@zhenia14](https://www.youtube.com/channel/UC4wVl97M79PeuMMZ6zGl2Pg)** *[04.09.2022 15:19](https://www.youtube.com/watch?v=GysZ795sZHY&lc=Ugyg_naOAFC7nPPQqz14AaABAg) · 👍 2*

Отличная подача, всё досканально. Можно ли разобрать this? куча информации, миллионы объяснений а как работает всеравно не понимаю.

---

**[@maddev8](https://www.youtube.com/channel/UCCRRd50MKiK4AjyAhylULbA)** *[16.09.2022 13:58](https://www.youtube.com/watch?v=GysZ795sZHY&lc=UgwuBfE1tD4WzRR0CJ94AaABAg) · 👍 3*

Мурыч ты говоришь (1:17:06), что компилятор делает дополнительную проверку на константу, а именно - не переопределен ли данный идентификатор. А почему он не делает такую же проверку на var theTen? Я же спокойно его могу также переопределить в том блоке, где ты показываешь переопределение константы.
var theTen = typeThing(0b11)
while(--repeater) {
    {
       var theTen='lalala';
    }
}

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[01.05.2023 05:05](https://www.youtube.com/watch?v=GysZ795sZHY&lc=UgwuBfE1tD4WzRR0CJ94AaABAg.9g2-6Yf_bll9p9Yb7OVsOO)*

> По той причине, что в случае var это делать не нужно - так как это регламентируется фактом вызова функции и возврата из функции. В случае же let и const - любой вложенный блок может стать проблемой. По этой причине с var все просто, а вот с let и const все сложно.
> В спецификацию их протащили очень зря. Из за них очень многое просело с точки зрения производительности. Но язык JS не был бы самим собой, если бы с ним нельзя было бы делать подобные вещи

---

**[@SERGIUS_ORIGINAL](https://www.youtube.com/channel/UCorE8HdQ4HputSutpZpphFg)** *[06.06.2023 16:24](https://www.youtube.com/watch?v=GysZ795sZHY&lc=UgzG1VskNVPFa-mZYNB4AaABAg)*

Благодарочка за працю.

---

**[@bulation9247](https://www.youtube.com/channel/UCEsDQNJPOijdA7Wno0GXnQQ)** *[15.07.2023 18:48](https://www.youtube.com/watch?v=GysZ795sZHY&lc=UgwAkKTinRycy5_EOs94AaABAg) (ред. 16.07.2023 13:07)*

Можно ли сделать вывод, что если я хочу добавить свойство в объект и не хочу использовать Map, то выгоднее будет сделать так:
obj = {
   ...obj,
   newProp: 'value',
}

---

**[@_Good_Evening_](https://www.youtube.com/channel/UC9HBo0_7o8jROXlvkFcVfIg)** *[31.12.2023 21:22](https://www.youtube.com/watch?v=GysZ795sZHY&lc=Ugx7c9bmauu8dpl5kop4AaABAg)*

Очень годный контент, огромное спасибо тебе, Мурыч!!!)

---
