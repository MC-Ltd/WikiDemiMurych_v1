---
title: "Мне нужно знать о JavaScript: ArisenRising"
date: 2024-11-08
tags: ["intk", "0", "js", "qst", "opti"]
videoId: "wYHO3UcHyBY"
duration: "1:34:20"
views: 6552
likes: 269
comments: 20
---
# [Мне нужно знать о JavaScript: ArisenRising](https://www.youtube.com/watch?v=wYHO3UcHyBY)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 08.11.2024 07:26  
**Тривалість:** 1:34:20  
**Перегляди:** 6552 · **Лайки:** 269 · **Коментарі:** 20
![thumbnail](https://i.ytimg.com/vi/wYHO3UcHyBY/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=wYHO3UcHyBY)
## Коментарі (13 · відповідей: 7)

**[@aleksandr2245](https://www.youtube.com/channel/UCk_nD0EDscNtiWPaJgRPPGw)** *[07.11.2024 20:53](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgyGmRzvblvJHWzEdsF4AaABAg) · 👍 13*

йоу, Мурыч, надеюсь ты уже лучше себя чувствуешь, спасибо за стрим

---

**[@alekseypavlov2539](https://www.youtube.com/channel/UCeuKzbNggbgafH3M8LyPbmA)** *[07.11.2024 23:24](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgyX2H4Ab8Yi7kJsz2B4AaABAg) (ред. 07.11.2024 23:29) · 👍 1*

Спасибо за стрим. 

Образно говоря вот что твориться с данными:

let counter = 0

const indificators = {}
const heap = {}

function createHeapValue(indifcatorCode, value) {
    const heapCode = '0x0' + ++counter

    let findValue = null

    for (const heapCode in heap) {
        if (heap[heapCode].type === typeof value && heap[heapCode].value === value) {
            findValue = heap[heapCode]
            break
        }
    }

    if (findValue) {
        findValue.indifcatorCode.push(indifcatorCode)
    } else {
        heap[heapCode] = {
            type: typeof value,
            value,
            indifcatorCode: [ indifcatorCode ],
        }
    }
}

function createIdificator(declaration, name, operator, value) {
    const indifcatorCode = '0x0' + ++counter

    indificators[indifcatorCode] = {
        declaration,
        name
    }

    createHeapValue(indifcatorCode, value)
}

function getValue(indificatorName) {
    let indificator = null

    for (const indificatorCode in indificators) {
        if (indificators[indificatorCode].name === indificatorName) {
            indificator = {
                code: indificatorCode,
                ...indificators[indificatorCode]
            }
            break
        }
    }

    if (!indificator) return

    for (const heapCode in heap) {
        if (heap[heapCode].indifcatorCode.includes(indificator.code)) {
            return heap[heapCode].value
            break
        }
    }

    return
}

createIdificator('var', 'a', '=', 1)
createIdificator('let', 'b', '=', 2)
createIdificator('const', 'c', '=', 3)
createIdificator('var', 'd', '=', 2)

createIdificator('var', 'e', '=', 4)
createIdificator('var', 'f', '=', getValue('b') + getValue('d'))

function printString(s) {
    console.log(s)
}

createIdificator('empty', 'emptyVarName1', '=', 'Hello, world!')
createIdificator('empty', 'emptyVarName2', '=', 'Hello, world!')
createIdificator('empty', 'emptyVarName3', '=', 'Hello, world!')
createIdificator('empty', 'emptyVarName4', '=', 'Hello, world!')
createIdificator('empty', 'emptyVarName5', '=', 'Hello, world!')

printString('Hello, world!')
printString('Hello, world!')
printString('Hello, world!')
printString('Hello, world!')
printString('Hello, world!')

console.log(indificators, heap)

> **[@centralcat3325](https://www.youtube.com/channel/UCNvwo4DqvFsWSPPqwLCN3og)** *[08.11.2024 14:28](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgyX2H4Ab8Yi7kJsz2B4AaABAg.AAZAKBupasGAA_mjBoPYUj) (ред. 08.11.2024 14:28) · 👍 1*

> @404Negative мурыч с дислексией то есть тебя ничему не научил?) Какую твой комментарий вообще можешь принести пользу

> **[@alekseypavlov2539](https://www.youtube.com/channel/UCeuKzbNggbgafH3M8LyPbmA)** *[08.11.2024 15:23](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgyX2H4Ab8Yi7kJsz2B4AaABAg.AAZAKBupasGAA_t48N62SG) · 👍 1*

> @404Negative ты придрался к коду написанном на коленке из-за названия переменных? Мог вообще a, b, c назвать. И да с английским у меня плохо. Обычно называю переменные если сложно, через google translate, тут это было не к чему.

---

**[@alexms8508](https://www.youtube.com/channel/UCoWpQCE1UUKReJg5b8qTFLQ)** *[08.11.2024 05:01](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=Ugy8mK94NMoDaDyZg8Z4AaABAg) · 👍 3*

Мурыч хорошо что ты вернулся)

---

**[@Stas-ir3gh](https://www.youtube.com/channel/UCoZe3n6A1XF4J1S9yvKS1Lg)** *[08.11.2024 06:33](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgxRE60KaxHPVAU5GMN4AaABAg)*

Ого, живой ещё! Это радует:)

---

**[@antonmahagon6299](https://www.youtube.com/channel/UC6hFaHwoIeaDo0XFnKO6t-g)** *[08.11.2024 11:31](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgxR9bZap_gp0Y3FAh14AaABAg)*

можете отсыпать мнений про esprima: parser ?

> **[@antonmahagon6299](https://www.youtube.com/channel/UC6hFaHwoIeaDo0XFnKO6t-g)** *[08.11.2024 11:36](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgxR9bZap_gp0Y3FAh14AaABAg.AA_TUq70lgLAA_U7RKSVPd)*

> как будто как раз в тему стрима програмулина

---

**[@narek7281](https://www.youtube.com/channel/UCUa3U5-hu8KquLW_b1ubKbA)** *[08.11.2024 20:00](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=Ugy8nAR8dEFiFU0pEFp4AaABAg)*

great video

---

**[@FedorPantyushin](https://www.youtube.com/channel/UCyOv-yErrXOo8nid_QWUpVQ)** *[08.11.2024 21:41](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=Ugz9OoVo_6QyD_alicV4AaABAg)*

Все есть вычислительный объект так сказать ...

---

**[@vladislavburko](https://www.youtube.com/channel/UCIZk0O5J9ZLnCia8FZn8MXQ)** *[08.11.2024 21:44](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgzxJPPixKvEBVqx3gB4AaABAg)*

00:00:01   Введение и цели трансляции
00:01:53   Начало разговора со Святославом
00:05:31   Вопросы и ответы
00:07:24   Спецификация JavaScript
00:11:04   Оптимизация и абстракции
00:17:33   Плюсы и минусы работы с данными
00:19:17   Работа с переменными в JavaScript
00:26:03   Внутреннее представление данных
00:30:22   Оптимизация и производительность
00:38:01   Пример с объектом и возрастом
00:40:47   Оптимизация работы с числами
00:43:19   Пример с функцией и идентификатором
00:47:32   Пример с экзотическим объектом
00:50:41   Спецификация и команды языка
00:56:19   Понимание идентификаторов и команд
00:58:12   Команды и литералы
00:59:09   Оптимизация работы с литералами
01:01:03   Анбоксинг
01:04:31   Куча и структура данных
01:10:56   Оптимизация циклов
01:16:20   Введение в JavaScript
01:17:15   Работа с данными в JavaScript
01:20:22   Оптимизация массивов
01:25:08   Спекулятивная оптимизация
01:31:01   Заключение

---

**[@kookaburru](https://www.youtube.com/channel/UChqpH14IXFRhgWvd1HWe6Fw)** *[12.11.2024 09:54](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgySa3umcmXvZt-lUTF4AaABAg) · 👍 2*

Мурыч заморочил чуваку голову с инструкциями 😂
Чел я ща объясню тебе все проще, цифры 1,2,3 и т.п. это все объекты в памяти с которыми связываются идентификаторы (переменые). С объектом может связываться более одного идентификатора. Когда с объектом не связан ни один идентификатор, объект будет удален сборщиком мусора все! Плевать на то что var, let или const это инструкции 😊

> **[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[13.11.2024 22:23](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgySa3umcmXvZt-lUTF4AaABAg.AAjaXXHFG86AAnW75s1yPN) · 👍 1*

> если обьект не связан ни с одним идентификатором - он не обязательно может быть удален сборщиком мусора, но может быть удален.
> 
> например строки, удаляются сборщиком в самую последнюю очередь и то только в ситуации если требуется память и ее больше негде взять.

---

**[@ArteEtMarte](https://www.youtube.com/channel/UC40NscIeVMaG46n2dkT11Ww)** *[02.01.2025 03:11](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=Ugyha8bdKbAJSdjPkmV4AaABAg)*

Вы как то негативно отзывались о Haskell. Чем он вас разочаровал? Хочу начать на нем разработку игры для души, но не совсем понимаю с чем столкнусь. Жопой чую кучу нюансов которые возникнут как с каким-нибудь Prolog, от которого тоже первое впечатление было - восторг, а потом как началось... Впрочем он все равно остался одним из любимых.

У Haskell, судя по бенчмаркам, хорошее быстродействие, небольшой оверхед на ffi и есть, вроде, неплохо работающая обертка для Vulkan.

Я смотрю на Haskell с его ленивыми вычислениями... как на нем записывают алгоритмы... На энергичных яп когда реализуешь сколь-нибудь сложный алгоритм приходится прям выворачивать его наизнанку, писать обертки чтобы никаких лишних доп вычислений или обходов дерева/коллекций небыло, чтобы не выросла его асимптотическая сложность. И за этими всем потом трудно распознать сам алгоритм... В Haskell же часто записывают алгоритм как есть, быть может, с небольшой модификацией, чтобы thunk'ов не накапливалось, а всю работу по минимизации вычислений делает ленивая стратегия. И это прям впечатляет! Так же ленивые вычисления позволяют управлять вычислением аргументов, что, судя по всему, делает их альтернативой макросам лиспов как минимум в большинстве случаев. Да и синтаксис Haskell - лаконичный, компактный, последовательный по сравнению с другими яп, с крутой деструктуризацей значений, кастомными операторами... На другие яп после Haskell смотришь и там прям насрано: все эти this, обращения через точку, запятые и скобочки при вызове ф-ции, не несущие особой смысловой нагрузки, но замусоривающие код... мне кажется, что это очень важно, чтобы единицы кода на экране были компактными, чтобы их можно было воспринять буквально за минимальное число фиксаций взгляда или чтобы как можно больше кода воспринималось за один взгляд т.к. не раз сталкивался с ситуациями когда отчетливо видно было, что мозг и его возможности много больше сознательной части, оперативной памяти или внимания, а наша зрительная система определенно имеет самую высокую пропускную способность: часто можно тупить глядя в код и решение приходит, хотя кажется и не думал вовсе.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[27.01.2025 18:01](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=Ugyha8bdKbAJSdjPkmV4AaABAg.ACmBzktMp50ADo9jFJasl0)*

> Напротив.
> Я не негативно к нему отношусь. Я сожалею что он никогда не станет мейнстримом.
> 
> Популярность языка формируется не его совершенством.

---

**[@aleksandrm3466](https://www.youtube.com/channel/UCiCp-Kghn28Lf86Caidskcg)** *[29.03.2025 17:59](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgyqgOzFBikq6RUthqx4AaABAg)*

​ @demimurych1,  Можно ли утверждать, что литералы на разных этапах работы движка ведут себя по разному: как струкруры (коробочки), как примитив/ссылочный тип (10, [1,2,3])? Например: такое выражение, var a = 10, на этапе на момент парсинга и построения AST - структура { type: "Literal", value: 10 }, но в рантайме как примитив small integer 10? Или структура остается?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[18.04.2025 19:13](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgyqgOzFBikq6RUthqx4AaABAg.AGGDzmsWEsYAH3rOwdLBe6)*

> Безусловно. Все современные, популярные Агенты исполняющие JS код, пытаются работу с литералами оптимизировать во всех возможных формах. 
> 
> Происходит это потому, что литерал сразу сообщает Анегнту чем он является и, как следствие, как с ним можно работать.
> 
> Одновременно с этим очень важно помнить - где наши знания о том как работает Агнет (например V8) а где спецификация языка. Потому как в вопросах оптимизации кода, даже спецификацию могут нарушать так как вздумается инженерам Агента.
> 
> Иными словами, если строить пирамиду профессиональности JS программиста, то первое с чего он должен начинать (фундамент) это спецификация. В настоящий же момент - это в лучшем случае каша из разных приемов которые были когда-то эффективными и на слуху.

---

**[@astrobrite540](https://www.youtube.com/channel/UC4D058sPZcXUR8ukz2ZlLIw)** *[12.04.2025 00:25](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgzftRoMEetkRkPRGd54AaABAg)*

Дякую за чудове пояснення за анбоксінг! Але як буде виконуватись якщо на  1:19:03 використати == ?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[18.04.2025 19:05](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=UgzftRoMEetkRkPRGd54AaABAg.AGnOWBjKEScAH3qStA5L9R)*

> Это очень хороший вопрос, который раскрывается в том случае, когда мы рассматриваем множество примеров разного сравнения.
> 
> Если говорить о самому универсальном и простом для восприятия способа не сильно думать о проблемах с производительностью, для современного V8 - то лучше всего использовать везде и всегда НЕСТРОГОЕ сравнение. 
> 
> Но при этом, Вы получаете код, который в большей степени зависит от Вашей экспертизы (когда вы точно знаете что и как будет сравниваться) и как следствие, его надежность будет уже в большей степени зависеть от вас. 
> 
> Когда-то давно, больше 5 лет назад, использования строго сравнения действительно гарантировало преимущество.  Например myVariable === undefined работало быстрее чем myVariable == undefined. Однако, те времена, для V8 в прошлом. По крайней мере пока.

---

**[@СергейЯкушев-ы9о](https://www.youtube.com/channel/UCGs0thI5RPbVIjs0JVY8v_A)** *[24.04.2025 11:51](https://www.youtube.com/watch?v=wYHO3UcHyBY&lc=Ugy8EQuMYfGPojx3_H54AaABAg)*

Скиньте пожалуйста ссылку на книгу мурыча

---
