---
title: "⎡msk⎦⎡04⎦ Производительность JavaScript и типы данных: Числа / Number."
date: 2023-06-21
tags: []
videoId: "YntHgxlmKy4"
duration: "33:25"
views: 2667
likes: 215
comments: 19
---
# [⎡msk⎦⎡04⎦ Производительность JavaScript и типы данных: Числа / Number.](https://www.youtube.com/watch?v=YntHgxlmKy4)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 21.06.2023 06:38  
**Тривалість:** 33:25  
**Перегляди:** 2667 · **Лайки:** 215 · **Коментарі:** 19
![thumbnail](https://i.ytimg.com/vi/YntHgxlmKy4/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=YntHgxlmKy4)
## Коментарі (10 · відповідей: 9)

**[@SERGIUS_ORIGINAL](https://www.youtube.com/channel/UCorE8HdQ4HputSutpZpphFg)** *[20.06.2023 20:36](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgyhaEcnvlCz7_aM_7Z4AaABAg) · 👍 3*

Благодарю за шикарнейший контент. Рекомендую всем.!!!

---

**[@chikenmacnugget](https://www.youtube.com/channel/UCyWOOKPeKYrjDQcZqz0Gyiw)** *[23.06.2023 05:31](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgzUZIDFwcZMpvF7rtd4AaABAg)*

По логике вещей NaN должен быть предсозданным объектом как и undefined. А значит, когда мы будем ссылаться на NaN, то ничего нового мы не создадим

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[26.06.2023 10:10](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgzUZIDFwcZMpvF7rtd4AaABAg.9rI3dETUEJ69rQHyLbbITt) · 👍 2*

> Да. NaN и есть предопределенным обьектом в рамках GLobalObject. Причем в случае V8 это обьект с максимально простой структурой. 
> Причем в рамках V8 при оптимизации, код связанный с проверкой на NaN сокращается в одну строку - на проверку числовой константы, которая лежит по определеному заранее преопределенному адресу оперативной памяти.

> **[@chikenmacnugget](https://www.youtube.com/channel/UCyWOOKPeKYrjDQcZqz0Gyiw)** *[26.06.2023 10:28](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgzUZIDFwcZMpvF7rtd4AaABAg.9rI3dETUEJ69rQK0bZIr7X) (ред. 13.06.2024 21:54) · 👍 1*

> @AsForJS просто в видео было сказано обратное

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[04.07.2023 01:09](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgzUZIDFwcZMpvF7rtd4AaABAg.9rI3dETUEJ69rivOF0BTWT) · 👍 1*

> Дайте ссылку на время в видео, с комментарием, что именно Вы заметили.
> Если окажется, что Вы правы, я просто обязан об этом как написать, так и заявить в других видео. 
> 
> Пока я не очень понимаю о каком именно куске видео Вы говорите.

> **[@chikenmacnugget](https://www.youtube.com/channel/UCyWOOKPeKYrjDQcZqz0Gyiw)** *[04.07.2023 04:35](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgzUZIDFwcZMpvF7rtd4AaABAg.9rI3dETUEJ69rjHwyZwWQh) (ред. 13.06.2024 21:54)*

> @AsForJS19:35 примерно

---

**[@dmitry4337](https://www.youtube.com/channel/UCEfSN8EnrT2QiQ5bqsYRncQ)** *[25.06.2023 09:07](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgzURkHN2Fsz-ESbTV54AaABAg)*

в тайпскрипті ви можете використати branded type якщо вам потрібен якийсь конкретний підтип, наприклад number8

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[26.06.2023 10:08](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgzURkHN2Fsz-ESbTV54AaABAg.9rNaydXdv-R9rQHiY31U9s) · 👍 2*

> То є так. Але Тайпскріпт зроблено таким чином, що код який він генерує, не має ніякого відношення щодо перформенсу.

> **[@dmitry4337](https://www.youtube.com/channel/UCEfSN8EnrT2QiQ5bqsYRncQ)** *[27.06.2023 08:49](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgzURkHN2Fsz-ESbTV54AaABAg.9rNaydXdv-R9rSiViGDOcp) (ред. 18.04.2024 03:12)*

> ​@AsForJS Ви маєте на увазі, що ts генерує неоптимальний код? 
> Код згенерований тайпскриптом залежить від target який ви вказали в вашому tsconfig. якщо ви вкажете   es5, то звичайно тайпскрипт при еміті коду буде застосовувати набір трасформерів для генерації поліфілів. Якщо ж вказати target es next то будуть застосовані тільки:
>  1) трансформер який вирізає анотації типів з аст 
>  2) трансформер class fields
>  3) резолвер модулів  
> 
> жоден з яких не впливає на перформанс.  
> 
> якщо в вас інша думка, то було б цікаво побачити приклади, чи може навіть окремий випуск присвячений ts
> 
> якщо тайпскрипт генерує неоптимальний код, то варто відкрити issue чи зробити PR (правда я не в курсі як активно вони мержать сторонні PR)

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[04.07.2023 01:07](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgzURkHN2Fsz-ESbTV54AaABAg.9rNaydXdv-R9rivCzLeGsi) · 👍 1*

> Я маю на увазі наступне:
> Ті обмеження, які накладав спочатку свого існування TS на програміста, дозволять код, який був написан цим програмістом, у разі компіляції привести до максимально ефективної форми. Тобто, якщо б програмісти компілятору TS дали собі волю, то вони б змогли  зробити так, щоб TS компілятор генерував максимально ефективній код.
> 
> Але ж, цього не будо зроблено тоді та вже не може бути зроблено зараз. Бо еволюція TS пішла шляхом, який зробив це неможливим. Як найменш в загальному сенсі цього слова. Можливо, це ще зробити частково, але в загалі вже ні.
> 
> Бо інженери TS обрали шлях формування мови з потрібними їм можливостями, але не мови яка б дозволяла не лише контролювати типи, але й на основі цієї інформації генерувати оптимізований код. 
> 
> TS - це глухий кут.
> Прорив щодо JS зараз можливий лише в одному напрямку - додання до синтаксису статичної типізації. І це виведе JS на новий рівень. Це буде революція, значно більше ніж поява ES5

> **[@Alequez97](https://www.youtube.com/channel/UCNi45kuHt5_49ESN6VijsGw)** *[29.05.2024 13:57](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgzURkHN2Fsz-ESbTV54AaABAg.9rNaydXdv-RA410fEA4DEI)*

> ​@AsForJSМне кажется или в другом видео Вы рассказывали о том, что попытка протащить в спецификацию типизацию аналогичной в ТайпСкрипт это идиотское решение и что автором спецификации не стоит этого делать. Здесь же вы говорите, что это была бы революция. Или я что-то неверно вспомнил?

---

**[@liganshow](https://www.youtube.com/channel/UCRP46IO-xsC-LvHHMnjMavA)** *[01.07.2023 12:01](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=Ugx_EI1TNsCNZmMhn-14AaABAg)*

А что насчет infinite и -infinite?)

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[03.07.2023 22:06](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=Ugx_EI1TNsCNZmMhn-14AaABAg.9rcMgoUE-wN9riaWsvmAxe) · 👍 1*

> Ровно тоже самое что и для NaN или -0.
> Об этом пойдет речь в следующем видео. А именно о том, как и какие константы представлены.

---

**[@island1345](https://www.youtube.com/channel/UCS2aZI1ZW4j9keu0pnlbB6w)** *[03.11.2023 16:59](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgwGiqtpoPnIo8abRd94AaABAg)*

супер

---

**[@borozenniy4561](https://www.youtube.com/channel/UCGYWz8qLO6YHXzpZ90F9iUw)** *[20.11.2023 18:32](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgyVl3R_nwRRCsyCpOF4AaABAg)*

Дякую за відео

---

**[@Last_Voyager](https://www.youtube.com/channel/UCnkXuaSY1KLwFy0BgQ-WCjg)** *[28.11.2023 07:56](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgxW8q2P1MesbkBFsr54AaABAg)*

Дякую

---

**[@johngalt9494](https://www.youtube.com/channel/UCULcuPJ1SALjUpSli2PMNyA)** *[29.12.2023 18:07](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgweuCs5AB2dxzeKMJR4AaABAg) · 👍 1*

Коммент в поддержку канала !

---

**[@kosee4008](https://www.youtube.com/channel/UCY2IBduXMsjHIJom9vWszRQ)** *[02.01.2024 13:37](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=UgxeJAIXQIQReGAsV5N4AaABAg)*

Ваш канал для меня открытие! Посоветуйте, пожалуйста, оптимальный подход к обработке многомерно массива с данными: к элементам массива с индексами x,y,z (до 10 млн элементов) присоединяю объекты с данными. Формат объекта и типы данных ещё не выбрал. Нужно максимально быстро, имеется возможность распараллеливания на графические процессоры. Спасибо!

---

**[@narek7281](https://www.youtube.com/channel/UCUa3U5-hu8KquLW_b1ubKbA)** *[20.04.2024 17:22](https://www.youtube.com/watch?v=YntHgxlmKy4&lc=Ugza1u_5rmjFG7m6AMh4AaABAg)*

great video

---
