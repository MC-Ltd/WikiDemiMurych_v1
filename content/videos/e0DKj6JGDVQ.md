---
title: "Смотрим вместе YT:   Ulbi TV, собеседование на  Middle  FrontEnd разработчика"
date: 2025-06-30
tags: ["yt", "11", "js", "ulbi", "sobes"]
videoId: "e0DKj6JGDVQ"
duration: "4:21:22"
views: 9555
likes: 243
comments: 58
---
# [Смотрим вместе YT:   Ulbi TV, собеседование на  Middle  FrontEnd разработчика](https://www.youtube.com/watch?v=e0DKj6JGDVQ)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 30.06.2025 23:31  
**Тривалість:** 4:21:22  
**Перегляди:** 9555 · **Лайки:** 243 · **Коментарі:** 58
![thumbnail](https://i.ytimg.com/vi/e0DKj6JGDVQ/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=e0DKj6JGDVQ)
## Коментарі (23 · відповідей: 35)

**[@astrobrite540](https://www.youtube.com/channel/UC4D058sPZcXUR8ukz2ZlLIw)** *[30.06.2025 23:25](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgykPdG2yyviLbPgTGh4AaABAg) · 👍 4*

Изгнание бесов из реактдевелоперов

---

**[@vdbxxx](https://www.youtube.com/channel/UClsjzAwVoVWWQEpnJE8pDJg)** *[01.07.2025 06:47](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyCHZ2rggtUnp0V_0p4AaABAg)*

Начнём с того, что ваше решение не проще - простой цикл против применения костылей, появившихся недавно в языке. Продолжим тем, что писать его дольше и читать его труднее (вы сами зависали в документации, прежде чем найти нужные функции). B закончим тем, что там с разницей в производительности? Подозреваю, что в отдельных частных случаях ваш код потребует больше памяти и времени исполнения.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[07.07.2025 01:29](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyCHZ2rggtUnp0V_0p4AaABAg.AK13m17DX9PAKFxACw2Nns)*

> Я не понял что именно Вы назвали костылями. Поясните пожалуйста.
> 
> А в документации я всегда зависаю, по несколким причинам: я дислексик и мне нужно больше времени чтобы что-то понять, и это отдельный прием, который позволяет человеку просматривающему видео, сосредоточится на том что на экране и самому сделать выводы.
> 
> Если у Вас есть потребность оценить мои способности к решению задач без чтения документации вот Вам видео
> https://www.youtube.com/watch?v=6H0e4c-SPgo&list=PL3ziSA8uO7KmJo-QbCvhj57cVW5JF5Nyx&index=6
> 
> Там с десяток задач с пояснениями, с условием не заглядывать ни в одну из документаций.

---

**[@FrankBakulov](https://www.youtube.com/channel/UC73lSQURf81UCdJHJ884tJA)** *[01.07.2025 08:55](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyzOCfLP-wuCQoXEbp4AaABAg) · 👍 2*

48:40 "мы можем функцию асинк сделать?" - вздох на фоне. Бесценно! ❤

---

**[@СергейГоловань-т6з](https://www.youtube.com/channel/UCkxkMbdQUZPKjLN4dDD9S1w)** *[01.07.2025 09:41](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgzqEXtodFIFSH3zUnZ4AaABAg) (ред. 01.07.2025 09:50)*

1:23:58 Почему нельзя было воспользоваться свойством errors из AggregateError? Оно и хранит нужный нам массив со списком значений, выброшенных из отклоненных промисов. Получится что то вроде:
async resolver(promises) {
   try {
     return await Promise.any(promises)
   } catch (e) {
      return e.errors
   }
}

Здесь пользуемся тем, что результат асинхронной функции будет обернут в Promise.

P.S. Сори, замечание про то, что errors может быть не всегда доступен услышал)

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[07.07.2025 01:25](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgzqEXtodFIFSH3zUnZ4AaABAg.AK1NkYkzi1ZAKFwgBBgiRo)*

> Кроме того, Ваш код будет выполняться последовательно. Что уничтожает преимущество предоставляемое Promise.

---

**[@anthonys173](https://www.youtube.com/channel/UChEXzcASC0k6B2vqX03L9ew)** *[01.07.2025 10:56](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugy4GwlAXOsIvf1JuyF4AaABAg) · 👍 3*

Привет, лекции какого автора рекомендовали послушать на 39 минуте? Не смог разобрать фамилию.

> **[@AvigdorKatz](https://www.youtube.com/channel/UCk6X3w_IO90tJpulmBkPE9w)** *[01.07.2025 11:43](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugy4GwlAXOsIvf1JuyF4AaABAg.AK1WLKFt04iAK1aizyeoMn)*

> Та вроде разборчиво звучит Брагилевский

> **[@anthonys173](https://www.youtube.com/channel/UChEXzcASC0k6B2vqX03L9ew)** *[01.07.2025 12:37](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugy4GwlAXOsIvf1JuyF4AaABAg.AK1WLKFt04iAK1guGRn4o8)*

> @AvigdorKatz спасибо

---

**[@kakieToYroki](https://www.youtube.com/channel/UCBnoCxkFZD4XkCDzBAwl5JA)** *[01.07.2025 11:49](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgxXQRVheTsFYBmaXu54AaABAg) · 👍 7*

07:54 Мурыч против доты - так и запишем 😁

> **[@NoName-bf9wh](https://www.youtube.com/channel/UC1dybHqsY8dQoiPbio9S8ow)** *[02.07.2025 16:01](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgxXQRVheTsFYBmaXu54AaABAg.AK1bLcbYgehAK4cxsVzwGW) · 👍 2*

> в очередной раз поражаюсь как люди могут переиначивать смысл сказанного...
> я, конечно, понимаю, что ты рофлишь, просто мне реально показалось, что он выскажет позицию против, хотя фактически это не так

---

**[@ИванВоротилин-п9ю](https://www.youtube.com/channel/UCW_19fzG_g6Vbo52vkIHaCQ)** *[01.07.2025 11:57](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgwSFdyY53MYDOqWXsZ4AaABAg)*

Влад, респект тебе!

---

**[@FaragayCage](https://www.youtube.com/channel/UC3tDuTILL3wUU9MUvM-OOSw)** *[01.07.2025 17:57](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyTbUoEnkmQPn7sREp4AaABAg)*

44:00 мое решение до просмотра разбора от Мурыча

async function resolver(promises: Promise<number>[]): Promise<number | number[]> {
    const rejects = new Array<number>();

    for (const promise of await Promise.allSettled(promises)) {
        if (promise.status === 'fulfilled') return promise.value;

        rejects.push(promise.reason);
    }

    return rejects;
}

> **[@mikhailrezhisser4351](https://www.youtube.com/channel/UCXy6T6yFYnJ2KC3AfM4BYXQ)** *[01.07.2025 18:45](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyTbUoEnkmQPn7sREp4AaABAg.AK2GVqUehw1AK2LyK_tn7V)*

> минус в том что тебе нужно дожидаться выполнения всех промисов, хотя в идеале нужно вернуть сразу если есть первый успешный

> **[@FaragayCage](https://www.youtube.com/channel/UC3tDuTILL3wUU9MUvM-OOSw)** *[02.07.2025 02:20](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyTbUoEnkmQPn7sREp4AaABAg.AK2GVqUehw1AK3A60Bd01A) (ред. 02.07.2025 03:03)*

> Увы не вижу пример кода, который бы эффективно исправлял этот минус, поэтому возьмем решение Мурыча и представим кейс, что все промисы реджектят. Но тогда мы вынуждены дожидаться выполнения всех промисов дважды, это тоже минус. Асимптотическая сложность функции всегда оценивается по худшему сценарию, соответственно у меня это Promise.allSettled + итерация по settled промисам - O(2n), а у Мурыча Promise.any + Promise.allSettled + map - O(3n). Вот и получается, что решение Мурыча лучше когда хотя бы один промис резолвит, а мое решение лучше когда все реджектят, таков трейд-офф.

> **[@FaragayCage](https://www.youtube.com/channel/UC3tDuTILL3wUU9MUvM-OOSw)** *[02.07.2025 03:05](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyTbUoEnkmQPn7sREp4AaABAg.AK2GVqUehw1AK3F9WaRxCR) · 👍 1*

> UPD: после просмотра разбора мое решение не изменилось, но почитав комментарии пришел к этому:
> 
> async function resolver(promises: Promise<number>[]): Promise<number | number[]> {
>     return Promise.any(promises).catch((rejects: AggregateError) => rejects.errors);
> }
> 
> Оказывается метод Promise.any() роняет в исключение AggregateError объект, когда все промисы реджектят, из него можно достать массив переданных в Promise.reject()  значений и не нужно запускать выполнение промисов еще раз. Временная сложность этой функции при любом сценарии получается O(n) - идеально. Все таки действительно бывает полезно заглядывать в спецификацию)

> **[@vanel9933](https://www.youtube.com/channel/UCSBOwadbKrQsoIIO2tdoDnA)** *[02.07.2025 06:49](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyTbUoEnkmQPn7sREp4AaABAg.AK2GVqUehw1AK3doI3LcYM)*

> ​@FaragayCageвы совершенно не понимаете, что такое временная и асимптотическая сложность

> **[@FaragayCage](https://www.youtube.com/channel/UC3tDuTILL3wUU9MUvM-OOSw)** *[02.07.2025 14:29](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyTbUoEnkmQPn7sREp4AaABAg.AK2GVqUehw1AK4TU9ARbBK)*

> @vanel9933 нет, это вы не понимаете.

---

**[@mikhailrezhisser4351](https://www.youtube.com/channel/UCXy6T6yFYnJ2KC3AfM4BYXQ)** *[01.07.2025 18:44](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyGB4HREOM4nDXrUBN4AaABAg) (ред. 01.07.2025 18:53) · 👍 16*

сделал пизже мурыча (ставим лайки):
function resolver(promises) {
  return Promise.any(promises).catch(e => Promise.reject(e.errors));
}

> **[@omahaLinkva](https://www.youtube.com/channel/UCzpe5YASSzjFIT4QN2ZVT4g)** *[01.07.2025 19:26](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyGB4HREOM4nDXrUBN4AaABAg.AK2Lo4o5y4SAK2QbehS_1k) (ред. 01.07.2025 19:26) · 👍 2*

> Я ему весь стрим в чате писал об этом, видимо я не рос до его уровня чтобы городить такой огород как он согласно спецификации 😅

> **[@FaragayCage](https://www.youtube.com/channel/UC3tDuTILL3wUU9MUvM-OOSw)** *[02.07.2025 01:50](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyGB4HREOM4nDXrUBN4AaABAg.AK2Lo4o5y4SAK36eS8HStF) · 👍 1*

> О, ну хоть кто-то здесь читал спецификацию и  помнит контракты промисов 👏

> **[@TheLevius](https://www.youtube.com/channel/UCzch7ASsg9zJzd4yrAJv8-Q)** *[02.07.2025 10:29](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyGB4HREOM4nDXrUBN4AaABAg.AK2Lo4o5y4SAK4221QJUbF) · 👍 3*

> мне казалось что смысл задачи в том что нельзя использовать any, race, allSettled

> **[@omahaLinkva](https://www.youtube.com/channel/UCzpe5YASSzjFIT4QN2ZVT4g)** *[02.07.2025 15:40](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyGB4HREOM4nDXrUBN4AaABAg.AK2Lo4o5y4SAK4a_HuxMKC) · 👍 1*

> ​@TheLeviusтам не было такого условия, но кстати не понятно должны ли промисы исполнятся паралельно или последовательно

> **[@egork.chudin](https://www.youtube.com/channel/UCfGWfzeUK3de9N7PcT0PrdA)** *[29.07.2025 11:25](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyGB4HREOM4nDXrUBN4AaABAg.AK2Lo4o5y4SAL9ew9dFiJX) · 👍 1*

> Promise.reject не отработает, надо resolve, чтобы результат вернуть.

> **[@omahaLinkva](https://www.youtube.com/channel/UCzpe5YASSzjFIT4QN2ZVT4g)** *[29.07.2025 11:50](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyGB4HREOM4nDXrUBN4AaABAg.AK2Lo4o5y4SAL9hjQntPSR)*

> ​@egork.chudinвсе там отработает, any вернёт промис, катч нужен для обработки ошибок

> **[@omahaLinkva](https://www.youtube.com/channel/UCzpe5YASSzjFIT4QN2ZVT4g)** *[29.07.2025 15:01](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyGB4HREOM4nDXrUBN4AaABAg.AK2Lo4o5y4SALA2bitd8nf) (ред. 29.07.2025 15:02)*

> ​​@egork.chudinотработает и вызовет reject, как обычный промис в котором произошла ошибка, если хочется можно resolve сделать. Только сути это не меняет, что это решается через any, а не через кучу костылей как на стриме

> **[@egork.chudin](https://www.youtube.com/channel/UCfGWfzeUK3de9N7PcT0PrdA)** *[29.07.2025 15:08](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyGB4HREOM4nDXrUBN4AaABAg.AK2Lo4o5y4SALA3PARVB5b)*

> @omahaLinkva да, я просто про то, что надо получить положительный результат. типа resolver([Promise.reject(5), Promise.reject(6)]).then(console.log) в случае reject ниче не выведет.
> 
> но да, мурыч намудрил

> **[@computercomputer3293](https://www.youtube.com/channel/UCMwqst-QsNwF-WWrdwhpdTw)** *[05.08.2025 16:42](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyGB4HREOM4nDXrUBN4AaABAg.AK2Lo4o5y4SALSFfK_j5bT)*

> Так вроде в видео он объясняет, что в таком случае нет гарантии, что все ошибки пропадут в массив

---

**[@AmericanDragon123](https://www.youtube.com/channel/UC1Dol7mXhwhf_cc0bMekkiA)** *[02.07.2025 04:04](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugywxye0dze0EN4257l4AaABAg) · 👍 1*

2:05:00 Your code is not very readable

---

**[@WillaTutorial](https://www.youtube.com/channel/UCL6x2pe5WdEF8uP5fmPesaw)** *[02.07.2025 08:08](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgxtxfaLGVRx-hh65nV4AaABAg)*

этот собес очевидно слабоват. Посмотрите пожалуйста собес на 500к на канале Миша - Frontend Dev. ИМХО если осознанно отвечаешь на вопросы с этого собеса, то это точно Мидл ++

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[07.07.2025 01:21](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgxtxfaLGVRx-hh65nV4AaABAg.AK3muRSydoMAKFwDHbnUr8)*

> На том канале есть Видео со мной. 
> https://www.youtube.com/watch?v=vrfbB3Udntw

---

**[@TheLevius](https://www.youtube.com/channel/UCzch7ASsg9zJzd4yrAJv8-Q)** *[02.07.2025 10:28](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgzZBaeTQeylmfDSGD14AaABAg) · 👍 2*

Я правильно понял что мурыч эту задачу час решал?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[07.07.2025 01:20](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgzZBaeTQeylmfDSGD14AaABAg.AK41u59LFfQAKFw5rrEoYY)*

> Неправильно. Подумай еще

---

**[@FrankBakulov](https://www.youtube.com/channel/UC73lSQURf81UCdJHJ884tJA)** *[02.07.2025 14:48](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugw1TSig2141eawA7Nt4AaABAg)*

allSettled не нужно - по условию задачи все промисы settled

---

**[@artemzalevsky1857](https://www.youtube.com/channel/UCX4dY8mukHm-JzQshY_3qzQ)** *[02.07.2025 18:31](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgwjP3x-bnSujqWwDB14AaABAg) · 👍 1*

Мурыч, смысл таких задач на собесах как раз в том, чтобы не использовать готовые статические методы. И ты решил намного сложнее, чем это решается на уровне современного языка JS.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[07.07.2025 01:19](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgwjP3x-bnSujqWwDB14AaABAg.AK4uCCJf3AqAKFw2ps7pso)*

> Смысл таких задач на собеседования в том, чтобы оценить как человек принимает решения. Сам по себе код - значение имеет очень опосредованное.

---

**[@igorsk1133](https://www.youtube.com/channel/UCOVjXHvpWG4YqtlyfCpSWCQ)** *[02.07.2025 22:35](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgxdxP-aghJt7EEiCd94AaABAg) · 👍 1*

3k ммр в доте это вроде и не много. но я хз сколько это часов. не играл в эту парашу

> **[@glfx_dragon](https://www.youtube.com/channel/UCaHlJH6J7bVlP1XHqga16eA)** *[06.07.2025 15:38](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgxdxP-aghJt7EEiCd94AaABAg.AK5L8BBZ7RvAKEt_01w3Tc)*

> 3к ммр можно как за 100 часов получить, так и за несколько тысяч

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[07.07.2025 01:17](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgxdxP-aghJt7EEiCd94AaABAg.AK5L8BBZ7RvAKFvrbQaCi7)*

> Речь шла не про Доту. А про chess

---

**[@amat0ru](https://www.youtube.com/channel/UCe6r95nuOx1chSeLzR0aabg)** *[03.07.2025 10:51](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugy4xgWsapccjDJkcmp4AaABAg) · 👍 3*

мурыч, по поводу первой задачи, если б ты не смотрел в доку ты бы и синтаксис и метод не вспомнил и ничего бы не написал, а человек не смотрел в доку и написал, смотря в доку, имея время, не имея волнения любой человек напишет такое же решение

> **[@user-yf1of4nu9w](https://www.youtube.com/channel/UCkQBvIwdNvFN2Y2ic45VrKA)** *[06.07.2025 07:45](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugy4xgWsapccjDJkcmp4AaABAg.AK6eLnNMBxuAKE2NpNaWPJ)*

> Ты вообще осознал свое вот это что ты высрал🤡😵‍💫🤡😵‍💫

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[07.07.2025 01:17](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugy4xgWsapccjDJkcmp4AaABAg.AK6eLnNMBxuAKFvnQv-BUu) · 👍 2*

> Когда то, один из посетителей моих трансляций, предьявил мне похожую претензию. Результатом чего стала запись:
> Решаем задачи без подглядывания в спецификацию.
> https://www.youtube.com/watch?v=6H0e4c-SPgo&list=PL3ziSA8uO7KmJo-QbCvhj57cVW5JF5Nyx&index=6
> 
> Кажется там я решил все без ошибок. Посмотрите. Может измените свое мнение.
> 
> Да и это не важно. Помнить все детали, всех методов - лично для меня очень обременительно. И я предпочитаю помнить, куда мне посмотреть, чтобы проконтролировать себя.
> 
> Если хотите, можете меня протестировать онлайн. Я не против.

> **[@vdbxxx](https://www.youtube.com/channel/UClsjzAwVoVWWQEpnJE8pDJg)** *[07.07.2025 05:41](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugy4xgWsapccjDJkcmp4AaABAg.AK6eLnNMBxuAKGOzlrOsc4)*

> @AsForJS _"Помнить все детали, всех методов - лично для меня очень обременительно."_ И не только вам. Именно поэтому любое решение с дополнительными методами будет сложнее и дольше в написании и чтении. Вы же утверждали, что ваше решение проще в сравнении с простым циклом с абсолютно понятным await.

> **[@yarburart7242](https://www.youtube.com/channel/UCKHEa7INulixxZvAZrO7QEA)** *[08.08.2025 16:40](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugy4xgWsapccjDJkcmp4AaABAg.AK6eLnNMBxuALZypHuVk3_)*

> ​@AsForJS какие тогда действия на самом собеседовании в такой ситуации?

---

**[@Andrew-NaN](https://www.youtube.com/channel/UCvEyMg75ev6ICAbl2yxUBpg)** *[04.07.2025 09:24](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugwli-E5HtPMmiwg4e14AaABAg) (ред. 04.07.2025 09:37) · 👍 3*

4:13:00 мурыч объясняет КАК ПРОИСХОДИТ ВЫПОЛНЕНИЕ КОДА и разницу между "ВСПЛЫТИЕМ", HOISTABLE DECLARATION (функции, генераторы включая async), VARIABLE STATEMENT and LET/CONST DECLARATION

---

**[@vasilyivanov7792](https://www.youtube.com/channel/UCeZX5PEH0KiOpxOwLMU7h-g)** *[06.07.2025 08:23](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgwM3mhe3ubv_nxfco14AaABAg) · 👍 2*

const resolver = (promises) => Promise.any(promises).catch((error) => error.errors);

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[07.07.2025 01:07](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgwM3mhe3ubv_nxfco14AaABAg.AKE6n6YH7X5AKFui5D9Kdj)*

> Только следует не забывать, что каждый метод из Promise.prototype возвращает новый промис - который не дешев.
> 
> В коде выглядит так, будто бы всего лишь одна точка с вызовом метода, вместе с тем под капотом создание полноценного промиса на каждом шаге.

---

**[@АсланМальсагов-й8и](https://www.youtube.com/channel/UCQQnj-q4QfTFywU8IwPKtzg)** *[08.07.2025 15:04](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugwd3eF9Kva1xjBT8614AaABAg) · 👍 1*

На async/await 

const resolver = async (arr) => {
    const errors = [];
    
    for (let i = 0; i < arr.length; i++) {
        try {
            return await arr[i];
        } catch (error) {
            errors.push(error)
        }
    }

    return errors
}

> **[@АсланМальсагов-й8и](https://www.youtube.com/channel/UCQQnj-q4QfTFywU8IwPKtzg)** *[08.07.2025 15:09](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugwd3eF9Kva1xjBT8614AaABAg.AKJzFfLnLCkAKJzo1SfYwy) · 👍 1*

> async function resolver(arr) {
>     try {
>         return await Promise.any(arr);
>     } catch (error) {
>         return error.errors;
>     }
> }

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[08.07.2025 17:28](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugwd3eF9Kva1xjBT8614AaABAg.AKJzFfLnLCkAKKEjlQNMfA)*

> Можно и так, если нас не волнуют проблемы производительности и прожорливости async функций.

> **[@EgorFrade](https://www.youtube.com/channel/UCp4dF6CWtuEXeEkXfol25UA)** *[14.07.2025 10:45](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugwd3eF9Kva1xjBT8614AaABAg.AKJzFfLnLCkAKYyLcKRcgj)*

> вроде в условии нужно было вернуть самый "быстрый" а тут будет рандомный

---

**[@ильякочетков-з7ч](https://www.youtube.com/channel/UCn_uahQqulot-YuroHu4-Ew)** *[09.07.2025 19:06](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugwl6yeh-EYOp9I2RpF4AaABAg)*

я че-то не понял. Тут вот вроде недавно Климов мелькал перед стримом. А сейчас "никак не отношусь"... к делу это не относится, конечно, но шото я пропустил

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[29.07.2025 22:05](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=Ugwl6yeh-EYOp9I2RpF4AaABAg.AKMznAnZQaeALAo4ojKyzJ) (ред. 29.07.2025 22:05) · 👍 2*

> Мы разошлись в той части, где я считаю, что если разговариваю с человеком, то ожидаю от него именно его экспертизы. 
> Илья Климов решил, что, как минимум со мной, он может транслировать чат GPT вместо своей личной оценки.
> 
> В итоге я принял решение, что не имею право больше заставлять  такого великого человека транслировать лично для меня ответы чата GPT.  
> Потому как, чтобы узнать мнение последнего (чата), мне не нужно тратить время Ильи Климова.

---

**[@baknicholson8140](https://www.youtube.com/channel/UCx6CKmMQcgvNzIo4GctHoRQ)** *[10.07.2025 14:47](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgwuaCNr0RKWz2-wj8p4AaABAg)*

Сильно намудрил с решением задачи от YT: Ulbi TV

Вот решение, которое полностью удовлетворяет требованиям задачи, а так же проще и понятнее

function resolver(promises) {
    return Promise.any(promises).catch(e => e.errors);
}

> **[@baknicholson8140](https://www.youtube.com/channel/UCx6CKmMQcgvNzIo4GctHoRQ)** *[10.07.2025 14:49](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgwuaCNr0RKWz2-wj8p4AaABAg.AKP5uCclGPKAKP6871RC_L) · 👍 1*

> Сам Promise.any возвращает promise, дополнительное создание промиса не нужно. В случаи ошибки Promise.any возвращает AggregateError, из которого достаточно просто получить значения обращением к errors

> **[@computercomputer3293](https://www.youtube.com/channel/UCMwqst-QsNwF-WWrdwhpdTw)** *[05.08.2025 16:40](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgwuaCNr0RKWz2-wj8p4AaABAg.AKP5uCclGPKALSFVj2P_vb)*

> Так вроде в видео он объясняет, что в таком случае нет гарантии, что все ошибки пропадут в массив

---

**[@webHead7](https://www.youtube.com/channel/UC5nr6oXF3c_hvCDwZMl4vSA)** *[12.07.2025 22:07](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyHPQcQd9gQiK95Kgt4AaABAg)*

Мою кошку зовут Туча...
Угадайте мое удивление с первых секунд ролика...

---

**[@aw3s0me](https://www.youtube.com/channel/UCZF0SMvwrmENu83ho9A2BRA)** *[22.07.2025 15:26](https://www.youtube.com/watch?v=e0DKj6JGDVQ&lc=UgyhyCIljrmSum3MhA14AaABAg)*

ну и да, обычно такие задачи подразумевают что весь этот сахар в виде any / all / allSettled - недоступен.
Смысл этих задач как раз и написать статический метод класса промис

---
