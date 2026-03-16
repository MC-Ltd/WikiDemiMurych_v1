---
title: "⎡talks:14⎦ Отвечаю на комментарии, оставленные под предыдущими стримами"
date: 2024-01-07
tags: []
videoId: "xpFPhMERCLc"
duration: "3:10:51"
views: 2996
likes: 89
comments: 9
---
# [⎡talks:14⎦ Отвечаю на комментарии, оставленные под предыдущими стримами](https://www.youtube.com/watch?v=xpFPhMERCLc)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 07.01.2024 13:04  
**Тривалість:** 3:10:51  
**Перегляди:** 2996 · **Лайки:** 89 · **Коментарі:** 9
![thumbnail](https://i.ytimg.com/vi/xpFPhMERCLc/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=xpFPhMERCLc)
## Коментарі (2 · відповідей: 7)

**[@jean_zfc](https://www.youtube.com/channel/UC_GbATs4nUTnXLrvO9NpWTQ)** *[07.01.2024 04:13](https://www.youtube.com/watch?v=xpFPhMERCLc&lc=UgxNe4wQSqEW7hYqs4x4AaABAg)*

Название не соответствует содержанию 🙃

> **[@goodgamer2720](https://www.youtube.com/channel/UCMh8m7jG_19dWozK3cSSCHw)** *[07.01.2024 10:15](https://www.youtube.com/watch?v=xpFPhMERCLc&lc=UgxNe4wQSqEW7hYqs4x4AaABAg.9zFl4uSu3D29zGPZ6XA3W_)*

> а какое должно быть?

---

**[@cafedead](https://www.youtube.com/channel/UCBY5cq_88gH_6MnMAnVM_hA)** *[07.01.2024 17:13](https://www.youtube.com/watch?v=xpFPhMERCLc&lc=UgzqJabYL6e4l9UjEAV4AaABAg) (ред. 14.09.2024 14:04) · 👍 3*

Я затестил в рантайме варианты решения FizzBuzz участников 1, 2 и 4 от Яндекса, твое, и свое решения. Вот результаты на 691200 элементах массива. Твой код работает хуже всех, а не лучше, как ты утверждаешь. Не нужно хамить прямо на стримах незнакомым людям, которым ты, очевидно, проигрываешь. Нужно уметь признавать свои ошибки.

Мое решение на Свич-кейсах лучше всех, на втором месте решение лысого мужчины, записывающего по 21 элементу в массив. Я прогнозировал на 50% более долгое исполнение твоего кода из-за трех циклов, но все оказалось еще хуже. Моему решению оно проигрывает в 10 раз. Таким образом, я даже могу себе позволить и квадратными скобками массив проинициализировать, пушить в него, и деление делать, сколько душе угодно.

Твой код можно немного поправить, это даст заметный прирост.

--- 
Yandex #1 Shortmen Done After 44ms
Yandex #2 Girl Done After 30ms
Yandex #4 Bald Man Done After 15ms
Murych Done After 120ms
Michael Done After 12ms
--- 
Yandex #1 Shortmen Done After 63ms
Yandex #2 Girl Done After 84ms
Yandex #4 Bald Man Done After 11ms
Murych Done After 124ms
Michael Done After 12ms
--- 
Yandex #1 Shortmen Done After 32ms
Yandex #2 Girl Done After 27ms
Yandex #4 Bald Man Done After 22ms
Murych Done After 127ms
Michael Done After 13ms
--- 
Yandex #1 Shortmen Done After 35ms
Yandex #2 Girl Done After 19ms
Yandex #4 Bald Man Done After 14ms
Murych Done After 113ms
Michael Done After 9ms
--- 
Yandex #1 Shortmen Done After 53ms
Yandex #2 Girl Done After 21ms
Yandex #4 Bald Man Done After 13ms
Murych Done After 117ms
Michael Done After 8ms
--- 
Yandex #1 Shortmen Done After 36ms
Yandex #2 Girl Done After 25ms
Yandex #4 Bald Man Done After 17ms
Murych Done After 144ms
Michael Done After 8ms
--- 
Yandex #1 Shortmen Done After 51ms
Yandex #2 Girl Done After 18ms
Yandex #4 Bald Man Done After 20ms
Murych Done After 123ms
Michael Done After 8ms
---

> **[@SerzhNesteruk](https://www.youtube.com/channel/UCvSxoIuRvinnq_mbU2KDTPA)** *[08.01.2024 23:13](https://www.youtube.com/watch?v=xpFPhMERCLc&lc=UgzqJabYL6e4l9UjEAV4AaABAg.9zH9N-P_pKE9zKNPyS2QeV)*

> Поделитесь, пожалуйста, своим вариантом решения. Любопытно взглянуть. 🤓 У меня, например, получился вот такой простенький вариант решения "в лоб" в императивном стиле:
> 
> const fizzBuzz = length => {
>         const resultArray = [];
>         for (let i = 0; i < length;) {
>             resultArray[i++] = (
>                 i % 21 === 0 ? 'FizzBuzz'
>                 : i % 3 === 0 ? 'Fizz'
>                 : i % 7 === 0 ? 'Buzz'
>                 : i
>             );
>         }
>         return resultArray;
>     };
> 
> Тело цикла я потом, правда, чуть переделал:
>             resultArray[i++] = (
>                 (i % 3 === 0 ? 'Fizz' : '') +
>                 (i % 7 === 0 ? 'Buzz' : '')
>             ) || i;
> Код стал чуть более читаемым, но производительность изначального варианта (где больше проверок на кратность) почему-то была выше 🤔

> **[@SerzhNesteruk](https://www.youtube.com/channel/UCvSxoIuRvinnq_mbU2KDTPA)** *[21.01.2024 07:34](https://www.youtube.com/watch?v=xpFPhMERCLc&lc=UgzqJabYL6e4l9UjEAV4AaABAg.9zH9N-P_pKE9zpAF014JsA)*

> @cafedead Под решением на свич-кейсах вы имели в виду что-то в таком роде?
> 
>     const fizzBuzz = length => {
>         const result = [];
>         for (let i = 1; i <= length; i++) {
>             switch (i % 21) {
>                 case 0:
>                     result.push('FizzBuzz');
>                     break;
>                 case 3:
>                 case 6:
>                 case 9:
>                 case 12:
>                 case 15:
>                 case 18:
>                     result.push('Fizz');
>                     break;
>                 case 7:
>                 case 14:
>                     result.push('Buzz');
>                     break;
>                 default:
>                     result.push(i);
>             }
>         }
>         return result;
>     };

> **[@Watozarato](https://www.youtube.com/channel/UC0f-TKFbfRF_PaYbA95TkBA)** *[14.09.2024 13:08](https://www.youtube.com/watch?v=xpFPhMERCLc&lc=UgzqJabYL6e4l9UjEAV4AaABAg.9zH9N-P_pKEA8N0pssyVgi)*

> Чувак, ты логически осознаешь, что в обычных решениях на любой миллион элементов приходится 3 миллиона гребанных операций? В случае с тремя циклами количество операций падает почти на 30%, а то и выше. Три цикла быстрее все обработают гарантировано.

> **[@cafedead](https://www.youtube.com/channel/UCBY5cq_88gH_6MnMAnVM_hA)** *[14.09.2024 13:37](https://www.youtube.com/watch?v=xpFPhMERCLc&lc=UgzqJabYL6e4l9UjEAV4AaABAg.9zH9N-P_pKEA8N4ENM2GrQ) (ред. 14.09.2024 13:43)*

> @Watozarato чел, ты логически осознаешь, что я цифры привел?  Не надо тут про "гарантии", Мурыч как раз продемонстрировал, что гарантий никаких нет. Сам затести. Это вот если исправить решение Мурыча, тогда там что-то и заработает быстро, готов признать. Но количество операций с тремя циклами не падает, а наоборот растет. Опомнись. Дело не в этом... Дело в суммарном количестве условных переходов в решениях. Их меньше в варианте Мурыча, а в вариантах с кучей if их больше всех. Но для этого надо нормально писать, не косячить в других местах, сожрав этим всю выгоду.

> **[@cafedead](https://www.youtube.com/channel/UCBY5cq_88gH_6MnMAnVM_hA)** *[14.09.2024 13:52](https://www.youtube.com/watch?v=xpFPhMERCLc&lc=UgzqJabYL6e4l9UjEAV4AaABAg.9zH9N-P_pKEA8N5rrQ0mpW) (ред. 14.09.2024 14:19)*

> @Watozarato не гарантировано, раз у Мурыча получилась такая лажа. Я готов признать, что исправив решение Мурыча можно получить быстрое и правильное решение на 4-х циклах, и что мои прогнозы были не правильными, и вариант в действительности не тупиковый. Дело не в количестве операций, а в количестве условных переходов. Не знаю, как ты считаешь операции. Итераций в варианте с тремя циклами больше на 50%.

> **[@Watozarato](https://www.youtube.com/channel/UC0f-TKFbfRF_PaYbA95TkBA)** *[11.01.2026 09:13](https://www.youtube.com/watch?v=xpFPhMERCLc&lc=UgzqJabYL6e4l9UjEAV4AaABAg.9zH9N-P_pKEARprizmrG4s)*

> Жаль не помню детали задачи физбаза, поэтому написал что было в памяти на коленке
> function loop(array){
> 	for(var i=0; i<array.length; ++i){
> 		if(array[i]%3===0) array[i]="fizz";
> 		if(array[i]%7===0) array[i]="buzz";
> 		if(array[i]%11===0) array[i]="fizzbuzz";
> 	}
> 	return array;
> }
> function highLoop(array){
> 	for(var i=0; i<array.length; i+=3) array[i]="fizz";
> 	for(var i=0; i<array.length; i+=7) array[i]="buzz";
> 	for(var i=0; i<array.length; i+=11) array[i]="fizzbuzz";
> 	array[0]="fizz";
> 	return array;
> }
> var max=10;
> var length=2000000;
> 
> function create(max){
> 	var array=new Array(max);
> 	for(var i=0; i<max; ++i) array[i]=i;
> 	return array;
> }
> console.time("loop");
> for(var i=0; i<max; ++i){
> 	var array=create(length)
> 	loop(array);
> }
> console.timeEnd("loop");
> 
> console.time("high_loop");
> for(var i=0; i<max; ++i){
> 	var array=create(length)
> 	highLoop(array);
> }
> console.timeEnd("high_loop");
> Ой, всего-то 3 цикла в 5 раз быстрее работаю

---
