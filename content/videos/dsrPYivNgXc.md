---
title: "Try to hack My JavaScript: Решения для readyState"
date: 2025-02-08
tags: ["tthmjs", "1", "drs", "expl"]
videoId: "dsrPYivNgXc"
duration: "47:41"
views: 1940
likes: 98
comments: 9
---
# [Try to hack My JavaScript: Решения для readyState](https://www.youtube.com/watch?v=dsrPYivNgXc)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 08.02.2025 05:52  
**Тривалість:** 47:41  
**Перегляди:** 1940 · **Лайки:** 98 · **Коментарі:** 9
![thumbnail](https://i.ytimg.com/vi/dsrPYivNgXc/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=dsrPYivNgXc)
## Коментарі (7 · відповідей: 2)

**[@mazeltof3392](https://www.youtube.com/channel/UC2PsgpKa6H45LKKqPAxDUQQ)** *[07.02.2025 17:57](https://www.youtube.com/watch?v=dsrPYivNgXc&lc=UgyaaM3ioLbyNZImkWB4AaABAg) · 👍 2*

Мурыч, выздоравливай!

---

**[@valvetigu5207](https://www.youtube.com/channel/UC4hEa6vhI7hFePcFTb-pPSQ)** *[07.02.2025 18:09](https://www.youtube.com/watch?v=dsrPYivNgXc&lc=UgzS3OzdpKd4Jaxb0qB4AaABAg)*

мое имя в титрах. я улыбаюсь)

---

**[@alexperemey6046](https://www.youtube.com/channel/UCchNS6618CdinWR5iznDcAQ)** *[07.02.2025 18:34](https://www.youtube.com/watch?v=dsrPYivNgXc&lc=Ugziuu9pNEU-SCG6K3N4AaABAg)*

Вашу маму и тут и там показывают.

---

**[@greatfiredragon](https://www.youtube.com/channel/UCyzSr6mqFWvt8RlMmqzHtYw)** *[07.02.2025 18:44](https://www.youtube.com/watch?v=dsrPYivNgXc&lc=Ugzx-mpcdMuBfFrDAn14AaABAg) (ред. 07.02.2025 18:54) · 👍 2*

Мурыч, спасибо большое за эту задачку и за сегодняшний разбор решений! Сам я догадался только до одного решения (с подменой property), но так кайфанул, когда решил! Лучше тысячи оргазмов. Спасибо!

> **[@greatfiredragon](https://www.youtube.com/channel/UCyzSr6mqFWvt8RlMmqzHtYw)** *[07.02.2025 19:02](https://www.youtube.com/watch?v=dsrPYivNgXc&lc=Ugzx-mpcdMuBfFrDAn14AaABAg.AEFZPoyU4UlAEFaVICzwG9)*

> ИМХО это решение самое правильное.
> 
> ObserverAPI интересное, но все же как будто читерство)

> **[@greatfiredragon](https://www.youtube.com/channel/UCyzSr6mqFWvt8RlMmqzHtYw)** *[07.02.2025 19:11](https://www.youtube.com/watch?v=dsrPYivNgXc&lc=Ugzx-mpcdMuBfFrDAn14AaABAg.AEFZPoyU4UlAEFbSMpCHfI)*

> Пользуясь случаем, 
> Очень круто вы рассказали про реверс инжиниринг google docs. А недавно "взломали" hh.ru
> 
> Я не верил, что у hh.ru может быть настолько дебильный код... Но как оказывается может)
> 
> В google docs хотел бы узнать, как работать с обфусцировнным кодом. То есть, вот мы нашли функцию которая отвечает за цвет текста ссылки. А как написать userscript, которые сможет подменять эту функцию вне зависимости от её названия?

---

**[@The14Some1](https://www.youtube.com/channel/UCSD-4fNtuwjkwW4-XTSUfSQ)** *[08.02.2025 07:27](https://www.youtube.com/watch?v=dsrPYivNgXc&lc=UgxfXgs8eqhb-kB51dh4AaABAg)*

У Тучи течка?

---

**[@The14Some1](https://www.youtube.com/channel/UCSD-4fNtuwjkwW4-XTSUfSQ)** *[08.02.2025 07:43](https://www.youtube.com/watch?v=dsrPYivNgXc&lc=UgyVLL07PF1PYUJJp8d4AaABAg)*

43:05 Попрошу, eval у вас в отдельном скрипте. Его не обязательно подписывать, и подмена его ничего не даст.

---

**[@ilyagamepub](https://www.youtube.com/channel/UCOWeUcz3RAZeorXUxyIxrYQ)** *[20.02.2025 14:24](https://www.youtube.com/watch?v=dsrPYivNgXc&lc=Ugx9hwzn62UY_RLHI-x4AaABAg)*

Эх, жаль, что наткнулся на видео только сейчас.
У меня вот такое добро получилось для решения
let readyState = "complete";
Object.defineProperty(document, "readyState", {
    get() { 
        if(readyState === "complete"){
            readyState = NaN
            return NaN; 
        } else {
            readyState = "complete"
            return "complete";
        }  
            },
    set(value) { return readyState = value },
});
А теперь посмотрим решения от автора

---
