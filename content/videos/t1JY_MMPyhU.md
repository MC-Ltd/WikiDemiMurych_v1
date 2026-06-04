---
title: "⎡razbor:15⎦ Разбор видео: Let и Const диссиденты в языке JavaScript"
date: 2025-01-28
tags: []
videoId: "t1JY_MMPyhU"
duration: "4:31:31"
views: 4970
likes: 189
comments: 32
---
# [⎡razbor:15⎦ Разбор видео: Let и Const диссиденты в языке JavaScript](https://www.youtube.com/watch?v=t1JY_MMPyhU)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 28.01.2025 00:42  
**Тривалість:** 4:31:31  
**Перегляди:** 4970 · **Лайки:** 189 · **Коментарі:** 32
![thumbnail](https://i.ytimg.com/vi/t1JY_MMPyhU/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=t1JY_MMPyhU)
## Коментарі (12 · відповідей: 20)

**[@RTFMurych](https://www.youtube.com/channel/UC3NVT782r84UDLdx9JXtbow)** *[28.01.2025 00:33](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgzObcWkm0bCbYfWQqt4AaABAg) · 👍 11*

Достали эти новомодные шортсы — даёшь полноценный стрим по главам книги!

---

**[@IvanNovitskii](https://www.youtube.com/channel/UCwgs3cVW52cmxnDTa8uUa4g)** *[28.01.2025 01:04](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwxG7dCDBAZ7WE0B8F4AaABAg) (ред. 28.01.2025 01:07) · 👍 1*

я вам рекомндую всеже перепроверить свои тесты. сравните перфоманс этих четрыех скриптов. основной косяк в том, что мы использовали не локальные переменные функции, а не в let vs var
1)
function foo(){
  function abc() {       
    let a = 1;
    let acc = 0;
    for (var i = 0; i < 10000000; i++){
        acc += a;
        a++;
    };
  }
  abc();
}
2)
function foo1(){
  function abc() {       
    var a = 1;
    var acc = 0;
    for (var i = 0; i < 10000000; i++){
        acc += a;
        a++;
    };
  }
  abc();
}
3)
function bar(){
  let a = 1;
  let acc = 0;
  function abc() {       
    for (var i = 0; i < 10000000; i++){
        acc += a;
        a++;
    };
  }
  abc();
}
4)
function bar1(){
  var a = 1;
  var acc = 0;
  function abc() {       
    for (var i = 0; i < 10000000; i++){
        acc += a;
        a++;
    };
  }
  abc();
}

