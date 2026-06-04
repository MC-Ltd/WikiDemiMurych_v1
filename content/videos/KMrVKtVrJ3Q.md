---
title: "Производительность JS:  Обьекты в V8"
date: 2025-02-07
tags: ["perf", "8", "v8", "object"]
videoId: "KMrVKtVrJ3Q"
duration: "7:05:56"
views: 5343
likes: 177
comments: 14
---
# [Производительность JS:  Обьекты в V8](https://www.youtube.com/watch?v=KMrVKtVrJ3Q)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 07.02.2025 00:25  
**Тривалість:** 7:05:56  
**Перегляди:** 5343 · **Лайки:** 177 · **Коментарі:** 14
![thumbnail](https://i.ytimg.com/vi/KMrVKtVrJ3Q/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=KMrVKtVrJ3Q)
## Коментарі (6 · відповідей: 8)

**[@я-прогер-веб3](https://www.youtube.com/channel/UCH6LKRNP55LQpggzUFQOsVA)** *[07.02.2025 00:08](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=UgwEH2We286wWYyNo_d4AaABAg)*

Дано... Мутировать объекты нежелательно, удалять - добавлять свойства объекта нельзя!
Аргументация - анализ машинного кода сгенерированного интерпретатором

Пишем 3 минуты скрипт на коленке, даем шанс гипотезе :)
1 объект - тупо константа, пишем цикл 1м итераций, кидаем значение поля name в строку, засекаем время

2 докидываем в новый объект (специально не стал старый мутировать, а то в друг и там магия) объект 1млн полей, 
"чего нельзя делать", пишем цикл, в котором ищем поле по индексу, не тупо по ссылке .name как в первом тесте, 
а именно по объекту с 1м + полей, на каэдой из 1м итераций ищем поле по индексу i

3 пишем время старта Date.now() перед каждым тестом, считаем время Date.now() - время старта после цикла

из 50 тестов среднее время выполнения каждого цикла 80ms, как на 1м ключей, так и на 4. Почему?)

Почему забомбило? Да потому что Реакт отличная либа, а не так как Вы ее называете!!!!!

Скрипт приложил, тестил в браузере.

const test = () => {
    const obj_1 = {
      name: 'Ben',
      age: 30,
      info: {
        row_1: 'any',
        row_2: 1234567
      }
    }

    const start_time_1 = Date.now()
    let res_1 = '';
    for(let i = 0; i < 1000000; i++) {
      res_1 += obj_1.name;
    }
    console.log('const - ', Date.now() - start_time_1);

    const obj_2 = {
      name: 'Ben',
      age: 30,
      info: {
        row_1: 'any',
        row_2: 1234567
      }
    }
    for(let i = 0; i < 1000000; i++) {
      obj_2[`new_key_${i}`] = i;
    }
    
    const start_time_2 = Date.now()
    let res_2 = '';
    for(let i = 0; i < 1000000; i++) {
      res_2 += obj_2[i];
    }
    console.log('mut - ', Date.now() - start_time_2);
  }

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[07.02.2025 03:28](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=UgwEH2We286wWYyNo_d4AaABAg.AEDZfwUYn3TAEDv_gI36Vr) · 👍 4*

> По поводу твоих тестов. 
> Начни с того чтобы использовать performance.now который дает тебе высокоточный таймер. А не Date которое тебе таких гарантий не дает.
> 
> Пересмотри еще раз трансляцию.
> Там наглядным образом показано, что происходит при изменении формы Обьекта. 
> 
> Ты тестируешь не то, о чем шла речь. Строго говоря ты вообще непонятно что тестируешь.

