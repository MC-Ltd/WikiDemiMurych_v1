---
title: "⎡msk⎦ Задача с JavaScript собеседования о разбиении текста на строки заданной длины"
date: 2023-06-12
tags: []
videoId: "yfJ475DYo2w"
duration: "1:11:07"
views: 2093
likes: 140
comments: 11
---
# [⎡msk⎦ Задача с JavaScript собеседования о разбиении текста на строки заданной длины](https://www.youtube.com/watch?v=yfJ475DYo2w)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 12.06.2023 12:43  
**Тривалість:** 1:11:07  
**Перегляди:** 2093 · **Лайки:** 140 · **Коментарі:** 11
![thumbnail](https://i.ytimg.com/vi/yfJ475DYo2w/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=yfJ475DYo2w)
## Коментарі (7 · відповідей: 4)

**[@SERGIUS_ORIGINAL](https://www.youtube.com/channel/UCorE8HdQ4HputSutpZpphFg)** *[12.06.2023 10:38](https://www.youtube.com/watch?v=yfJ475DYo2w&lc=UgznyqrBq5b4x1KdK694AaABAg) · 👍 2*

Спасибо за эту трилогию с регулярками и юникодом, благодаря вашему труду я нормально так прокачал себя))

---

**[@BorderInVais](https://www.youtube.com/channel/UC1qmXy2vQ-hICupQzU6Jgpw)** *[12.06.2023 15:36](https://www.youtube.com/watch?v=yfJ475DYo2w&lc=UgxPi-mYnjmFexVdWCJ4AaABAg) · 👍 4*

Отличный ролик!
Хочется меж тем дамп закладок из хрома

---

**[@Elvina.frontend](https://www.youtube.com/channel/UCJJysJYIyllQzb8Fa7uf1wQ)** *[28.11.2023 09:11](https://www.youtube.com/watch?v=yfJ475DYo2w&lc=UgzSCncJ8Hsjft24aWV4AaABAg)*

спасибо)

---

**[@volitilov](https://www.youtube.com/channel/UCo0CLP5RoF_YbUwwHzx3MnA)** *[30.11.2023 10:37](https://www.youtube.com/watch?v=yfJ475DYo2w&lc=UgzmEgWEX18H3uKzCsZ4AaABAg) (ред. 30.11.2023 10:39)*

Добрый день, а как js понимает что та или иная группа символов, должна показывать какой-то Emoji? Это что-то типа как реализована DNS система? И что такое сам Emoji как конечный результат -- это картинка?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[30.11.2023 22:28](https://www.youtube.com/watch?v=yfJ475DYo2w&lc=UgzmEgWEX18H3uKzCsZ4AaABAg.9xjar0xFUU_9xksGOBQ1-O)*

> Стандарт UNICODE єто не просто таблица где каждому коду, поставлен в соответствие какой то символ (отображение)
> 
> В стандарте Unicode дейтсвительно очень много символов, отображение которых соответствует именно принципу - код символ, но не все.
> 
> В стандарте Unicode уже очень давно появились алгоритмы формирования отображения символов. Срабатывание которых зависит от некоторых управляющих последовательностей.
> 
> Самая простая из которых называется - суррогатные пары, или combining character. Когда есть некоторый символ ( ударение) который в стандарте находится в какойто области, когда система отображения понимает, что это код, символа который нужно скмбинировать  со следущим. 
> 
> Например, если в JavaScript Вы напишите `\u{301}a` то в той же console вы увидите отображение буквы a с ударением а не просто буквы a. Что произошло благодаря первому упровляющему символу который был задан последовательностью \u{301}
> 
> И это самый простой пример. Современный стандарт Unicode содержит алгоритмы где на вход принимается 12 управляющих символов формируюших отображение.
> 
> И конкретно я считаю в данном случае, что люди накурились бамбука и свернули где то не туда. С другой стороны это мое менние можно засунуть в одно место, потому, что я не могу точно знать всех тех трудностей с которыми столкнулись люди, которые придумали именно такое стандарт.

---

**[@khmerhan2748](https://www.youtube.com/channel/UCQY3nUwcprTrW9ny_D2RHHw)** *[25.02.2024 16:12](https://www.youtube.com/watch?v=yfJ475DYo2w&lc=Ugwb_0GQAnqO_BdwNUN4AaABAg)*

благодарю за рассказ - про сложности со смайлами в юникоде не знала (((

---

**[@romansemchuk1837](https://www.youtube.com/channel/UC3wxbNSfzFBrWW8jYppAJ9Q)** *[14.05.2024 02:01](https://www.youtube.com/watch?v=yfJ475DYo2w&lc=UgwQ9Se9CVd-vuva5gx4AaABAg)*

Спасибо.

---

**[@Алексей-п4б](https://www.youtube.com/channel/UCzG-T8exY0y1XILvkqUv5qA)** *[14.06.2025 16:54](https://www.youtube.com/watch?v=yfJ475DYo2w&lc=Ugy3Pz5jxEcBtMbM8qp4AaABAg)*

Всем привет 
пишу код
 `мама 'мыла' раму`.match(/[\p{L}\p{N}\p{P}\p{S}\s]{1,6} (\s|$)/ug )
а результат не массив а null выдает,
Что не так я сделал, подскажите

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[15.06.2025 02:48](https://www.youtube.com/watch?v=yfJ475DYo2w&lc=Ugy3Pz5jxEcBtMbM8qp4AaABAg.AJMNnAbsiRxAJNRm_UtWWw) · 👍 2*

> У Вас перед (\s|$) стоит символ пробела. Удалите его и все заработает как Вы описали.
> 
> Тут следовало бы еще задать вопрос, что именно Вы хотели получить. Какую задачу решаете. Чтобы, возможно, подсказать более эффективное решение.

> **[@Alex-p6x9x](https://www.youtube.com/channel/UC3ecJ5ifc7mnWd5qF4lE6vg)** *[15.06.2025 03:00](https://www.youtube.com/watch?v=yfJ475DYo2w&lc=Ugy3Pz5jxEcBtMbM8qp4AaABAg.AJMNnAbsiRxAJNT8iyNwiX)*

> Огромное спасибо! 
> Удачи и ЗДОРОВЬЯ!

> **[@Алексей-п4б](https://www.youtube.com/channel/UCzG-T8exY0y1XILvkqUv5qA)** *[15.06.2025 09:36](https://www.youtube.com/watch?v=yfJ475DYo2w&lc=Ugy3Pz5jxEcBtMbM8qp4AaABAg.AJMNnAbsiRxAJOAS5-o_8-)*

> @AsForJS Спасибо! Задач нет, учится учится учится!

---
