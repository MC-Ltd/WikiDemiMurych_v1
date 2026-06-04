---
title: "⎡coding:12-3⎦ LeetCode: 30 JavaScript задач за 30 часов - Part3 - JavaScript Live Coding."
date: 2023-11-25
tags: []
videoId: "_su4lhLXwfk"
duration: "5:22:01"
views: 4545
likes: 121
comments: 15
---
# [⎡coding:12-3⎦ LeetCode: 30 JavaScript задач за 30 часов - Part3 - JavaScript Live Coding.](https://www.youtube.com/watch?v=_su4lhLXwfk)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 25.11.2023 09:38  
**Тривалість:** 5:22:01  
**Перегляди:** 4545 · **Лайки:** 121 · **Коментарі:** 15
![thumbnail](https://i.ytimg.com/vi/_su4lhLXwfk/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=_su4lhLXwfk)
## Коментарі (11 · відповідей: 4)

**[@kdwyd](https://www.youtube.com/channel/UCx-uJnbNl2aRsEd7CQrH7Rw)** *[26.11.2023 07:44](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=UgxsHggbQS5jYhSJ0DJ4AaABAg) · 👍 1*

Привет! 
А есть возможность звука прибавить в след. раз? Без наушников с ноутбука прям вслушиваться приходиться, да и в наушниках с телефона на полную громкость приходится делать.

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[27.11.2023 21:17](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=UgxsHggbQS5jYhSJ0DJ4AaABAg.9xZzujanLOD9xd0k0frXa_) · 👍 1*

> Конечно. Вроде бы на самом стриме я спрашиваю все ли хорошо слышно. Но видимо этого не достаточно

---

**[@alexandroppolus](https://www.youtube.com/channel/UCMuGh1mA8uzJeO-LLN8KdRw)** *[27.11.2023 02:17](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=UgyLGxY4Sh7KOCAI17d4AaABAg) (ред. 27.11.2023 17:48)*

Мурыч, привет! Предлагаю челлендж:

var a = [ function() { console.log(this, arguments); }, 'thisObj', 1, 2, '3', [4], {}, 5 ]; // a[0] - нестрелочная функция, остальное произвольно
a[0].apply(a[1], a.slice(2))

Можешь ли ты переписать вторую строку так, чтобы её длина была менее 20 символов? В рамках стандартной библиотеки JS, не меняя первую строку и не добавляя иные.

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[27.11.2023 21:14](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=UgyLGxY4Sh7KOCAI17d4AaABAg.9xazEifvOnA9xd0RIAV1xs) (ред. 27.11.2023 21:23)*

> Я не люблю бессмысленные задачи. О них скучно думать, а что еще важнее - бесполезно.
> Если на вскидку то это решается образом, подобным этому:
> a[0].bind.call( ...a )``
> тут 24 символа, но я не вижу необходимости думать над тем как сэкономить 4 символа,  потому как задача скучная, а самое главное бесполезная - то есть не имеет никакого практического применения в рамках заданого условия (сэкономить символы в строке)
> 
> Дайте мне мотивацию чтобы решать это. Сейчас я ее не вижу. Кроме того, я явным образом показал Вам те идеи при помощи которых эта задача решается.

---

**[@leon83935](https://www.youtube.com/channel/UCQWoq45oCaF2rcWStxBAnYA)** *[27.11.2023 16:49](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=UgwMCvdQJurhLdW4pE94AaABAg) · 👍 2*

аудитория растёт, задачки щёлкаем

---

**[@aleksandrm3466](https://www.youtube.com/channel/UCiCp-Kghn28Lf86Caidskcg)** *[27.11.2023 23:33](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=UgzYJAHET3jo0N1wQot4AaABAg) · 👍 2*

Спасибо за новые знания. Разбор reduce просто пушка

---

**[@Sergiypsm](https://www.youtube.com/channel/UCucfiBOcj7ZJnE1hHcdvpuQ)** *[28.11.2023 10:36](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=Ugz0eZNWSv4XNy1Sewx4AaABAg)*

arr = [1, 2, 3, 4, 5, 6, 7]

n = 1
const result = arr.reduce((acc, _, i, arr) => {
    acc.push(arr.slice(n * i, n * (i + 1)));
    return acc
}, []).filter(e => e.length)


console.log(result);

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[30.11.2023 23:25](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=Ugz0eZNWSv4XNy1Sewx4AaABAg.9xeS7fme9hz9xkyoHB7uR_) · 👍 1*

> У этого решения есть одна большая проблема, которая связана с тем, как V8 или любой другой RunTime будет выделять память под Exotic Object Array при каждом новом push.
> 
> Точнее, не при каждом, а в случае когда он будет подходить к границе выделенной под текущую структуру. 
> 
> И именно с этой точки начинается решение этой задача на уровне Performance, До этого это просто жанглирование разными возможностями языка.

---

**[@UncaughtTypeError](https://www.youtube.com/channel/UCr9tEQyff-tk8xa_0Dvcb0A)** *[08.12.2023 22:36](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=UgzUg3t_Z1BCHWqowmR4AaABAg)*

Так що там з promiseAll? А то я мабуть загубив або прослухав. 
Бо в мене вийшло вирішити це завдання. Но я зовсім не впевнений що це те рішення яке є тим що потрібно. Бо воно виглядає як на мене більш перевантаженим і за кількості викликів then.

```
var promiseAll = (values) => values.reduce((all, call) => call().then((value) => all.then((next) => next.concat(value))), Promise.resolve([]));
```

Є вірне рішення? Хотілось би побачити.

---

**[@RichardLofty](https://www.youtube.com/channel/UCP--aGcyo4a_dfi7K2CszKg)** *[13.12.2023 12:55](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=Ugz_tE_g-VZFN-IUh_h4AaABAg) · 👍 1*

Приветствую, Мурыч.
У тебя ошибка в фундаментальной присупозиции.
Проекты по обучению людей определенным методом, абсолютно спокойно могут не выстреливать, при этом имея самую лучшую стратегию и методологию обучения.
На данный момент интернет переполнен информацией и рекламой.
И есть абсолютная куча примеров, объективно плохих проектов, которые становятся популярными, а иногда вообще мейнстримными.
Делают это ни тупо за счет рекламы.
Даже если создать лучший проект в мире, если за потоками шлака в интернете его не будет видно, то он просто умрет, и останется никому не известным ине нужным.
К сожалению сейчас так работает все, что связано с распространением информации.
Среднестатистический JS программист смотрит за неделю сотни а то и тысячи кринжовых тиктоков с откровенно ложной информацией о том же JS.
Только органичное продвижение или реклама могут хоть как то вдолбить обычному программисту что "круто знать как правильно на самом деле все работает".

> **[@RichardLofty](https://www.youtube.com/channel/UCP--aGcyo4a_dfi7K2CszKg)** *[13.12.2023 13:06](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=Ugz_tE_g-VZFN-IUh_h4AaABAg.9yGJyREz7h29yGLIjXUxbQ) (ред. 13.12.2023 13:07) · 👍 1*

> И это только одна сторона ситуации.
> А есть и вторая.
> Самая важная!
> Пока не изменится отношение потребителя - ничего не поменяется.
> Пока юзеры сайтов, не начнут отказываться, из принцыпа, пользоваться теми или иными сервисами, из-за того что они слишком много жрут, лагают или просто криво работают, пока это не начнет массово происходить, массовый отказ - бунт юзеров, бизнесу будет плевать, ибо ему не выгодно тратить время на правильность кода, когда можно запилить новую фичу и получать деньги за день, вместо денели.
> Только спрос способен повлиять на бизнес, и тем самым на продукт.
> Сейчас развелось такое количество "вкатунов" именно потому что бизнесы готовы нанимать любую обезьяну, лишь бы иногда то что она пишет приносило деньги, и хоть как-то работало.

---

**[@RichardLofty](https://www.youtube.com/channel/UCP--aGcyo4a_dfi7K2CszKg)** *[13.12.2023 13:21](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=Ugwk_4H7iYMIFQzDN0J4AaABAg) · 👍 1*

У задач в литкоде нету никакой высшей идеи или мысли.
Скорее всего сами задачи были сделаны одними людьми, а их описание поручено другим людям.
В итоге получается дымящийся кал.
А сами задачи, просто каждый раз проверяют твое знание каких то встроенных методов или апи.

---

**[@dmitrytkach8650](https://www.youtube.com/channel/UC1fJ36aEqrQ5W6rTlgDL3ug)** *[19.12.2023 03:25](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=UgzlGr1OM6Ab3sxR22t4AaABAg) (ред. 19.12.2023 03:34)*

Мурыч, привет! Вот такое решение накидал для Chank array. 
Может не идеально но идея была вот такая,

const chank = (arr, size)=> {
    const group = new RegExp(`\\d{1,${size}}`, 'g');
    return arr
         .join("")
         .match(group) // =>['312', '452', '758', '432', '1']
         .map(val=>[val]);
}
chank([3,1,2,4,5,2,7,5,8,4,3,2,1], 3);

result: [ ["312"],["452"],["758"],["432"],["1"] ]

---

**[@Sergei546](https://www.youtube.com/channel/UCkIbOOnDXfE32PYAsMQs6Qg)** *[04.04.2024 14:37](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=UgxNiz6C3rz2SQtxXXp4AaABAg)*

контент просто супер. смотрю 3 часть. 12 часов красоты 1 и 2 часть уже позади ехуу

---

**[@Sergei546](https://www.youtube.com/channel/UCkIbOOnDXfE32PYAsMQs6Qg)** *[12.04.2024 15:59](https://www.youtube.com/watch?v=_su4lhLXwfk&lc=UgyCGycznHeBv-5ektN4AaABAg) (ред. 12.04.2024 16:26)*

в этом видео было 2 ошибки у литкода, тесты падали на ваши решения, теперь их нет по вашим решениям, починили литкод

---
