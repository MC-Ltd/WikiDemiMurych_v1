---
title: "[Stripped] Производительность  Async Function"
date: 2025-07-08
tags: ["perf", "10", "async", "Function", "Ecma", "v8"]
videoId: "A6zgTaxo3R4"
duration: "44:11"
views: 3638
likes: 169
comments: 28
---
# [[Stripped] Производительность  Async Function](https://www.youtube.com/watch?v=A6zgTaxo3R4)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 08.07.2025 23:41  
**Тривалість:** 44:11  
**Перегляди:** 3638 · **Лайки:** 169 · **Коментарі:** 28
![thumbnail](https://i.ytimg.com/vi/A6zgTaxo3R4/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=A6zgTaxo3R4)
## Коментарі (21 · відповідей: 7)

**[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[09.07.2025 00:08](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgyvNyLN3g3boQUeWCR4AaABAg) · 👍 5*

Это урезанная до 40 минут версия 6 часового стрима. Полная версия со всеми вопросами и ответами тут https://youtube.com/live/VfQiG2jATgQ

> **[@lunandev](https://www.youtube.com/channel/UCbFap_BhuLBncU3FDZc_MhA)** *[09.07.2025 01:41](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgyvNyLN3g3boQUeWCR4AaABAg.AKKxVCNwYAgAKL77AwHJfa) · 👍 2*

> Спасибо

---

**[@dihaneeer](https://www.youtube.com/channel/UC2huwPsbDiCGlOlnXFxglmw)** *[09.07.2025 00:21](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgzUyc8Oa3EfSxn9f0p4AaABAg) · 👍 1*

Спасибо за запись и наглядное объяснение! 👍

---

**[@alenache1](https://www.youtube.com/channel/UCJ-u6p_Urn0fbRu7MgvV_tQ)** *[09.07.2025 05:50](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgyVoZ4EWj-_bng6Edl4AaABAg) · 👍 15*

Шортсы от Мурыча на 40 минут 🤣🤣🤣

> **[@bukanaka](https://www.youtube.com/channel/UClwPjU0S-_hiTbH1JsoS-rg)** *[26.09.2025 07:34](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgyVoZ4EWj-_bng6Edl4AaABAg.AKLZaBGThJvANXALqKSkhk) · 👍 1*

> 😂😂

---

**[@AvigdorKatz](https://www.youtube.com/channel/UCk6X3w_IO90tJpulmBkPE9w)** *[09.07.2025 07:17](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgyvhQyLhnLiz2bx9b14AaABAg) · 👍 7*

Спасибо за сокращённую версию. Про разницу ресурсов и использование генераторов не знал. Но про последовательность или параллельность запросов с использованием await это по-моему само собой разумеющееся.

---

**[@АлексейСтепаненко-м8в](https://www.youtube.com/channel/UCQd5CW9PupQxYtXp7iyOmhA)** *[09.07.2025 08:16](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgwVE3SuCJi3Ev_cxfl4AaABAg) · 👍 1*

Респект, братуха, за то что пояснил.

---

**[@admToha](https://www.youtube.com/channel/UCVI_tHFBxVcJoxu86lGi5Qw)** *[09.07.2025 12:06](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgyZB-g5Nig6_B5Lt6Z4AaABAg) (ред. 09.07.2025 12:20) · 👍 2*

>> При этом для ассинхронной функции, которая делает ровно тоже самое...

Мурыч, позвольте возразить. Ваша асинхронная функция делает НЕ(!) тоже самое. В приведённой асинхронной функции промисы выполняются последовательно, сначала 1-ый, после него - 2-ой. А вот в примере неасинхронной функции оба промиса выполняются параллельно внутри Promise.all(). Разница существенная.

Если нужно то же поведение, то нужно переписать неасинхронную функцию например так:
function doAsync(){
  const result = [];
  Promise.resolve("First").then(res => result.push(res) && Promise.resolve("Second")).then(res => result.push(res) && console.log(result));
}

UPD. Вы дальше в видео уже объясняете про последовательное/параллельное выполнение, так что моё возражение, видимо, не к месту.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[29.07.2025 22:11](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgyZB-g5Nig6_B5Lt6Z4AaABAg.AKMEfoqP1OIALAonWCplHG) · 👍 1*

> Нет не так. 
> что для Promise.All, что для связывания двух промисов внутри Async примера, порядок одинаков и соотвествует спецификации. 
> 
> И то что это так, явным образом показано на записи трейса выполнения функции.

> **[@admToha](https://www.youtube.com/channel/UCVI_tHFBxVcJoxu86lGi5Qw)** *[02.08.2025 08:07](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgyZB-g5Nig6_B5Lt6Z4AaABAg.AKMEfoqP1OIALJbS8p0cuW)*

> @AsForJS Мной подразумевалось, что пример синтетический / учебный, то есть на месте Promise.resolve() можно подставить любое асинхронное действие, когда порядок будет не столь очевиден.

---

**[@alexl.4388](https://www.youtube.com/channel/UCuHwA5_DoKfJFNTrNsPS9pg)** *[09.07.2025 13:12](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgwUydiN_PcTVGbH9cB4AaABAg) (ред. 09.07.2025 13:17)*

Мы убедились, что для async-функций вместо Promise расход памяти примерно в 2 раза больше при запуске одной функции. А если таких функций будет много, расход памяти будет расти пропорционально их количеству или как-то по-другому? 
Мысль в том, что если асинхронных функций достаточно много и расход растет не пропорционально, а, допустим, уменьшаясь, то их использование может быть оправдано.

Но даже если и так, то все равно остается жирный минус в виде сильно затрудненной оптимизации...

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[29.07.2025 22:09](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgwUydiN_PcTVGbH9cB4AaABAg.AKMMC8BvPLBALAoZipyZDX) · 👍 1*

> Относитесь к async/await как к удобному инструменту, который стоит дополнительных денег, сделать понятным для себя то, что можно сделать без этих денег, но при этом с большим напряжением.
> 
> А дальше уже Вам решать как разработчику, что для Вас при текущей задачи важнее:
> сделать проще для понимания, но дороже 
> или
> сделать сложнее для понимания, но эффективнее

---

**[@xkochevnikx_svt](https://www.youtube.com/channel/UCASBqrtTuVLzyxtDktIBgdA)** *[09.07.2025 13:59](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgwNA6WU2ypZtV_xHDJ4AaABAg) · 👍 2*

Очень познавательно, спасибо за ролик, здоровья автору!

---

**[@ilyagamepub](https://www.youtube.com/channel/UCOWeUcz3RAZeorXUxyIxrYQ)** *[09.07.2025 17:25](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=Ugz5v6mOT8qMV1itaY14AaABAg) · 👍 1*

Очень познавательное видео. Всю жизнь жил с формулировкой "await это синтаксический сахар над промисами". Разрыв шаблона пока не бородатого джаваскриптера с пятилетним стажем

---

**[@boonya41](https://www.youtube.com/channel/UCwY8gYrLxL7wQ1m-1H7lGlw)** *[10.07.2025 20:41](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgwUynoJdMKnrEjRN3F4AaABAg)*

Так ведь запросы параллельны, но ожидание резолвов их промисов все равно последовательное. `await Promise.all([todosPromise, commentsPromise])` я так делаю

---

**[@sergeisychov9810](https://www.youtube.com/channel/UCZeedKbfYHtbVgySFkabJkA)** *[13.07.2025 10:15](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgwIwv8KnolhpmPKkZx4AaABAg) (ред. 13.07.2025 10:17)*

Пока смотрел на 10 минут больше чем можно было, успела месячная борода вырасти)))
Спасибо, Мурыч)))
Интересный контент про await, генераторы и конечно же байткод (куда же без него😂).

---

**[@mavricus](https://www.youtube.com/channel/UCs2TxbiYdbk_SVh7tApG32A)** *[14.07.2025 00:12](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgyntXRMWXXgOJUgjVF4AaABAg) · 👍 2*

Согласен с автором, async/await действительно удобен, но под капотом это синтаксический сахар над генераторами, и его использование не бесплатно с точки зрения производительности. В high-load сценариях (например, серверный код) важно понимать, как это устроено внутри.

По поводу последнего примера: если заранее создать промисы и потом ждать их через await, есть риск, если второй промис реджектнется до завершения первого, ошибка пройдёт мимо и вызовет uncaughtException. В серверном коде это критично, потому что такие ошибки должны приводить к рестарту процесса.

Поэтому этот подход допустим только при полном контроле над промисами. Во всех остальных случаях лучше считать его антипаттерном.

> **[@ixplo](https://www.youtube.com/channel/UCi1w3WhkVWha0BAIBEXL-bA)** *[29.07.2025 20:52](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgyntXRMWXXgOJUgjVF4AaABAg.AKXpwQz-WZHALAfj0sGEJf) · 👍 1*

> +1 хз что автору помешало сделать await Promise.all([fetch1, fetch2])

---

**[@ixplo](https://www.youtube.com/channel/UCi1w3WhkVWha0BAIBEXL-bA)** *[29.07.2025 20:51](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgxvfriT2HpgE9Rk7nZ4AaABAg)*

а сделать await Promise.all([fetch1, fetch2]) нам религия не позволила в последнем примере? )

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[29.07.2025 21:21](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgxvfriT2HpgE9Rk7nZ4AaABAg.ALAfccZp-YjALAj1sgZJ7P)*

> Можно и так. Смысл был не в этом. 
> Смысл был в том, чтобы обратить внимание на тот факт, что разрешение промиса, который может быть выполнен заранее, можно и нужно выполнять заранее.
> 
> Смысл в том, чтобы показать что await это не про пошаговое выполнение асинхронного кода. Это про то, как пошагово организовывается резолвинг промисов.

---

**[@aculhan](https://www.youtube.com/channel/UCG3q-yE4W1EAAWPChK57swQ)** *[15.08.2025 23:16](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgwGk4INZ3dHtgBO5b54AaABAg) · 👍 1*

Видео очень информативное, я незнал что там творится под капотом, спасибо Дядя Мурыч

---

**[@simonsyoutube2003](https://www.youtube.com/channel/UCOi8JyGOAsEvvxHyPapldMg)** *[29.08.2025 18:54](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgyNwEb--YTzNRdYeQp4AaABAg)*

https://youtu.be/76wzB8-GB98?si=n83dCd-LJKKofP27

---

**[@ЯнаБабичева-ъ9д](https://www.youtube.com/channel/UC0BnzePpRW3QAHkhkVD_5RQ)** *[12.09.2025 15:12](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgzKbhf8Z4M6VaYvliJ4AaABAg)*

спасибо за такую ценную информацию

---

**[@drivee667](https://www.youtube.com/channel/UC2iW4tSzKSxvu10cn6QMu4A)** *[17.10.2025 08:20](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgwaizZE0kr3H4VEg8R4AaABAg) · 👍 1*

если бы все стримы уложить в 40 мин цены бы не было.

---

**[@ВикторКулагин-ь2у](https://www.youtube.com/channel/UCHOnFz5RbOpVQKKXRvdwZlQ)** *[30.10.2025 15:38](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgzA8BLbwDo84_RjdUN4AaABAg)*

Ух, ты. Какой толковый человек. Супер

---

**[@DmitryAstrauh](https://www.youtube.com/channel/UCnjc0e-9iIfsl0RYIsAd2dQ)** *[21.12.2025 20:50](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=Ugy_8kWZyzpT6WssJ1p4AaABAg) · 👍 1*

Здравствуйте. А может ли быть так, что async await это все же синтаксический сахар над промисами, а то, что в байт-коде встречаются упоминания генератора это не больше чем оптимизация самого V8?

---

**[@jiunov](https://www.youtube.com/channel/UCHNliZIxswncH3-HO0w5BHw)** *[26.02.2026 01:01](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=UgzRQ0Nm4SmSK1I9swt4AaABAg)*

Без использования Firefox ничего не стоит, похуй на ваш V9, и ты старый успокойся, rust или zig  поучи, один язык не стоит жизни, технологии меняются, разное там пробуй... Js имеет историю и оброс хуйней всякой из-за этого, вывод, убоать лишнее, придумать простой новый язвк для скриптинга. Вы бля старики заебали хвалить свои могилы и в них разбираться, вы в лингвистику посмотрите. Языки нужны чтобы просто передавать хуйню между "оюъектами", если сложный нахуй нужен. JS охуенный язык всё равно, но нужно подумать орациональности и будущем, чё мы дальше будем растить кодовую базу движка которая один хуй на си пишется или чё делать?

---

**[@advance5189](https://www.youtube.com/channel/UCikjXPtUzv58EGw2wStgnsQ)** *[14.05.2026 14:42](https://www.youtube.com/watch?v=A6zgTaxo3R4&lc=Ugw3rJkZwboFOUC4OqV4AaABAg) (ред. 14.05.2026 15:43)*

Разве async/await - это синтаксический сахар над генераторами? Может я не туда смотрю, но согласно той же спецификации async/await и генераторы - это две независимые друг от друга конструкции, хоть и используют похожий механизм приостановки текущего execution context и его подальшее возобновление (27.7.5.1 AsyncFunctionStart, 27.7.5.3 Await, 27.5.3.1 GeneratorStart). Раньше, до появления встроенной поддержки async/await браузерами, действительно такие транспайлеры как Babel транспилировали async/await через генераторы. Но сейчас они никак не связаны между собой, хоть и концептуально похожи.

UPD: Все зависит от реализации async/await движком. Например, как показано в видео на 13:06, V8 похоже переиспользует байт-код генераторов.

---
