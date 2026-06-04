---
title: "[Stripped] Тип String согласно официальной спецификации ECMAScript. Часть 1 из 3."
date: 2025-06-14
tags: ["spec", "9", "js", "ecma", "String", "unicode", "utf16"]
videoId: "wCcVWQ9bikg"
duration: "50:28"
views: 2683
likes: 150
comments: 17
---
# [[Stripped] Тип String согласно официальной спецификации ECMAScript. Часть 1 из 3.](https://www.youtube.com/watch?v=wCcVWQ9bikg)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 14.06.2025 05:52  
**Тривалість:** 50:28  
**Перегляди:** 2683 · **Лайки:** 150 · **Коментарі:** 17
![thumbnail](https://i.ytimg.com/vi/wCcVWQ9bikg/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=wCcVWQ9bikg)
## Коментарі (13 · відповідей: 4)

**[@AlexanderBorshak](https://www.youtube.com/channel/UCcY6GQl77kuMf2BjIB-HjhQ)** *[14.06.2025 08:17](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=Ugx0_PXUn6cHB2vjrhZ4AaABAg) · 👍 2*

Там может стоило в самом начале сказать, что строки в  JS хранятся в формате Unicode, где для хранения символа используются т.н.  Code Unit; а сами Code Unit в строках закодированы в формате UTF16, то есть каждый "символ" занимает 2 (или 4) байта. А так - за деревьями леса не видно...

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[15.06.2025 02:54](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=Ugx0_PXUn6cHB2vjrhZ4AaABAg.AJLS_CODJzXAJNSS9sk9UT) · 👍 4*

> Нельзя. И вот почему.
> Как только Вы скажете, что это прямое следствие стандарта Uicode, то Вам придется объяснять что это за стандарт и как он работает, уйдя от основной темы. 
> Причем уйдя настолько далеко, что вам и месяца не хватит описывая все пограничные случаи.
> 
> Простое же заявление о том, что это стандарт Unicode - это пердеж в лужу, которое ничего кроме знание термина Unicode не поясняет. Напомню, спецификация стандарта Unicode, как минимум, в полтора раза больше спецификации ECMA.
> 
> Мой преподавательский опыт мне наглядно продемонстрировал, что идти нужно от примеры проблемы к ее решению. После чего уже формировать вокруг решения теоретическую базу.

---

**[@greatfiredragon](https://www.youtube.com/channel/UCyzSr6mqFWvt8RlMmqzHtYw)** *[14.06.2025 18:36](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=Ugygg0LFWNGC8XCixMx4AaABAg) · 👍 1*

Ого, спасибо! Долго и подробно, да ещё и с примерами — кайф!

---

**[@yomo1abh586](https://www.youtube.com/channel/UCoCgTB0pDpma-m1KK4j6dqA)** *[14.06.2025 22:00](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=UgzI4CPcX6c9gfUT-5x4AaABAg) (ред. 14.06.2025 22:17)*

Спасибо большое за эту лекцию !)
Мне, тупенькому фронту, в свои 20 лет не совсем понятно зачем  мне это знать, но сам процесс доставляет удовольствие. 

Еще раз спасибо  большое. С удовольствием слушал и делал конспекты ))

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[15.06.2025 02:45](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=UgzI4CPcX6c9gfUT-5x4AaABAg.AJMviopYG_hAJNRRTdv0zV) · 👍 4*

> Поставят вдруг Вам задачу обработки текста, а вы уже будете знать откуда ноги растут и не повторите типичных ошибок с length split и т.д.

> **[@yomo1abh586](https://www.youtube.com/channel/UCoCgTB0pDpma-m1KK4j6dqA)** *[15.06.2025 03:10](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=UgzI4CPcX6c9gfUT-5x4AaABAg.AJMviopYG_hAJNUGZJU3tG) · 👍 1*

> ​@AsForJS искренне надеюсь дожить до времени,  когда угоубленные знания языка будут важнее на работе чем очеркдной фреймворк. 
> То что сейчас на фронте мало удовольствия доставляет,  будто постепенно просиходит стогнация знаний.
> 
> Спасибо еще раз за отличный материал. Буду ждать следующую часть)

---

**[@sergeystarkov8010](https://www.youtube.com/channel/UCdl2geq2PfEIpO7xq3Lyy7Q)** *[19.06.2025 21:12](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=Ugzj_46IdvwUZrYp0K14AaABAg)*

Спасибо за обрезанную версию - так, действительно, удобней. Ждём продолжения!

---

**[@rwxae](https://www.youtube.com/channel/UCYnEbUWhqWxc93u8VIme_wQ)** *[24.06.2025 11:24](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=Ugy2MW4PWPzLNd82NSB4AaABAg) · 👍 1*

Полезный метериал, большое спасибо за то, что делаете!

---

**[@rerurkful](https://www.youtube.com/channel/UCgJQG9TBnlKENdGSnxqh2bA)** *[26.06.2025 19:16](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=UgxomunNGCcUQ-yjOGJ4AaABAg) · 👍 1*

Блин, Мурыч, прям вот респектище!!!!! Красавчик!!!!

---

**[@qubbiq](https://www.youtube.com/channel/UCU3Ig9mg5sgw4NaVh-dpnSQ)** *[27.06.2025 17:29](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=UgxrvgFr8Vn0cyN0EpZ4AaABAg)*

А можно ссылку на презентацию?

---

**[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[30.06.2025 20:17](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=Ugzp4Ikxdax6bsTx-cV4AaABAg)*

Таймкоды:
00:00:00 Введение
00:01:17 Дисклеймер
00:01:27 О чем пойдет лекция 
00:01:37 Формат лекций
00:02:45 Для кого это лекция 
00:07:06 Что такое String и Code Unit
00:10:00 Code Unit на примерах
00:12:00 Grapheme  
00:16:25 Grapheme на примерах
00:19:22 Промежуточные итоги  
00:24:25 Примеры для самоконтроля  
00:29:10 Стандарт Unicode  
00:29:53 Unicode и таблица символов
00:38:56 Unicode Code Point
00:40:04 Unicode промежуточные итоги  
00:49:14 Code Point и Code Unit (конец первой части)

---

**[@vidinnenpc](https://www.youtube.com/channel/UCEDy_EJsn0QxuJGGx9QnNbQ)** *[18.07.2025 09:00](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=UgwXh5LI0fi0zLiNgzl4AaABAg)*

Подскажите пожалуйста. Я ввёл в консоли хрома var a = 'й', var b = 'й', и у меня сравнение переменных true даёт. Почему у вас false? Я что-то не так делаю?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[29.07.2025 21:44](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=UgwXh5LI0fi0zLiNgzl4AaABAg.AKi4VHzKxlYALAllqKBoQn) · 👍 2*

> Потому что отображаемый символ, согласно стандарту Unicode это не обязательно тоже самое что и вводимый. 
> 
> Кириллический "й" может быть представлен двумя способами: как U+0439 и как последовательность из двух Code Unit: '\u0438\u0306'
> 
> `й` === '\u0438\u0306'; // false
> `й` === '\u0438\u0306'.normalize(); // true
> `й`.normalize('NFD') === '\u0438\u0306'; // true

---

**[@Andreitrenkal](https://www.youtube.com/channel/UCqmzhvFupuq_6i5a-UNeFig)** *[29.09.2025 21:36](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=Ugz66ig2QQZhnppz4Yl4AaABAg) · 👍 1*

Это было очень сильно! Спасибо!

---

**[@artsus4](https://www.youtube.com/channel/UCGCR-6JRjXy7N8C0nREXbWg)** *[01.01.2026 04:54](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=Ugw1AmEsSyT1Y8K3N4B4AaABAg)*

Дякую! Років десять тому читав теж саме, але для Java. Пригадуються якісь Code Plains та суррогатні пари. Проте, із символами поза перші 65536 так і не вдалося попрацювати, тому деталі забулися. А може, спочатку забулися деталі, і саме через це із символами з "вищих  вимірів" і не працював.

---

**[@keeeparis](https://www.youtube.com/channel/UCB8CTMJf5M8uWeeLoVZt49A)** *[05.03.2026 09:17](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=UgyqgjacQEdEy6HGmol4AaABAg)*

это очень крутое видео!

---

**[@exedealer](https://www.youtube.com/channel/UCFhHWgJZB0MWCmK_Cu5rKlQ)** *[22.05.2026 16:44](https://www.youtube.com/watch?v=wCcVWQ9bikg&lc=UgyB-iMszd3Vkfmv0vl4AaABAg)*

спасибо

---