> **[@я-прогер-веб3](https://www.youtube.com/channel/UCH6LKRNP55LQpggzUFQOsVA)** *[07.02.2025 12:15](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=UgwEH2We286wWYyNo_d4AaABAg.AEDZfwUYn3TAEErt6zI0e_) · 👍 1*

> ​@AsForJS тестировал время выполнения скрипта при работе с объектом, как Вы это называете с "измененной формой".

---

**[@igoronoprienko1259](https://www.youtube.com/channel/UCJqADnP3G2_YysqMY6weyQg)** *[07.02.2025 06:02](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=UgzaE5td2cv07Oco3Y54AaABAg) · 👍 1*

Это не стрим! Это стримище! :) Спасибо большое!

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[09.02.2025 18:20](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=UgzaE5td2cv07Oco3Y54AaABAg.AEECDpObGs2AEKfFM9sIk5)*

> єто шортс какой-то. требуем полной версии

> **[@igoronoprienko1259](https://www.youtube.com/channel/UCJqADnP3G2_YysqMY6weyQg)** *[12.02.2025 16:44](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=UgzaE5td2cv07Oco3Y54AaABAg.AEECDpObGs2AESD_v5tZpb) · 👍 1*

> @demimurych1 Мурыч, а можете пожалуйста сделать стрим и рассказать как программировать. В прямом смысле слова, как программировать??? Ну знаю я синтаксис JavaScript к примеру, знаю синтаксис языка С, а тетрис написать не могу. Могу написать простой конвертор валют. То есть как разбить задачу на подзадачи как выбрать структуру и т.д. Можно и на языке С если что. По сути это не важно на каком языке. На ютубе много пишут тетрисы но донести информацию не умеют или не хотят. Или посоветуйте книги где рассказывают как программировать, а не синтаксис и т.д. А может вообще надо начать с дискретной математики все? Я в тупике сейчас. Помогите. Спасибо.

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[13.02.2025 02:31](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=UgzaE5td2cv07Oco3Y54AaABAg.AEECDpObGs2AETGnPDiNc8)*

> @igoronoprienko1259 программировать нужно так, чтобы не было мучительно больно делать рефакторинг.
> 
> Главная мысль которую должен держтаь программист на подкорке, это как спланировать архитектуру приложения таким образом, чтобы она допускала свое расширение, без рисков сломать все приложение.
> 
> Исключение - вопросы кризис менеджмента.

> **[@igoronoprienko1259](https://www.youtube.com/channel/UCJqADnP3G2_YysqMY6weyQg)** *[13.02.2025 07:37](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=UgzaE5td2cv07Oco3Y54AaABAg.AEECDpObGs2AETomqu0l7X) (ред. 13.02.2025 07:37)*

> @demimurych1 "программировать нужно так, чтобы не было мучительно больно делать рефакторинг." Это если ты уже умеешь программировать. А если не умеешь? Как определять структуры данных для данных? Для того же тетриса к примеру я нашел в интернете, что фигурки можно хранить в массиве. Сам бы я никогда в жизни наверное не додумался бы. Вот как это чуйло развить? Может вы знаете какие то книги?

---

**[@Артем-в9э9щ](https://www.youtube.com/channel/UC1DWehEZ271S_0ePh7XHouA)** *[07.02.2025 11:36](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=Ugxt0HMktKVhvffvWuR4AaABAg)*

А в даном видео проводился тест, про который вначале говорили, когда 2 объекта (json) на 1 тыс. полей склеить, как в итоге будет вести себя js ?

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[09.02.2025 18:19](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=Ugxt0HMktKVhvffvWuR4AaABAg.AEEnPJaQEkMAEKf9QBET75)*

> в следующем.
> 
> если кратко, то на текущий момент в v8 стоит строгое ограничение:
> 
> пропертис ин обжект - 250 и не больше.
> пропертис во внешней структуре - еще 250
> 
> 
> любое привышение - переход в режим словаря.
> 
> 
> старые способы создать 32000 проперти ин обжетк, больше не работают

---

**[@kowkavn2356](https://www.youtube.com/channel/UCaCYq3PjfpFeCpZT0xciyfQ)** *[08.02.2025 22:44](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=UgzAncyOAPtAOu4DQVV4AaABAg) (ред. 09.02.2025 16:58)*

1:58:45 - 2:03:55 Краткий итог "Тип представления Named Properties",  (Де)Оптимизации с строковыми ключами
5:55:00 - Почему в js можно использовать символ доллара

---

**[@maddev8](https://www.youtube.com/channel/UCCRRd50MKiK4AjyAhylULbA)** *[27.02.2025 15:16](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=UgwZaQTsODV9HgNwGP14AaABAg)*

не понятно, например, в IsLooselyEqual попадают два объекта, то Sametype вернет true  (так как два объекта подпадают под пункт - 8. If x is an Object and y is an Object, return true), а затем вызовет IsStrictEqual, который в первом пункте вызывает тоже самое 1. If SameType(x, y) is false, return false. , но поскольку у нас не вернется false, то мы попадает в третий пункт - 3. Return SameValueNonNumber(x, y). Нажимаем на него и нам подходит первый пункт - 1. Assert: SameType(x, y) is true.
То что получается? он вызывает Sametype три раза в разных функциях? зачем?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[18.04.2025 22:00](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=UgwZaQTsODV9HgNwGP14AaABAg.AF2gTpkUqhCAH49WRnZvFY)*

> Спецификацию пишут люди, которые описывают нормы языка. 
> Не в их компетенции пояснять и понимать: 
> 1) как это сделать так чтобы алгоритм работал оптимально;
> 2) приведенное описание можно было оптимизировать вообще.
> 
> В их компетенции дать эталонную реализацию, с результатом работы которой, авторы Агентов, будут сравнивать работу их кода.

---

**[@gen7891](https://www.youtube.com/channel/UCEoNAGhXCHIH5g5Z8U-YC0w)** *[10.10.2025 18:23](https://www.youtube.com/watch?v=KMrVKtVrJ3Q&lc=UgxHhWrYTgAnjgkNKrV4AaABAg)*

Соведущий заколебал в фоне бармотать че-то...

---
