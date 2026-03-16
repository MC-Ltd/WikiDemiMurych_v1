---
title: "⎡msk⎦ JavaScript Destructuring Assignment или не все то золото что коротко пишется."
date: 2023-05-15
tags: []
videoId: "98mOkxRFHYA"
duration: "16:01"
views: 2071
likes: 190
comments: 23
---
# [⎡msk⎦ JavaScript Destructuring Assignment или не все то золото что коротко пишется.](https://www.youtube.com/watch?v=98mOkxRFHYA)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 15.05.2023 04:55  
**Тривалість:** 16:01  
**Перегляди:** 2071 · **Лайки:** 190 · **Коментарі:** 23
![thumbnail](https://i.ytimg.com/vi/98mOkxRFHYA/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=98mOkxRFHYA)
## Коментарі (14 · відповідей: 9)

**[@evgenstepanov6319](https://www.youtube.com/channel/UCtXFC6eD6hm5hyHbLmiTxxw)** *[15.05.2023 08:43](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgzlKtYMtkkYmD9jwaN4AaABAg) (ред. 15.05.2023 08:54) · 👍 1*

Правильно понимаю, что  если мы используем деструктуризацию через объект, к примеру const obj = {a: 1, b:2} преобразуя в  const {a, b} = obj, то в этом случае все отработает корректно, и простыня байт кода появляется только при использовании array assignment?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[16.05.2023 12:33](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgzlKtYMtkkYmD9jwaN4AaABAg.9pizbpY4pX79plyiYBwy-d) · 👍 4*

> Да. Именно так.
> Потому, что именно для ситуации использования конструкции, которая содержит [ ],  спецификацией определяется создания итератора. Вне зависимости от того, какого обьема данные, и что из них используется в нашей синтаксической конструкции.
> 
> То есть Вы абсолютно правы, когда говорите, что только в случае использования синтаксической конструкции, которая похожа на Array Literal балгодоря использованию квадратных скобок [] - всегда будет создан полноценный итератор, который характеризуется простыней кода.
> 
> Когда это понимаешь, то отдаешь себе отчет в том, чего стоит та или иная операция. 
> 
> Например я, никогда не использую Array Assignment Pattern, когда пишу код, который будет использован где-то и кем то. Но когда я хочу быстро решить какой-то вопрос для себя, например обработать список узлов на странице, которые возвращает document.querySelectorAll("div"), то я с удовольствием позволяют себе написать:
> [ ... document.querySelectorAll("div")].map ( [...] )
> 
> потому,  что это коротко, понятно, и нужно только мне, когда я знаю что готов подождать лишнюю секунду, лишь бы не давить лишние кнопки на клавиатуре.
> 
> Но если этот код пойдет куда-то и кому-то, то я никогда в жизни подобную конструкцию не напишу, потому, что мне будет стыдно за то потребление ресурсов, которое будет использовано подобным итератором. И подумаю над тем, как тот же код написать красивее.

> **[@evgenstepanov6319](https://www.youtube.com/channel/UCtXFC6eD6hm5hyHbLmiTxxw)** *[16.05.2023 12:40](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgzlKtYMtkkYmD9jwaN4AaABAg.9pizbpY4pX79plzVfyI3_Z)*

> @AsForJS спасибо за исчерпывающий ответ!

> **[@anishchenko](https://www.youtube.com/channel/UCB-qep9CiL7iZljv_fdNW8A)** *[17.05.2023 19:43](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgzlKtYMtkkYmD9jwaN4AaABAg.9pizbpY4pX79ppJkLUd-Mv)*

> @AsForJS  в видео Вы делаете акцент на том что надо использовать (указывать) именно ключи const {0:a, 1:b} = obj  я так понимаю ключевой момент именно в том чтоб указать ключ,  вместо такой записи const {a, b} = obj. или я не правильно понял?))  т.е. есть ли разница в форме записи  const {0:a, 1:b} = obj  или  const {a, b} = obj

> **[@ДмитрийНестерук-о1с](https://www.youtube.com/channel/UCXz3SCABrVJwBSvUOTq-T3A)** *[21.05.2023 19:55](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgzlKtYMtkkYmD9jwaN4AaABAg.9pizbpY4pX79pzdKoJP0IV) (ред. 13.06.2024 23:24)*

> @anishchenko а можна дестуктурувати масив таким чином : const {a, b} = obj? Чи ви відео не дивились?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[07.06.2023 01:03](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgzlKtYMtkkYmD9jwaN4AaABAg.9pizbpY4pX79qdOEHPK17p) · 👍 9*

> Разница в том какая синтаксическая конструкция используется. 
> Если это конструкция вида:
> var theArray = [1, 2, 3];
> var [a, b, c] = theArray;
> 
> то есть конструкция которая использует паттерн с квадратными скобками: то будет сгенерирован полноценный итератор ( полотенце кода).
> 
> Если же это паттерн с фигурными скобками: то такого сделано не будет.
> А что же произойдет когда мы напишем:
> var {a, b} = obj; 
> или 
> var {a, b} = theArr;
> 
> А произойдет следующее. 
> Для строки var {a, b} = obj; 
> строго в соответствии со спецификацией, будут созданы два идентифкатора a и b. Которые будут связаны со значением в том случае, если в obj есть ключ a или b. 
> 
> Ровно тоже самое и с строкой var {a, b} = theArr; 
> То есть будут созданы идентификаторы a и b и они будут связаны со значением которое имеет ключ a или b внутри theArr.
> 
> То есть в случае паттерна с квадратными скобками, создается полотенце кода, происходит полное итерирование обьекта и тд. А в случае памметрна с фигурными скобками, генерируется код доступа по ключу.
> 
> Например код: var {a, b} = obj;  преобразовывается к коду:
> var a = obj.a
> var b = obj.b;
> 
> или код: var {a, b} = theArr;
> var a = theArr.a
> var b = theArr.b;
> 
> Так как этих проперти нет, произойдет поиск по цепочки прототипов, и если и там нет то будет связано значение undefined.
> 
> А давайте подумаем, какое проперти всегда есть у Array Exotic Object ? 
> Правильно, у любого array всегда есть проперти length.
> Значит если мы напишем
> var theArr = [1, 2, 3];
> var {length} = theArr;
> 
> что должно произойти?
> Должен быть создан идентификатор length который будет связан со значением из property length для theArr. А какое у нас значение length в нашем примере для theArr? Правильно 3. 
> Значит length будет связано с тройкой.
> 
> 
> *ИГОГО*
> В случае использования любой синтаксической конструкции, связанной с символом = и квадратными скобками (например var [a,b,c] = theArr) будет создано полотенце кода с полным перебором всего theArr.
> 
> В случае использования синтаксической конструкции , связанной с символом = и фигурными скобками, (например var {a, b, c} = theArr) будет создано три команды каждая из которых создаст идентификатор a b или c, и при этом они будут связаны с theArr["a"], theArr["b"] или theArr["c"] соответственно.
> 
> Улавливаете?

---

**[@FedorBasmanof](https://www.youtube.com/channel/UC9wiSAQWG5Wml_bBomXMJYw)** *[15.05.2023 12:24](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgwLUl-xxVi-bjW8yWZ4AaABAg) · 👍 3*

Мурыч, верни вебку, не хватает твоего солнечного лика(

---

**[@FedorBasmanof](https://www.youtube.com/channel/UC9wiSAQWG5Wml_bBomXMJYw)** *[15.05.2023 13:21](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=Ugzz8mk5JUeKBqAprKh4AaABAg) · 👍 3*

Побольше таких видео с разбором байт-кода и таких мест в языке, очень нужные и полезные видео! Жду с нетерпением

---

**[@ixplo](https://www.youtube.com/channel/UCi1w3WhkVWha0BAIBEXL-bA)** *[15.05.2023 18:38](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgxyM_iaPsbr_DCUf5J4AaABAg) · 👍 1*

надеюсь, я не увижу деструктурирования массива через фигурные скобки в своих фронтенд-проектах ) тк около ста процентов фронтендеров надолго подвиснут, увидев такое ) Но спасибо за информацию

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[16.05.2023 12:15](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgxyM_iaPsbr_DCUf5J4AaABAg.9pk2l4yAN-g9plwedzGatN) · 👍 2*

> Самое важное в этом видео то, что ставит программиста перед вопросом - а почему я сам не догадался что ключи Exotic Object Array можно использовать как ключи для деструктурирующего присваивания.  Что должно было бы заставить человека больше думать над тем, чем является его код.
> 
> А это, в свою очередь, не позволило бы делать то, против чего Ваш протест. И я его целиком и полностью поддерживаю - код нужно писать осмысленно, а не использовать рекомендации шаманского типа.

---

**[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[03.06.2023 08:44](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=Ugw7INKNFzzOem3TGQB4AaABAg) · 👍 1*

Зачем вы the пишете в названиях идентификаторов? Привычка?

Как по мне, артикль лишний.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[04.06.2023 22:38](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=Ugw7INKNFzzOem3TGQB4AaABAg.9qUuse0QS8I9qYz5sZJeBC)*

> Я дислексик. Я не могу держать в голове больше 3 обьектов. Обычный человек может от 5 до 7. Потому я окружаю себя все время подсказками, которые мне упрощают жизнь

> **[@Евгений-э4н1б](https://www.youtube.com/channel/UC0zCoezb3PtBZsMTFg2y9Gw)** *[07.06.2023 07:40](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=Ugw7INKNFzzOem3TGQB4AaABAg.9qUuse0QS8I9qe5ea_Xrcm) · 👍 1*

> Так грамматически правильней)

---

**[@olezhonnv3215](https://www.youtube.com/channel/UCC8wE-XmGNMFvczNw_7UqNg)** *[03.06.2023 08:54](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgyUUsv8JIaepMn9ABx4AaABAg) · 👍 1*

Ну а как реализовать без итератора деструктуртзацию массива? Не просто же именно так это описано в спеке.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[04.06.2023 22:37](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgyUUsv8JIaepMn9ABx4AaABAg.9qUvyir-gRA9qYyzSe6rrL) · 👍 4*

> Совершенно верно!!!
> Я же это и подчеркивал. Я не говорил что это нельзя использовать. Я настаивал на том, что нужно понимать стоиомсть такого решения. Если меня стоимость устраивает - то использовать. А если нет - то думать как решить задачу иначе.

---

**[@SERGIUS_ORIGINAL](https://www.youtube.com/channel/UCorE8HdQ4HputSutpZpphFg)** *[08.06.2023 15:40](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgxQjw2ixQCwQXQ4kbx4AaABAg)*

Спасибо Большое!!!

---

**[@aleksandr1277](https://www.youtube.com/channel/UCfn0ShMtY4chSKs1t9C9nBw)** *[08.12.2023 20:45](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=Ugxu0JxIY7oaRkjdDYx4AaABAg)*

Хорошее объяснение. Благодарю! Как раз сейчас, интересуюсь микрооптимизацией кода, и вынужден углубляться в детали реализации.

---

**[@johngalt9494](https://www.youtube.com/channel/UCULcuPJ1SALjUpSli2PMNyA)** *[16.12.2023 14:31](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgxWV7RLFLH_FbNWsud4AaABAg) · 👍 2*

Коммент в поддержку канала !

---

**[@raff_m_d6971](https://www.youtube.com/channel/UCdsqd4Phl6ebcHNL1p1B5eg)** *[21.12.2023 19:08](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=Ugy4TKnzopqxwqljnqB4AaABAg)*

Выражаю безграничную благодарность автору за контент

---

**[@raff_m_d6971](https://www.youtube.com/channel/UCdsqd4Phl6ebcHNL1p1B5eg)** *[21.12.2023 19:08](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgzLdUQ9hZ2_mELiKJZ4AaABAg) · 👍 3*

Выражаю безграничную благодарность автору за контент

---

**[@fractalminding](https://www.youtube.com/channel/UC1PF4egUFAH2yY0uLo5dyxw)** *[10.01.2024 00:15](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=UgzFDA-3w_SXitg_4Kd4AaABAg) · 👍 1*

Я такое не использую. Делаю в таком духе:

var theArr = [1, 2, 3];
var a = theArr[0];
var b = theArr[1];

Надеюсь, это работает не медленнее, чем деструктурирующее присваивание 😁

---

**[@khmerhan2748](https://www.youtube.com/channel/UCQY3nUwcprTrW9ny_D2RHHw)** *[13.03.2024 22:14](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=Ugzl5R5qb8SAdAuyOfF4AaABAg) (ред. 13.03.2024 22:16)*

Круто всё разжевано!!! Правда возникают следующие вопросы ))). Например, что равноценны ли записи
myObj.myFunc();
и
var {myFunc}=myObj;
myFunc();
Но имя удочку, я уже понимаю, как наловить рыбку для своего любопытства.

Ещё раз благодарю, Мурыч-сама

---

**[@raff_m_d6971](https://www.youtube.com/channel/UCdsqd4Phl6ebcHNL1p1B5eg)** *[02.04.2024 05:58](https://www.youtube.com/watch?v=98mOkxRFHYA&lc=Ugws1_ahpm_YiY4shpx4AaABAg)*

Выражаю благодарность автору за контент

---
