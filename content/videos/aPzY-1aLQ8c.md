---
title: "⎡msk⎦ Обзор на JavaScript видео \"Подсвечиваем НЕ ЛАТИНСКИЕ СИМВОЛы в коде и тексте\""
date: 2023-06-10
tags: []
videoId: "aPzY-1aLQ8c"
duration: "2:06:19"
views: 1723
likes: 71
comments: 14
---
# [⎡msk⎦ Обзор на JavaScript видео "Подсвечиваем НЕ ЛАТИНСКИЕ СИМВОЛы в коде и тексте"](https://www.youtube.com/watch?v=aPzY-1aLQ8c)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 10.06.2023 00:48  
**Тривалість:** 2:06:19  
**Перегляди:** 1723 · **Лайки:** 71 · **Коментарі:** 14
![thumbnail](https://i.ytimg.com/vi/aPzY-1aLQ8c/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=aPzY-1aLQ8c)
## Коментарі (9 · відповідей: 5)

**[@chikenmacnugget](https://www.youtube.com/channel/UCyWOOKPeKYrjDQcZqz0Gyiw)** *[10.06.2023 04:45](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=Ugxnlw9FqgY9XbnMLCJ4AaABAg) · 👍 1*

Ну что-то через спред тв сделал в 2 раза меньше массив…

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[26.06.2023 13:58](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=Ugxnlw9FqgY9XbnMLCJ4AaABAg.9qlW5RQj3rl9rQh2jQe8Mz)*

> Потому что через спреад, вызывается Итератор обьекта String, который оперирует не символами UTF16, а codePoint-ами. 
> В результате сурогатные пары, которые состоять из двух символов UTF16 превращаются в 1 codePoint
> 
> Пример:
> '🏴'.length;   //2
> [...'🏴']; // ['🏴']
> `\ud83c\udff4`; // ['🏴']
> `\u{1f3f4}`; // ['🏴']

---

**[@kegorfx](https://www.youtube.com/channel/UCqUWxuaSIlR5EcUYyrtl_ww)** *[10.06.2023 13:51](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=UgweFg3eqbRchb6pXX54AaABAg) · 👍 1*

Вам надо успокоительное пить или медитацией заниматься 😂. 

Контент на канале, конечно, супер. Спасибо за него.

P. S. А чому не державною? (Извините, не удержался😂)

---

**[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[10.06.2023 15:04](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=UgxNgeL-bx7EZmbAitJ4AaABAg) · 👍 5*

Шо, Мурыч! До канала Лущенко уже добрался, да?))

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[26.06.2023 13:39](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=UgxNgeL-bx7EZmbAitJ4AaABAg.9qmbwmUc4_X9rQetTgS8bE) · 👍 1*

> Это он до меня, а не я до него

---

**[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[10.06.2023 15:06](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=UgzNQaE69SxBxHXPRLx4AaABAg) · 👍 2*

Имя им легион - тем, кто спеку не читал, а ведет ютуб канал по JS.

---

**[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[11.06.2023 14:26](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=UgxMxYnTVitoiMmLJ7x4AaABAg) (ред. 11.06.2023 14:27) · 👍 4*

Мурыч, поясни мне пожалуйста.

Почему флаг Уэльса дал длину строки 14, а спрэд оператор выдал массив с 7 элементами?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[26.06.2023 13:38](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=UgxMxYnTVitoiMmLJ7x4AaABAg.9qp7NgkvgWk9rQenhxZCtt) (ред. 26.06.2023 14:09) · 👍 1*

> Потому, что spread использует итератор от Object  String.
> А итератор от String разбирает строку по codePoint
> Соотвественно флаг Уэльса состоит из 14 UTF16 символов но при этом, используются CodePoint которые используют по два UTF16 символа.
> 
> Например:
> Первый символ для флага уэльса - это эмодзи черного флага
> `🏴`
> `🏴`.length; //2
> [...`🏴`]; '' [`🏴`]
> которое можно получить используя два UTF16 кода
> `\ud83c\udff4`
> или при помощи 1 codePoint
> `\u{1f3f4}`
> 
> Это как раз показательный пример того, каким монстром стал unicode.
> 
> 
> Кстати на простора интернета, раньше был распространен подобный метод подсчета символов в строке, используя spread на строке

---

**[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[11.06.2023 16:05](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=UgzmO68rU28ZlZ4Zhvh4AaABAg) · 👍 5*

Я всегда старался избегать регулярок - трудно быть безмозглым)

---

**[@IvanIvanov-ss8lj](https://www.youtube.com/channel/UCYdJ47daC9tbacjIxNOWHDw)** *[15.06.2023 02:54](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=UgxLa4mtNhIYelRJG9Z4AaABAg) · 👍 1*

Лучше всё-таки не показавать, что у вас в папке загрузок скачано)

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[26.06.2023 12:48](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=UgxLa4mtNhIYelRJG9Z4AaABAg.9qyBLoBkpI29rQ_54ZpyJd) · 👍 1*

> Если Вы о порнографии. То это не секрет. Это отдельная часть моей работы. Есть видео на других каналах где я рассказываю об этом. 
> Дело в том, что я достаточно глубоко разбираюсь в техническом SEO. А это область которая имеет первое применение именно в плоскости продвижения сайтов с порнографией.
> Потому, меня не единожды привлекают как консультанта по этой области.
> 
> О чем есть и видео, где я напрямую показываю инструменты которыми пользуюсь для решения задач подобного рода. Точнее пользовался раньше.

> **[@IvanIvanov-ss8lj](https://www.youtube.com/channel/UCYdJ47daC9tbacjIxNOWHDw)** *[28.06.2023 05:29](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=UgxLa4mtNhIYelRJG9Z4AaABAg.9qyBLoBkpI29rUwNvHXnFH) (ред. 18.04.2024 00:46) · 👍 1*

> @AsForJS Интересно)

---

**[@recycle-bin-camp](https://www.youtube.com/channel/UCn-3ty2MkvT3LV866YyEhpA)** *[30.01.2024 18:28](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=Ugx4W9bWs_nKF6mb7HV4AaABAg)*

если посимвольно нельзя перебирать как тогда перебирать?

---

**[@narek7281](https://www.youtube.com/channel/UCUa3U5-hu8KquLW_b1ubKbA)** *[25.04.2024 19:39](https://www.youtube.com/watch?v=aPzY-1aLQ8c&lc=Ugws8oIkarO-JV2ynWp4AaABAg)*

great video

---
