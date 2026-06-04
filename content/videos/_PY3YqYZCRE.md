---
title: "Существует ли приведение типа в JavaScript"
date: 2025-02-16
tags: ["spec", "7", "js", "ecma", "type", "conversion"]
videoId: "_PY3YqYZCRE"
duration: "6:51:01"
views: 5617
likes: 159
comments: 9
---
# [Существует ли приведение типа в JavaScript](https://www.youtube.com/watch?v=_PY3YqYZCRE)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 16.02.2025 02:07  
**Тривалість:** 6:51:01  
**Перегляди:** 5617 · **Лайки:** 159 · **Коментарі:** 9
![thumbnail](https://i.ytimg.com/vi/_PY3YqYZCRE/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=_PY3YqYZCRE)
## Коментарі (8 · відповідей: 1)

**[@RTFMurych](https://www.youtube.com/channel/UC3NVT782r84UDLdx9JXtbow)** *[16.02.2025 07:20](https://www.youtube.com/watch?v=_PY3YqYZCRE&lc=Ugz1fvrNxZgC95w1Xi54AaABAg) · 👍 1*

lgo-go! — «У самурая нет цели, только путь…»

---

**[@freetimeproject7](https://www.youtube.com/channel/UCIs3LkRqUzrBa90Wf4eknTQ)** *[16.02.2025 11:31](https://www.youtube.com/watch?v=_PY3YqYZCRE&lc=UgyfYUbJqAy-0e6HnC94AaABAg) · 👍 3*

джаваскрипт - очень милое приведение....типа)

---

**[@boycovclub](https://www.youtube.com/channel/UCxbDPizEG96FDSCQ8JFpFRA)** *[16.02.2025 18:31](https://www.youtube.com/watch?v=_PY3YqYZCRE&lc=Ugz8t6lBupQd2ZCm4Y54AaABAg)*

Мурыч прокомметируй такое монадическое поведение в композиции функций без создания типов Монад
// Супер пайп
const pipe = (...fns) => (defaultValue) => (value) =>
    fns.reduce((acc, fn) => {
        switch (true) {
            case acc == null: // Если null или undefined – возвращаем defaultValue
                return defaultValue;
            case acc instanceof Promise: // Если Promise – вызываем .then(fn)
                return acc.then(fn);
            default: // Обычный случай
                return fn(acc);
        }
    }, value);

// Если подключить еще каррирование нижних функций то будет суперски
const syncFn = (x) => x + 1;
const asyncFn = async (x) => x * 2;
const nullFn = () => null;
const undefinedFn = () => undefined;
const logFn = (x) => { console.log(x); return x; };

const pipeline = pipe(syncFn, asyncFn, logFn); // создаем пайп

console.log(pipeline('Default Value')(5)); // (5 + 1) * 2 -> 12 (лог в консоль)
console.log(pipeline('Default Value')(null)); // null -> 'Default Value'
console.log(pipeline('Default Value')(undefined)); // undefined -> 'Default Value'
console.log(pipeline('Default Value')(10)); // (10 + 1) * 2 -> 22 (лог в консоль)

> **[@boycovclub](https://www.youtube.com/channel/UCxbDPizEG96FDSCQ8JFpFRA)** *[16.02.2025 18:40](https://www.youtube.com/watch?v=_PY3YqYZCRE&lc=Ugz8t6lBupQd2ZCm4Y54AaABAg.AEbi0E0WbQHAEbj4b31tdj)*

> или более совершенная версия без проброса дальше по композиции
> const pipe = (...fns) => (defaultValue) => (value) => {
>     let stopped = false; // Флаг остановки цепочки
> 
>     return fns.reduce((acc, fn) => {
>         if (stopped) return acc; // Если цепочка остановлена, просто возвращаем текущее значение
> 
>         switch (true) {
>             case acc == null: // Если null или undefined – возвращаем defaultValue и останавливаем цепочку
>                 stopped = true;
>                 return defaultValue;
>             case acc instanceof Promise: // Если Promise – вызываем .then(fn)
>                 return acc.then(fn);
>             default: // Обычный случай
>                 return fn(acc);
>         }
>     }, value);
> };

---

**[@ArtemMindsurfer](https://www.youtube.com/channel/UCtApnkzZe-Bo6ZQd5CHeJXQ)** *[19.02.2025 07:48](https://www.youtube.com/watch?v=_PY3YqYZCRE&lc=UgxRQTdyh_F5rBo07f94AaABAg) · 👍 3*

wow я ждал этого многие месяцы!

---

**[@MaxNadeev](https://www.youtube.com/channel/UCmvcgVfOCDhe8V3yGtEQGtg)** *[20.06.2025 22:32](https://www.youtube.com/watch?v=_PY3YqYZCRE&lc=UgxtvAawUCF97yATAWB4AaABAg)*

Годнота

---

**[@kowkavn2356](https://www.youtube.com/channel/UCaCYq3PjfpFeCpZT0xciyfQ)** *[22.10.2025 22:58](https://www.youtube.com/watch?v=_PY3YqYZCRE&lc=UgxncqgQgWj7artMdiV4AaABAg) · 👍 1*

2:10 Суть проблемы
6:00 Начало 
7:30 string+number
14:40 Любимый пример мурыча
17:24 Неправильно восприятие && оператора
25:06 Аналогичный пример с ||
32:23 isNaN и Number.isNaN
57:30 Пример от слушателя 0 < true
1:01:01 Пример "ё" < "я"
1:11:00 Продолжается громкое обсуждение кто как думал при изучении js о приведении типов
~1:17:00 Про то что джун должен знать идеально js
~1:20:00 Обсуждение что кому задавали на собеседовании
1:22:04  { valueOf: () => 11 } + { valueOf: () => 1 } или почему нужно ставить скобочки
1:39:50  Участники беседы начали рассуждать про задачу выше
1:44:29 Догадки по решению задачи выше
1:48:07 Объяснение решения задачи выше 
1:52:30 Пример с инкрементом строки "5" 
2:19:40 Проблема 5 + 5
2:39:20 О различии между интерпетацией и компиляцией
3:25:25 в js Внутренний объект не часть внешнего объекта  
3:27:29 Питон умрёт (5-7 лет)
3:31:58 Почему Питон используется 
3:35:12 Точка зрения определяется точкой сидения 
3:45:10 "В то время когда поляне и древляне..." или куда делись Помпеи
3:48:05 история скандинавов и викингов...  // шёл 3 час стрима про js 
3:49:28 Один не бог? 
3:52:10 Упоминание Сериала "Викинги"  
3:56:38 Астероид, Целители или почему не отращивают конечности
4:05:07 Про черную дыру 
4:07:48 Работа с языком js должна вызывать ...
4:12:40 Регулярки, задача получить все слова в предложении
4:34:31 Все говорят что php говно и я скажу
4:38:10 Пример кода из чата  а++ == ++а и тд
4:39:40 Про Performance API
4:47:30 Про опыт и опыт мурыча 
4:52:30 Когда у кого появился интернет и компьютер
5:08:20 (Рассуждения) Зачем нужен Докер?
5:35:49 Сборщик мусора это HR
6:49:57 Живите счастливо

---

**[@miarur](https://www.youtube.com/channel/UCNJRDBE-uLQ8r7wteq1_cIg)** *[03.11.2025 18:28](https://www.youtube.com/watch?v=_PY3YqYZCRE&lc=UgwfiZ7woxXsw6iyr814AaABAg)*

спасибо за полезную информацию!

---

**[@suleymanbasir6347](https://www.youtube.com/channel/UCGEXnKnHvtzFcszXEyBo7Dw)** *[29.05.2026 10:47](https://www.youtube.com/watch?v=_PY3YqYZCRE&lc=Ugxn1M1WviFn39RjApR4AaABAg)*

1:03:16 

2. Почему с буквой "ё" всё пошло не так?Когда в международную таблицу Юникод добавляли кириллицу (русские буквы), основной блок букв от "а" до "я" записали строго по порядку (от кода 1072 до 1103).Но букву "ё" добавили в таблицу позже всех остальных, отдельно! Для неё просто не осталось места внутри основного алфавитного ряда. В итоге её код оказался в самом конце, далеко за буквой "я".Посмотрите на их реальные коды в компьютере:Буква "а" = код 1072Буква "б" = код 1073...Буква "я" = код 1103 (самый конец основного блока)Буква "ё" = код 1105 (вынесена отдельно в конец)Поэтому, когда вы пишете "ё" > "я", JavaScript снова просто сравнивает два числа под капотом: 1105 > 1103. Математически это true, поэтому компьютер считает, что "ё" больше.

ETO OTVET CHATGPT

---