> **[@SerzhNesteruk](https://www.youtube.com/channel/UCvSxoIuRvinnq_mbU2KDTPA)** *[28.01.2025 02:09](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwxG7dCDBAZ7WE0B8F4AaABAg.ADov6wpwFn_ADp1_dLqlIm) (ред. 28.01.2025 11:52)*

> Тесты для таких функций дают уже более адекватный результат. 👌 Любопытно, что между функциями foo1 и bar1 колоссальная разница в производительности, хотя в обоих случаях у нас используется только var.

> **[@xclonikx](https://www.youtube.com/channel/UC7Ezu12Jsg1ZVzSiNzgvEiA)** *[28.01.2025 09:00](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwxG7dCDBAZ7WE0B8F4AaABAg.ADov6wpwFn_ADplbHWXPFV)*

> Your tests are weird. They are all using "var" in the "for" loop. The only difference is the first variable declarations, that's why they are almost identical performance wise.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[29.01.2025 23:46](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwxG7dCDBAZ7WE0B8F4AaABAg.ADov6wpwFn_ADtvosxvUY2)*

> Уже все перепроверено и не мной.
> Смотрите видео про жирную точку, и идите спорить с разработчиками Angular или typeScript которые говорят то, что говорил я. Ну или на худой конец к инженерам V8. Которое потратили пол года на то, что бы уменьшить издержки binding для let и const на 5%. Чем сильно стали гордиться.
> 
> Вопрос закрыт после того, как инженеры V8 стали оптимизировать под решение этой проблемы. Дальше можно со мной уже не дискутировать верно? Идите доказывайте им что они  неправы.

> **[@IvanNovitskii](https://www.youtube.com/channel/UCwgs3cVW52cmxnDTa8uUa4g)** *[29.01.2025 23:50](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwxG7dCDBAZ7WE0B8F4AaABAg.ADov6wpwFn_ADtwIRhaS9v) (ред. 29.01.2025 23:51) · 👍 1*

> @AsForJS  ну вы жжёте я сказал что тест вы проводили не верно

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[01.02.2025 06:57](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwxG7dCDBAZ7WE0B8F4AaABAg.ADov6wpwFn_ADzqh4ddK5s)*

> Смотри видео про жирную точку в споре о вар лет и конст.
> 
> После чего с удовольствием понаблюдаю как вы будете спорить с инженерами v8

> **[@IvanNovitskii](https://www.youtube.com/channel/UCwgs3cVW52cmxnDTa8uUa4g)** *[01.02.2025 10:29](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwxG7dCDBAZ7WE0B8F4AaABAg.ADov6wpwFn_AE-E-RI8cVl) (ред. 01.02.2025 11:36) · 👍 1*

> @demimurych1 это какая-то странная шутка?
> Я в комментариях на стриме, в комментариях под вторым видео прямо говорю, что считаю что let никак не может работать быстрее var. В целом по большей части, я согласен с выводами второго видео.
> Данный комментарий говорит о неверно проведенном тесте на этом видео. Поэтому ваши комментарии идти и с кем-то спорить, я считаю неуместными.

---

**[@SerzhNesteruk](https://www.youtube.com/channel/UCvSxoIuRvinnq_mbU2KDTPA)** *[28.01.2025 01:30](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgzXUV-PilS4CwltUuN4AaABAg) · 👍 4*

Тесты сравнения быстродействия var и let/const очень неочевидны (не даром даже Мурыч в них запутался), неубедительны, а возможно даже некорректны. Данные тесты показывают, что эффективнее из функции использовать локальные идентификаторы (а не внешние). Но разве, когда мы используем let/const, то в обязательном порядке делаем это во внешнем окружении функции? 🤷‍♂️ Как эти тесты показывают отличия быстродействия var от let/const, если и var, и let, и const есть в обоих случаях? Догадываюсь, что никак. 😒

> **[@SerzhNesteruk](https://www.youtube.com/channel/UCvSxoIuRvinnq_mbU2KDTPA)** *[28.01.2025 01:38](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgzXUV-PilS4CwltUuN4AaABAg.ADoy8MPOI7yADoyz5lRn3I) · 👍 1*

> Разница в быстродействии с заменой let на var конечно же есть, но она довольно небольшая, выигрыш может составить до 5%. И такие тесты Мурыч уже проводил ранее. Но видимо 5% показалось очень мало, поэтому придуман код, где разница будет до 40%. И не важно, что он показывает совсем не то, что мы якобы тестируем. Главное вовсе не корректность тестов, а ошеломляющий эффект на неискушенную публику: "+40% быстродействия просто при использовании var... WOW😱" 🤦‍♂️

> **[@SerzhNesteruk](https://www.youtube.com/channel/UCvSxoIuRvinnq_mbU2KDTPA)** *[29.01.2025 19:06](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgzXUV-PilS4CwltUuN4AaABAg.ADoy8MPOI7yADtQjmQPymd)*

> Update: Примерно через полчаса после этих комментариев автор видео всё-таки провёл корректные тесты в "Дополнении" к этому разбору (видео [razbor:15.1]). Посему озвученные претензии снимаются.🫡

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[01.02.2025 06:56](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgzXUV-PilS4CwltUuN4AaABAg.ADoy8MPOI7yADzqaa5MLeD)*

> Смотри видео на 8 минут, про жирную точку в споре о вар лет и конст.

> **[@SerzhNesteruk](https://www.youtube.com/channel/UCvSxoIuRvinnq_mbU2KDTPA)** *[01.02.2025 10:30](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgzXUV-PilS4CwltUuN4AaABAg.ADoy8MPOI7yAE-E6n9XjNR)*

> @demimurych1 Спасибо) Мне на эту тему очень понравилось ваше 32-секундное видео "Почему все неправильно используют var, let и const...".👍🙃

---

**[@tashchan](https://www.youtube.com/channel/UCcnSv2i3rBPSpdE98aGffvQ)** *[28.01.2025 10:00](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgysUfQHdPj9hfvkj314AaABAg) · 👍 4*

Мам я в телевизоре 😁

---

**[@dimacomedy](https://www.youtube.com/channel/UCP7rCV63QQfG8Fw4HpDMrOQ)** *[29.01.2025 16:24](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgyhHMQ-nVcZ8uqa2JF4AaABAg) · 👍 1*

"Развлекательный кантент" на 4 часика подъехал :)))

---

**[@SerzhNesteruk](https://www.youtube.com/channel/UCvSxoIuRvinnq_mbU2KDTPA)** *[30.01.2025 00:36](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwAuSm5GqOr2O0EJH54AaABAg) · 👍 1*

Утверждения Мурыча о том, что гугловский стайл гайд не запрещает использовать ключевое слово `var`, к сожалению, не соответствуют действительности. 🙅‍♂️

В английском языке одни и те же слова нередко могут истолковываться по-разному, но чтобы избежать каких-либо разночтений и неверных толкований, в Google JavaScript Style Guide (пункт 1.1) используется стандарт RFC2119, который строго регламентирует применение и трактовку слов "must", "must not", "required", "shall", "shall not", "should", "should not", etc.
Так вот, предложение "The var keyword must not be used." из пункта 5.1.1 не может быть истолковано иначе, как полный запрет на использование ключевого слова `var`. И только лишь тогда (и только тогда!), когда современный синтаксис ES6+ недоступен, то использование `var` считается допустимым (пункт 9.4.1) наряду с объектом `arguments`, который имеет статус 'deprecated'.

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[01.02.2025 06:54](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwAuSm5GqOr2O0EJH54AaABAg.ADu0_MB9KNdADzqQOJG0qk)*

> Там ключевое слово - local

> **[@SerzhNesteruk](https://www.youtube.com/channel/UCvSxoIuRvinnq_mbU2KDTPA)** *[01.02.2025 11:39](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwAuSm5GqOr2O0EJH54AaABAg.ADu0_MB9KNdAE-M0jQlbwe)*

> @demimurych1 В пункте 5.1.1 руководство от гугла настоятельно рекомендует всегда использовать let/const, чтобы объявляемые переменные были локальными. А в последнем предложении полностью запрещает использование ключевого слова `var`, нет там никакого "local". Если бы использование `var` не было бы запрещено, то в специальном разрешении на его использование для устаревшего синтаксиса (пункт 9.4.1) отсутствовал бы всякий смысл. 🤷‍♂️

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[03.02.2025 04:28](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwAuSm5GqOr2O0EJH54AaABAg.ADu0_MB9KNdAE3jCuC6oIG)*

> @SerzhNesteruk Читай название раздела - Local variable declarations. Если непонятно по названию раздела, открывай Style Guide JavaScript а не Style Guide TypeScript и читай:
> Declare all local variables with either const or let.

> **[@SerzhNesteruk](https://www.youtube.com/channel/UCvSxoIuRvinnq_mbU2KDTPA)** *[03.02.2025 11:08](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwAuSm5GqOr2O0EJH54AaABAg.ADu0_MB9KNdAE4S0qKj6-q)*

> @demimurych1 Допустим, вы правы. Но вы ведь сами неоднократно (и вполне справедливо) призывали не писать код в глобальном окружении, а оборачивать его хотя бы в самовызываемую функцию. Ну, а любая переменная, объявленная внутри функции, даже с ключевым словом var, уже является не глобальной, а именно локальной (local). И исходя из вашей же цитаты стайл гайда, для объявления локальных переменных нужно использовать исключительно const или let.

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[03.02.2025 22:57](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwAuSm5GqOr2O0EJH54AaABAg.ADu0_MB9KNdAE5iCYQM40v)*

> @SerzhNesteruk Global Environment в JavaScript это не тоже самое, что и отношение между локальными и глобальными переменными. Global Environment в JavaScript - это особое окружение со своими особыми правилами поведения, зафиксированные в спецификации. 
> Когда я говорю, выносите код за пределы Global Environment, я опираюсь именно на эти особенности поведения. 
> 
> Далее. 
> let a=1;
> function bFunc() {
>     let b=2;
>         return function cFunc() {
>              let c=3
>         } 
> }
> 
> bFunc()();
> 
> Для cFunc, локальной переменной является переменная "c". Переменные b и a для нее являются глобальными
> Для функции bFunc глобальной переменной является только переменная a. при этом переменная b является локальной для своего окружения bFunc.
> 
> Далее.
> Я всегда говорил и повторяю, для локального окружения, использование var/let/const идентичны по издержкам в случае RunTime Semantics.
> Разница появляется только тогда когда используется let const в локальном окружении в то время, когда обьявлены они в глобальном (внешнем).
> 
> function doExampleWhereAllFineWithLet() {
>    function doCalculateCirlceArea( theRadius ) {
>        const PI = 3.14;
>        let thePower = 2;
>        return PI * theRadius ** thePower;
>    }
>    doCalculateCirlceArea( 10 );
> }
> doExampleWhereAllFineWithLet();
> 
> Оба идентификатора( thePI, thePower ), используются только в том функциональном окружении, в котором они заявлены. 
> Производительность этого кода будет на 100% идентична случаю, если бы мы вместо let/const использовали var.
> 
> Детальнее в телеграмме https://t.me/AsForJavaScript/665

---

**[@Alex-p6x9x](https://www.youtube.com/channel/UC3ecJ5ifc7mnWd5qF4lE6vg)** *[31.01.2025 08:15](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgzTl29-dYgRv0xAmJJ4AaABAg)*

Дет-пирдет на столько старый, что видел плоскую землю! 😊

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[01.02.2025 06:54](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgzTl29-dYgRv0xAmJJ4AaABAg.ADxPt3TMfXMADzqLKlmESs)*

> в гробу он ее видел

---

**[@Alex-p6x9x](https://www.youtube.com/channel/UC3ecJ5ifc7mnWd5qF4lE6vg)** *[31.01.2025 08:21](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwY8h_p8qtURvsoUy54AaABAg)*

Ув. Мурычь, скажите свое мнение о сайте mdn. На сколько их изложение, соответствуют спецификации.

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[01.02.2025 06:55](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwY8h_p8qtURvsoUy54AaABAg.ADxQXC4wrkmADzqWkEUgH8) · 👍 3*

> Англискую версию уже около года активно приводят в порядок.
> 
> Ру версия - ужасна.

---

**[@Alex-p6x9x](https://www.youtube.com/channel/UC3ecJ5ifc7mnWd5qF4lE6vg)** *[03.02.2025 08:58](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=Ugwo_wl0kJuNrZU5_Xx4AaABAg) (ред. 03.02.2025 09:46)*

Ув. Мурычь связи с тем, что люди разные и воспреятие у всех разное, поэтому не все примеры для когото будут понятны. Мой вам совет, если можно сильно не циклитесть что вас не понимают. А лучше прсторайтесь на каждую сииуацию создать разные примеры. 
Как вариант
1 дать кусок спецификации (технический вариант)
2 логический вариан (возможно блок схема или что то другое) 
3 обстракный вариант (как пример с бананами) 
4 какой-то миф
Я не чего не утверждаю, но уневерсально для всех людей у вас врядли получится. 
С нетерпением ждем Вашу книгу! И конечно будем ее хейтить!,😊

---

**[@diniszabrodsky8508](https://www.youtube.com/channel/UCkO7hEGdqVb-PPRUbU3pdJg)** *[05.02.2025 09:47](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwUQmh37DmgEWDvscl4AaABAg)*

тільки тут з приклада випливає, що не var в цілому швидший, а що якщо він знаходиться в середині функції або іншої області видимості він стає швидшим. Цікаво було б подивитись як би вели себе чисто let, const і var  в подібних умовах

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[06.02.2025 02:57](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwUQmh37DmgEWDvscl4AaABAg.AE9SLtLy5tTAEBICvUk7rt)*

> На телеграм канале привязанном к этому, есть публикации примеров с пояснениями https://t.me/AsForJavaScript/665

---

**[@Артем-в9э9щ](https://www.youtube.com/channel/UC1DWehEZ271S_0ePh7XHouA)** *[05.02.2025 11:46](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwF787RJqMhz6Us94d4AaABAg)*

Объясни логику видосов по 4 часа. Ведь если ты уверен, что знаешь спецификацию или можешь ее объяснить, ты бы мог по каждой спорной теме просто создавать видео и объяснять. Это же лучше для сообщества, чем смотреть чье-то видео и прицепляться к каждой мелочи.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[06.02.2025 02:56](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgwF787RJqMhz6Us94d4AaABAg.AE9ezC8idjqAEBI7qqFwTi) · 👍 1*

> Чтобы записать видео, нужно много работать над сценарием. Текстом. И т.д.
> Мне не нравиться это делать.
> 
> При этом, если писать все это сразу онлайн, выходят вот такие монстры по 4 часа, но у них есть преимущество - фиксируют живого человека, со всеми аго ошибками и идиотизмами.
> 
> Та абсолютно прав в том, что для окружающих, было бы лучше все это сжимать до 15 минут.  Я это понимаю. Иногда (из 167 видео есть 3) у меня получается.

---

**[@Артем-в9э9щ](https://www.youtube.com/channel/UC1DWehEZ271S_0ePh7XHouA)** *[05.02.2025 13:16](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgzKugsIStXeYMf64GV4AaABAg)*

Если честно, в итоге не понял как правильно делать. Понял что глобально не желательно использовать var, так как происходит запись в глоальный объект, но в том числе let\const то же нужно использовать в блочном окружении, так как на уровне байтов ( забыл как называется ) на каждый лет и конст дополнительная обертка идет ThrowRefferenceErrorIfHole. Так а что в итоге в глобальном окружении использовать ?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[06.02.2025 02:54](https://www.youtube.com/watch?v=t1JY_MMPyhU&lc=UgzKugsIStXeYMf64GV4AaABAg.AE9pJ14JfkdAEBHqEONSPj) · 👍 1*

> В телеграме на канале который привязан к этому каналу, есть пост с примерами.
> Вот ссылка https://t.me/AsForJavaScript/665

---
