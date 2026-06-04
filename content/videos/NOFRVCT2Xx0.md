---
title: "Производительность  V8 объектов  в примерах"
date: 2025-02-11
tags: ["perf", "9", "v8", "object", "examples"]
videoId: "NOFRVCT2Xx0"
duration: "2:08:13"
views: 2950
likes: 128
comments: 5
---
# [Производительность  V8 объектов  в примерах](https://www.youtube.com/watch?v=NOFRVCT2Xx0)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 11.02.2025 22:13  
**Тривалість:** 2:08:13  
**Перегляди:** 2950 · **Лайки:** 128 · **Коментарі:** 5
![thumbnail](https://i.ytimg.com/vi/NOFRVCT2Xx0/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=NOFRVCT2Xx0)
## Коментарі (3 · відповідей: 2)

**[@climenty](https://www.youtube.com/channel/UCt-g5THKMYPltnhpoKn8fhg)** *[12.02.2025 07:56](https://www.youtube.com/watch?v=NOFRVCT2Xx0&lc=Ugz3SyDGyBJ06yzkUap4AaABAg) · 👍 1*

Ценная информация по причине своей неочевидности. Получается, Класс, при всём своём странном положении в Javascript является одним из предпочтительных способов создания объекта, так как обеспечивает порядок создания свойств. А альтернатива в виде функции-конструктора фактически имитирует его поведение.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[11.05.2025 23:39](https://www.youtube.com/watch?v=NOFRVCT2Xx0&lc=Ugz3SyDGyBJ06yzkUap4AaABAg.AERHCTabhKhAI-Z7dNe1_S) · 👍 1*

> Правильно, только наоборот. Это класс имитация функции конструктора. 
> Самая предпочтительная форма создания обьекта - это литеральная форма. 
> То есть  что-то наподобие:
> 
> function cretaeObject(a,b,c) {
>     return { a,b, c};
> }

---

**[@Артем-в9э9щ](https://www.youtube.com/channel/UC1DWehEZ271S_0ePh7XHouA)** *[13.02.2025 06:38](https://www.youtube.com/watch?v=NOFRVCT2Xx0&lc=Ugw1cvsrVjN4NOmi4cl4AaABAg)*

То есть что получается, если взять 2 одинаковых, с точки зрения структуры, объекта, для js это разные объекты, как во всех документация по языку говорится "объект равен другому объекту, только тогда, когда это один и тот же объект". А v8 внутри себя делает эти объекты одинаковыми с помощью inline-cash ? Пока мы что-то не поменяем в их структуре и произойдет деоптимизация

> **[@hurdyga](https://www.youtube.com/channel/UCjbvLb0gsDglbt28DeBiYWg)** *[20.04.2025 17:08](https://www.youtube.com/watch?v=NOFRVCT2Xx0&lc=Ugw1cvsrVjN4NOmi4cl4AaABAg.AETi5CWg12pAH8mcsbMsl4)*

> В тебе в будь-якому разі 2 обʼєкти не будуть рівними один одному як мінімум тому, що це різні області памʼяті.
> Тобто:
> var a = { a: 1 };
> var b = { a: 1 };
> a === b // false;
> 
> Не за допомогою inline-cache, а за допомогою порівняння hidden classes. Деоптимізація відбудеться лише тоді, коли послідовність додавання/видалення буде різна, бо тоді Hidden Class буде різний. Тобто грубо кажучи, Hidden Class - це blueprint, чи історія того, як був створений обʼєкт.

---

**[@DShpak27](https://www.youtube.com/channel/UCzk7Q4WRNf8AMYsv8diqx1Q)** *[08.07.2025 16:44](https://www.youtube.com/watch?v=NOFRVCT2Xx0&lc=UgzVDnKYhDP-sJ09hdZ4AaABAg) · 👍 1*

Дякую, друже, за твій труд.

---
