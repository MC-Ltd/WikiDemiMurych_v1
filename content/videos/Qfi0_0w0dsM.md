---
title: "Практика и теория сложности алгоритмов в контексте языка JavaScript"
date: 2025-07-18
tags: ["perf", "11", "computational", "complexity", "v8"]
videoId: "Qfi0_0w0dsM"
duration: "5:11:05"
views: 4826
likes: 160
comments: 10
---
# [Практика и теория сложности алгоритмов в контексте языка JavaScript](https://www.youtube.com/watch?v=Qfi0_0w0dsM)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 18.07.2025 00:25  
**Тривалість:** 5:11:05  
**Перегляди:** 4826 · **Лайки:** 160 · **Коментарі:** 10
![thumbnail](https://i.ytimg.com/vi/Qfi0_0w0dsM/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=Qfi0_0w0dsM)
## Коментарі (7 · відповідей: 3)

**[@RTFMurych](https://www.youtube.com/channel/UC3NVT782r84UDLdx9JXtbow)** *[18.07.2025 01:04](https://www.youtube.com/watch?v=Qfi0_0w0dsM&lc=UgypWTZ6utdrYsdpF9h4AaABAg)*

Игого: Big O бесполезен относительно JS, как JS бесполезен относительно счастья, но… увлечение Big O, способно приносить удовольствие как и увлечение JS.

---

**[@morskoj](https://www.youtube.com/channel/UCwhyAYoXok4Wj_sCPy_ScTg)** *[18.07.2025 06:38](https://www.youtube.com/watch?v=Qfi0_0w0dsM&lc=UgwxnU0ApoK1pyHKkhh4AaABAg)*

Спасибо большое!

---

**[@admToha](https://www.youtube.com/channel/UCVI_tHFBxVcJoxu86lGi5Qw)** *[18.07.2025 13:38](https://www.youtube.com/watch?v=Qfi0_0w0dsM&lc=UgzXJxfZlIb0pOGHeAF4AaABAg) (ред. 18.07.2025 13:45)*

Салют, Мурыч.
Можно вопрос?
На сколько затратна по времени и потреблению памяти рекурсия по сравнению с теми же действиями совершаемыми в циклах и при редуцировании reduce() в JavaScript?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[29.07.2025 21:36](https://www.youtube.com/watch?v=Qfi0_0w0dsM&lc=UgzXJxfZlIb0pOGHeAF4AaABAg.AKi_InImFUUALAklpA6jQa) · 👍 1*

> Зависит от конкретной реализации.
> Если брать V8 - то затратна на столько, что если можно ее избежать то это следует делать. Или выкручиваться за счет генераторов.
> 
> Это не проблема JS или его спецификации. Это проблема того как сделан V8 и отказа его рукводоства реализовывать часть спецификации касающейся Tail Position Call.
> 
> Если я верно помню, то в JSCore, эта оптимизация реализована. Но у меня никогда не доходили руки проверить как она там работает.

---

**[@ewfwefiweofwe](https://www.youtube.com/channel/UCP4dX9ufkHWPhGQfyiCWdGg)** *[18.07.2025 13:51](https://www.youtube.com/watch?v=Qfi0_0w0dsM&lc=Ugx7kKNeGDCJwZ-qGdx4AaABAg)*

я заметил что мурычу очень нравятся слова где встречается "жор". например коммивояжор или гугл кложор или просто кложор

---

**[@admToha](https://www.youtube.com/channel/UCVI_tHFBxVcJoxu86lGi5Qw)** *[18.07.2025 14:58](https://www.youtube.com/watch?v=Qfi0_0w0dsM&lc=UgxYyWIE2ArI_VsteE54AaABAg) · 👍 4*

Мы так и не услышали, как именно Мурыч использовал SAT на олимпиаде.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[29.07.2025 21:33](https://www.youtube.com/watch?v=Qfi0_0w0dsM&lc=UgxYyWIE2ArI_VsteE54AaABAg.AKiiTBph6rmALAkRE3a7uJ) · 👍 1*

> Я привел пример решения задачи, которое фактически удовлетворяется примитивным SAT солвером:
> 
> На вход подается поток чисел. Задача создать группы по 5 чисел, которые бы представляли наименьшую сумму из всех возможных.
> 
> Задача решается прямым перебором за 2 в степени n.
> Я придумал простой алгоритм составления этих групп, который реализовывался простым моим же SAT солвером, отвечающим на вопрос подходит группа или нет, без прямого перебора.

---

**[@АлексейСтепаненко-м8в](https://www.youtube.com/channel/UCQd5CW9PupQxYtXp7iyOmhA)** *[19.07.2025 10:36](https://www.youtube.com/watch?v=Qfi0_0w0dsM&lc=UgycvHjI9DNgLw2VlT94AaABAg)*

Мурыч, напиши алгоритм двухмерной триангуляции набора точек

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[29.07.2025 21:29](https://www.youtube.com/watch?v=Qfi0_0w0dsM&lc=UgycvHjI9DNgLw2VlT94AaABAg.AKkpNFhm00SALAjyOACgiD)*

> Если вспомню что это такое - то обязательно

---

**[@SerzhNesteruk](https://www.youtube.com/channel/UCvSxoIuRvinnq_mbU2KDTPA)** *[30.07.2025 20:06](https://www.youtube.com/watch?v=Qfi0_0w0dsM&lc=UgwbU8Q20idiQi8_Gwt4AaABAg)*

Как утверждает Demi Murych:
«Я беру на себя ответственность за КАЖДОЕ сказанное мной слово.» (07:41)
«Дональд Кнут, кстати, в своих книжках, когда оценивает алгоритмы, он вообще, в принципе, НЕ ИСПОЛЬЗУЕТ всей этой чухни, связанной с разными видами нотаций. Big O — это ж у нас не единственная нотация, обозначающая объём потребляемых ресурсов, или асимптотическую сложность потребления этих ресурсов, там их вообще десяток. Так вот, Дональд Кнут не использует НИ ОДНОЙ. Человек, который является признанным экспертом, который учит студентов, как программировать, НЕ ПОЛЬЗУЕТСЯ нотацией. Почему не пользуется? Потому что она бесполезна.» (01:08:39)

А как на самом деле?
Дональд Кнут настолько регулярно "вообще не использует ни одной" нотации асимптотической сложности, что в списке основных обозначений (приложение Б) его труда «Искусство программирования» значатся и Big O, и Big Omega (Ω), и Big Theta (Θ). Эти "бесполезные" нотации настолько не нужны, что их описанию даже посвящён отдельный раздел (1.2.11.1) в главе «Основные понятия» первого тома.

---
