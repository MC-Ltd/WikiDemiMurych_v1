---
title: "⎡coding:14⎦ LeetCode: Решаем hard задачи, отвечаем на вопросы."
date: 2023-11-29
tags: []
videoId: "oDUPhZuyam0"
duration: "4:51:25"
views: 6952
likes: 224
comments: 13
---
# [⎡coding:14⎦ LeetCode: Решаем hard задачи, отвечаем на вопросы.](https://www.youtube.com/watch?v=oDUPhZuyam0)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 29.11.2023 03:11  
**Тривалість:** 4:51:25  
**Перегляди:** 6952 · **Лайки:** 224 · **Коментарі:** 13
![thumbnail](https://i.ytimg.com/vi/oDUPhZuyam0/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=oDUPhZuyam0)
## Коментарі (7 · відповідей: 6)

**[@i-gogo](https://www.youtube.com/channel/UCK68X6lmP68O8NxSOiToMjA)** *[29.11.2023 04:05](https://www.youtube.com/watch?v=oDUPhZuyam0&lc=UgwoEG0vjshJJdQzTtd4AaABAg) · 👍 1*

при всём уважении к автору, но хотелось бы примеров как JS делает жизнь лучше…

А то — «учите самый простой язык в мире, чтобы сделать вашу жизнь максимально эффективной» но… столько часов негодования на реализацию чата YouTube во всем YouTube не найдёшь.

Максим, распарсите его уже в любом удобном для Вас виде…

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[30.11.2023 23:16](https://www.youtube.com/watch?v=oDUPhZuyam0&lc=UgwoEG0vjshJJdQzTtd4AaABAg.9xgKBv0nQYS9xkxlGUsiw3)*

> Относительно чата и моего негодования. Случилось оно в той форме именно потому, что обьем сообщений в чате стал больше привычного. 
> 
> До этого, проблема была не так очевидна, как следствие и негодование так же.
> 
> Я обычный человек, который имеет право на обычные слабости - если чат скачет что конь, я могу как тот самый конь с него поржать.
> 
> Одновременно с этим, у меня есть масса более важных задач, на которые не хватает времени. То есть задач которые более приоритетны чем писать парсер для чата YouTube.
> 
> Например ответить на Ваш комментарий, что я считаю более важным чем сидеть сейчас и разбираться с тем говном которое сделали программисты этого сервиса. 
> 
> С другой стороны, Вы возможно правы в том, что эффективнее было бы, не отвечать на комментарии, а показать всем код решения этой проблемы.

---

**[@ProJavaScript](https://www.youtube.com/channel/UCq5gKzOfiQxkDPvpo6wba_g)** *[29.11.2023 07:31](https://www.youtube.com/watch?v=oDUPhZuyam0&lc=UgztybYPcMdybN6skg94AaABAg) · 👍 1*

Добрый день.
Если хотите сложную задачу на особенности JavaScript, получите:
1. Нужно создать класс ProgressController наследник от нативного (встроенного в браузер - это важно) класса AbortController
2. У класса ProgressController, свойство signal должно быть экземпляром класса ProgressSignal, наследником от нативного (встроенного в браузер - это важно) класса AbortSignal
3. У классов ProgressController/ProgressSignal должны быть как свои методы и свойства, так и нативные
4. Свойство `new ProgressController().signal` должно быть совместимым с нативным API типа `fetch`, чтобы можно быть вызвать `ProgressController#abort()` и прервать запрос `fetch`

Эта задача чисто на JS. На других языках она будет решать совершенно по-другому.

Наивная структура классов будет выглядеть так:
```
class ProgressSignal extends AbortSignal {
    test(){ return 123 }
}
class ProgressController extends AbortController {
    constructor(){
        super();
        this.signal = new ProgressSignal();
    }
    test(){ return 1 }
}
```
Если что, решение у этой задачи есть (без подмены глобального нативного AbortController), так чтобы:
```
((new ProgressController()) instanceof AbortController) === true;
((new ProgressController()) instanceof ProgressController) === true;
((new ProgressController()).signal instanceof AbortSignal) === true;
((new ProgressController()).signal instanceof ProgressSignal) === true;
```

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[30.11.2023 23:08](https://www.youtube.com/watch?v=oDUPhZuyam0&lc=UgztybYPcMdybN6skg94AaABAg.9xggncqYcGS9xkwr-XpGhd)*

> Ваша задача не имеет никакого отношения к JavaScript.
> Она спекулирует на особенностях внешнего API Host среды. 
> 
> Ее можно переписать удалив из нее такие части как: ProgressController, AbortController etc...
> 
> Если Вам интересно как я буду позориться решая Вашу задачу, и вы готовы к прямому эфиру - то напишите мне в телеграмм. 
> 
> Мы договоримся о времени и запишем то, что получится

> **[@ProJavaScript](https://www.youtube.com/channel/UCq5gKzOfiQxkDPvpo6wba_g)** *[01.12.2023 06:28](https://www.youtube.com/watch?v=oDUPhZuyam0&lc=UgztybYPcMdybN6skg94AaABAg.9xggncqYcGS9xljD35h8bW) (ред. 13.06.2024 21:31)*

> @AsForJS Безусловно, я напишу Вам в телеграм.
> Однако, для других читающих поясню некоторые моменты:
> 1. Эта задача именно про js (моё мнение), несмотря на то, что для примера используется внешнее API.
> 2. Эта проблема актуальна в некоторых других кейсах. Например, если мы хотим отнаследоваться от Date, но при этом транспилировать код в es5 (Babel будет ругаться, но рабочее решение есть) 
> 3. Решение этой задачи связано с особенностями системы наследования js, а не с конкретным API. 
> 4. У меня нет цели, чтобы Вы позорились. Просто интересны Ваши рассуждения и как Вы придёте к решению.

---

**[@san4es1690](https://www.youtube.com/channel/UC42aW1JCrYZelQA8wCE5JBw)** *[29.11.2023 07:42](https://www.youtube.com/watch?v=oDUPhZuyam0&lc=Ugyb17w9mQdI1a1L2bl4AaABAg)*

Отличный канал. Очень нравиться подача материала, правда 95% не понимаю :), так как совсем недавно в программировании. Огромное спасибо автору, за его труд. Странно что так мало лайков и комментариев.

---

**[@railbatyrshin](https://www.youtube.com/channel/UCJgVMi5XN33KoJSx1hQQJLQ)** *[29.11.2023 14:32](https://www.youtube.com/watch?v=oDUPhZuyam0&lc=Ugyzc9NZ9ievNXs--MR4AaABAg)*

А как вы сделали компилятор для жс, чтобы смотреть байт код?)

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[30.11.2023 22:56](https://www.youtube.com/watch?v=oDUPhZuyam0&lc=Ugyzc9NZ9ievNXs--MR4AaABAg.9xhRz6-HEuX9xkvSnvJxfN) · 👍 3*

> Я его не делал. Я воспользовался возможностями современного V8, который сам предоставляет опции для получения такого кода.
> 
> Короткий ответ на Ваш вопрос - следует использовать ключ коммандной строки:
>  --print-bytecode
> более подробный ответ скоро появиться в отдельном видео. 
> 
> Очень много людей попросили меня показать простым языком этот процесс. И я его запишу, возможно даже сегодня ночью.
> 
> Части всего этого процесса уже записывались в разных видео. Но так чтобы одним общим материалом нет. Я это сделаю, чтобы не писать постоянно много букв.

---

**[@frogkick2755](https://www.youtube.com/channel/UCLwnXOF4PbWp3HRM4hsbTVA)** *[29.11.2023 23:53](https://www.youtube.com/watch?v=oDUPhZuyam0&lc=UgwNoGqeR6M4IzATI9p4AaABAg)*

Всем хорошего кодинга
Посоветуйте материал для изучения JS в полной мере

---

**[@ksa-h2n](https://www.youtube.com/channel/UCejFmdJCpiE5QJk3sflv0jA)** *[01.12.2023 18:23](https://www.youtube.com/watch?v=oDUPhZuyam0&lc=UgzHLksiBo_t3fREZpF4AaABAg) · 👍 1*

3:32:12 битовые операции же быстрее. Сколько "стоит" преобразование числа к строке? не говоря о последующей регулярке. Тест в студию!

---

**[@Red_Coder](https://www.youtube.com/channel/UCKCzvAD4FAlkd4PKxEZJtSA)** *[19.12.2023 10:39](https://www.youtube.com/watch?v=oDUPhZuyam0&lc=UgxS1Z_3ghccjBGBSy54AaABAg)*

В React предполагается, что вы будете транспилировать код. Такой процесс устранит все виды деструктурирующего присваивания

> **[@Borodatenkiy](https://www.youtube.com/channel/UCn9e5iSKRX9jzixQesepLAw)** *[15.08.2024 20:12](https://www.youtube.com/watch?v=oDUPhZuyam0&lc=UgxS1Z_3ghccjBGBSy54AaABAg.9yVXBWXsP7XA7AXWTksN9D)*

> Об этом можно где-то прочесть? Если да, то дайте пожалуйста ссылку на ресурс. заранее спасибо!

> **[@Red_Coder](https://www.youtube.com/channel/UCKCzvAD4FAlkd4PKxEZJtSA)** *[25.08.2024 16:51](https://www.youtube.com/watch?v=oDUPhZuyam0&lc=UgxS1Z_3ghccjBGBSy54AaABAg.9yVXBWXsP7XA7ZvTu33FyF)*

> @Borodatenkiy скорее всего в блоге одного из разоаботчиков библиотеки - Абрамов

---
