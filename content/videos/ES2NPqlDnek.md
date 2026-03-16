---
title: "В живую с Виталий Николаевичем Брагилевским и Тимуром ибн Джафаром"
date: 2025-10-04
tags: ["dlgs", "14", "js", "bragilevsky", "tumur", "paradigms"]
videoId: "ES2NPqlDnek"
duration: "3:02:31"
views: 5053
likes: 159
comments: 53
---
# [В живую с Виталий Николаевичем Брагилевским и Тимуром ибн Джафаром](https://www.youtube.com/watch?v=ES2NPqlDnek)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 04.10.2025 18:11  
**Тривалість:** 3:02:31  
**Перегляди:** 5053 · **Лайки:** 159 · **Коментарі:** 53
![thumbnail](https://i.ytimg.com/vi/ES2NPqlDnek/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=ES2NPqlDnek)
## Коментарі (21 · відповідей: 32)

**[@TimurShemsedinov](https://www.youtube.com/channel/UChSGI2R2kRMjzXJuYqHWQZg)** *[04.10.2025 18:19](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwvAqGpB1f-7vA5cPR4AaABAg) · 👍 20*

Мы в этот раз не отвечали на вопросы, но их можно задавать тут под видео, как минимум, я постараюсь ответить на все, сколько будет сил

> **[@boycovclub](https://www.youtube.com/channel/UCxbDPizEG96FDSCQ8JFpFRA)** *[04.10.2025 19:07](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwvAqGpB1f-7vA5cPR4AaABAg.ANrvYdrVoh1ANs0-BtbGhM) (ред. 04.10.2025 19:07) · 👍 3*

> Не перебивайте пожалуйста участников) это единственная просьба, вы сбиваете с мыслей. ФП это лучшая парадигма и не спорьте пожалуйста))

> **[@boycovclub](https://www.youtube.com/channel/UCxbDPizEG96FDSCQ8JFpFRA)** *[04.10.2025 19:34](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwvAqGpB1f-7vA5cPR4AaABAg.ANrvYdrVoh1ANs38edaW9s)*

> С вами не согласен, от того что я на классах напишу Функтор от этого он ООП не станет, вот вам пример с моего курса
> ```
>           // Сигнатура
>           fantasy-land/map :: Functor f => f a ~> (a -> b) -> f b
> 
>           // Создание функтора
>           // ==== синтаксис es5 ======
> 
>           // подготавливаем прототип для функции конструктора
>           // удалив наследование Object.prototype дефолтная
>           var prototypeFunctor = Object.create(null)
> 
>           // Название строки функции и метода согласно спецификации
>           const FANTASY_LAND_MAP = 'fantasy-land/map'
> 
>           // создаем функцию конструктор
>           function Functor(value) {
>             this.value = value
>           }
> 
>           // создаем правильные связи между прототипом и функций конструктором
>           Functor.prototype = prototypeFunctor
>           prototypeFunctor.constructor = Functor
> 
>           //  а вот теперь самое главное реализовываем интерфейс функтора
>           prototypeFunctor[FANTASY_LAND_MAP] = function (fn) {
>             return new Functor(fn(this.value))
>           }
> 
>           // Давайте разделим ключевую логику на части
>           // return new Functor(fn(this.value))
>           // 1. Текущей содержимое контейнера мы пропускаем через функцию
>           fn(this.value)
>           // 2. Возвращаем новый экземпляр типа функтор уже с новым значением
>           return new Functor(тут результат инструкции выше)
> 
>           // Пример
>           var functorObj = new Functor(5)
> 
>           var functorResult = functorObj[FANTASY_LAND_MAP](value => value * 2)
> 
>           // отсутствуют мутации
>           // реализован интерфейс спецификации
>           console.log(functorObj.value) // 5
>           console.log(functorResult.value) // 10
> 
>           // =========================
> 
>           // Полифил
>           // как устроен примерно внутри Object.create(objectProto)
>           var createObjectProto = function (obj) {
>             // для создания экземпляра формируем конструктор
>             function XXX() {}
> 
>             // устанавливаем правильные ссылки
>             XXX.prototype = obj || Object.prototype
>             XXX.prototype.constructor = XXX
> 
>             // создаем экземпляр и возвращаем
>             return new XXX()
>           }
> 
>           // ==== синтаксис es6 ======
>           // тут все гораздо проще
>           // тут в прототипе мы также можем уничтожить дефолтное наследование Object.prototype
>           class Functor {
>             constructor (value) {
>               this.value = value
>             }
> 
>             // этот метод и так уже будет хранится по дефолту в прототипе
>             [FANTASY_LAND_MAP] (fn) {
>               return new Functor(fn(this.value))
>             }
>           }
> 
>           // Пример описанный выше также сработает
>           const functorObj = new Functor(5)
>           // =========================
> 
> 
>           // ==== через чистые функции ======
>           // Создание функтора без создания экземпляров
>           // через чистые функции
>           const functor = value => ({
>             value,
>             [FANTASY_LAND_MAP]: (fn) => functor(fn(value))
>           })
> 
>           // создали объект и вернули его
>           const objA = functor(10)
>           const objB = objA[FANTASY_LAND_MAP](value => value - 5)
> 
>           console.log(objA.value) // 10
>           console.log(objB.value) // 5
> 
>           // =========================
> ```

> **[@TimurShemsedinov](https://www.youtube.com/channel/UChSGI2R2kRMjzXJuYqHWQZg)** *[04.10.2025 20:14](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwvAqGpB1f-7vA5cPR4AaABAg.ANrvYdrVoh1ANs7csBL8tH)*

> @boycovclub я буду перебивать, следующий вопрос ))

> **[@ApelsinovIvan](https://www.youtube.com/channel/UCW6wj4toLJXlb1VFzdnwkkA)** *[04.10.2025 20:55](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwvAqGpB1f-7vA5cPR4AaABAg.ANrvYdrVoh1ANsCPEd0Zqm)*

> А где взять примеры кода на разных парадигмах, о которых вы говорили на стриме?

> **[@TimurShemsedinov](https://www.youtube.com/channel/UChSGI2R2kRMjzXJuYqHWQZg)** *[04.10.2025 22:30](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwvAqGpB1f-7vA5cPR4AaABAg.ANrvYdrVoh1ANsNFpIz3op)*

> @ApelsinovIvan github HowProgrammingWorks Paradigms

> **[@muradocaq3464](https://www.youtube.com/channel/UCDzrjV6q--9iPMe5ntcojZg)** *[05.10.2025 06:53](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwvAqGpB1f-7vA5cPR4AaABAg.ANrvYdrVoh1ANtGmYoJRar) (ред. 05.10.2025 06:57)*

> Как раз добавлял Grady Booch в список литературы по ООП, и если эта книга уже устарела, то какую бы литературу порекомендовали бы?

> **[@alexsoomo7029](https://www.youtube.com/channel/UColHveA0RJ-POgzkp6UaMtw)** *[05.10.2025 07:59](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwvAqGpB1f-7vA5cPR4AaABAg.ANrvYdrVoh1ANtOMsfVrvP) · 👍 3*

> Почему только 3часа где остальные 5 часов? Неужели так сложно сделать полное видео? <3

> **[@TimurShemsedinov](https://www.youtube.com/channel/UChSGI2R2kRMjzXJuYqHWQZg)** *[05.10.2025 08:31](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwvAqGpB1f-7vA5cPR4AaABAg.ANrvYdrVoh1ANtRyZcHRpc)*

> @alexsoomo7029 У меня есть режисерская версия на 3 часа 15 минут

> **[@ilyawebdev](https://www.youtube.com/channel/UC-0sV6Q53HpQQ4GnUHCkVGg)** *[05.10.2025 12:32](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwvAqGpB1f-7vA5cPR4AaABAg.ANrvYdrVoh1ANtseBkf2Fx) · 👍 1*

> да, надо давать закончить мысль и не говорить всем сразу, иначе эти скачки с одного на другое сбивают с толку

> **[@TimurShemsedinov](https://www.youtube.com/channel/UChSGI2R2kRMjzXJuYqHWQZg)** *[05.10.2025 14:26](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwvAqGpB1f-7vA5cPR4AaABAg.ANrvYdrVoh1ANu4baDiFys)*

> @muradocaq3464 Все можно читать, но помнить, но подвергать сомнению, сейчас вся классика уже устарела, а новой не написали, с адаптацией ооп и паттернов на современный js и есть мои лекции, я бы и книгу написал, но книги люди уже не читают, разучились

> **[@dekorzh-y4m](https://www.youtube.com/channel/UCVLjoMfjex7gfjTWfN0Lgwg)** *[05.10.2025 17:44](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwvAqGpB1f-7vA5cPR4AaABAg.ANrvYdrVoh1ANuRJPkjdIk)*

> Тоже бесят эти шорцы

> **[@Son0fBeelzebub](https://www.youtube.com/channel/UChVbSVULfjhPqc1ZhiIXglg)** *[29.10.2025 06:40](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwvAqGpB1f-7vA5cPR4AaABAg.ANrvYdrVoh1AOr2N1wzCpf)*

> забавно, как мы обсуділі тему на прошлом стріме, что сінтакс не важен, еслі семантіка та же, а в ітоге на этом стріме вы поднялі эту же тему с самого начала, жаль, что её чуток сільнее не раскрутілі

---

**[@evgenygazdovsky](https://www.youtube.com/channel/UC3dr-LUCkVe0r3Hb_tLlLeA)** *[04.10.2025 18:34](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgxfwIAhxuEKBJm79tF4AaABAg) (ред. 04.10.2025 18:45) · 👍 1*

Для того чтобы говорить о парадигмах или стилях нужно зафиксировать точку относительно чего рассматривается парадигма! Один и тот же код на любом языке может одновременно являться и императивным и декларативным и функциональным. Зависит с какой стороны посмотреть. Например с точки зрения решаемой задачи императивный, а с точки зрения компилятора уже декларативный. А может и наоборот, для нас декларативный код, а для интерпретатора – функциональный! А то же самое мутабельное присваивание может оказаться иммутабельной функцией ;) ой как может!

---

**[@evgenygazdovsky](https://www.youtube.com/channel/UC3dr-LUCkVe0r3Hb_tLlLeA)** *[04.10.2025 18:46](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugzx50WjQJIVp9iECoR4AaABAg) · 👍 4*

Хорошо посидели! Респект Мурычу за Стругацких!

---

**[@АнтонСтасюк-е4р](https://www.youtube.com/channel/UCKmq4XhZnA27eJh-fM8L5yg)** *[04.10.2025 19:04](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugxu8BNsHb--5KZxQhd4AaABAg) (ред. 04.10.2025 19:05) · 👍 9*

Огонь трансляция, но как же у Мурыча горит, что не всегда он прав, и не всем нужна низкоуровневость и скорость )

> **[@nonamenobody2795](https://www.youtube.com/channel/UCGTmhHsw0FjMBz6Jr8WhmbQ)** *[05.10.2025 05:02](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugxu8BNsHb--5KZxQhd4AaABAg.ANs-bwb12u-ANt45xbHzEV) · 👍 1*

> нужна, но не все об этом задумываются.

> **[@sergeyab9468](https://www.youtube.com/channel/UCqa6oa2gZWRb9Bty1a6-ZlQ)** *[06.10.2025 04:14](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugxu8BNsHb--5KZxQhd4AaABAg.ANs-bwb12u-ANvZOitJVBv) · 👍 2*

> Она нужна но не в том плане что все думают. Просто Мурыч представитель этой стороны он ее и представляет. Понимаешь если бы была не нужна то и Мурыча бы не было просто сидел бы себе кодил и молчал. А так получается выходит в тренды ютуба - почему? Ну мое объяснение 1) запрос на это есть 2) хайп после спора с Соером 3) Он предлагает то что мало кто предлагает на ру ютубе нижнего ИТ сигмента ну и 4 и самое главное - вообще то речь не о том низкий ли уровень и какая скорость а речь о том как человек (любой) подходит к проблеме, будет ли он пытаться решать ее фундаментально (да возьми ту же информатику и математику за фундамент) или решать так как умеет. Если человек понимает что ему нужна база (не вся а скажем, математическая для того, архитектурная для сего и т.д.) то он будет стремиться ее освоить и применять а если не понимает (или она ему и правда не нужна) то он будет подходить к проблеме как умеет. Вот об этом Мурыч и говорит что она ВСЕМ нужна на самом деле. Да, он вроде понимает что не прям сейчас и не прям всем но он говорит что к ней надо стремиться и хотябы понимать что такое вообще БАЗА почему база и зачем база. Вот

---

**[@alexanderwebdev5558](https://www.youtube.com/channel/UCIsRZSmX2N2mhll3PfXaUWg)** *[04.10.2025 19:23](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugych0rPdiZHGevK8cl4AaABAg) · 👍 2*

This is a great video, very interesting.

---

**[@boycovclub](https://www.youtube.com/channel/UCxbDPizEG96FDSCQ8JFpFRA)** *[04.10.2025 19:32](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgzuhDNiN66YxVNMg6R4AaABAg)*

С вами не согласен, от того что я на классах напишу Функтор от этого он ООП не станет, вот вам пример с моего курса
```
          // Сигнатура
          fantasy-land/map :: Functor f => f a ~> (a -> b) -> f b

          // Создание функтора
          // ==== синтаксис es5 ======

          // подготавливаем прототип для функции конструктора
          // удалив наследование Object.prototype дефолтная
          var prototypeFunctor = Object.create(null)

          // Название строки функции и метода согласно спецификации
          const FANTASY_LAND_MAP = 'fantasy-land/map'

          // создаем функцию конструктор
          function Functor(value) {
            this.value = value
          }

          // создаем правильные связи между прототипом и функций конструктором
          Functor.prototype = prototypeFunctor
          prototypeFunctor.constructor = Functor

          //  а вот теперь самое главное реализовываем интерфейс функтора
          prototypeFunctor[FANTASY_LAND_MAP] = function (fn) {
            return new Functor(fn(this.value))
          }

          // Давайте разделим ключевую логику на части
          // return new Functor(fn(this.value))
          // 1. Текущей содержимое контейнера мы пропускаем через функцию
          fn(this.value)
          // 2. Возвращаем новый экземпляр типа функтор уже с новым значением
          return new Functor(тут результат инструкции выше)

          // Пример
          var functorObj = new Functor(5)

          var functorResult = functorObj[FANTASY_LAND_MAP](value => value * 2)

          // отсутствуют мутации
          // реализован интерфейс спецификации
          console.log(functorObj.value) // 5
          console.log(functorResult.value) // 10

          // =========================

          // Полифил
          // как устроен примерно внутри Object.create(objectProto)
          var createObjectProto = function (obj) {
            // для создания экземпляра формируем конструктор
            function XXX() {}

            // устанавливаем правильные ссылки
            XXX.prototype = obj || Object.prototype
            XXX.prototype.constructor = XXX

            // создаем экземпляр и возвращаем
            return new XXX()
          }

          // ==== синтаксис es6 ======
          // тут все гораздо проще
          // тут в прототипе мы также можем уничтожить дефолтное наследование Object.prototype
          class Functor {
            constructor (value) {
              this.value = value
            }

            // этот метод и так уже будет хранится по дефолту в прототипе
            [FANTASY_LAND_MAP] (fn) {
              return new Functor(fn(this.value))
            }
          }

          // Пример описанный выше также сработает
          const functorObj = new Functor(5)
          // =========================


          // ==== через чистые функции ======
          // Создание функтора без создания экземпляров
          // через чистые функции
          const functor = value => ({
            value,
            [FANTASY_LAND_MAP]: (fn) => functor(fn(value))
          })

          // создали объект и вернули его
          const objA = functor(10)
          const objB = objA[FANTASY_LAND_MAP](value => value - 5)

          console.log(objA.value) // 10
          console.log(objB.value) // 5

          // =========================
```

---

**[@nonamenobody2795](https://www.youtube.com/channel/UCGTmhHsw0FjMBz6Jr8WhmbQ)** *[05.10.2025 01:56](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgxfP11zD7KH1eKuEP94AaABAg) · 👍 2*

важна не парадигма, а метод

> **[@sergeyab9468](https://www.youtube.com/channel/UCqa6oa2gZWRb9Bty1a6-ZlQ)** *[05.10.2025 11:17](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgxfP11zD7KH1eKuEP94AaABAg.ANsjrP7XSa0ANtk1l0Zm_A) · 👍 1*

> Метод решает все (ну кто не понял я имею ввиду слово метод не функция или свойство в контексте синтаксиса а банально рецепт КАК делать правильно в той или иной ситуации. Метод от слова - методика, алгоритм, проверенный рецепт)

> **[@qwekertarsionov4646](https://www.youtube.com/channel/UCpGSyYe7nE9SBUKF-S0JGzA)** *[05.10.2025 15:35](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgxfP11zD7KH1eKuEP94AaABAg.ANsjrP7XSa0ANuCXwwYYAS)*

> ​@sergeyab9468
> Ии каков он рецепт хорошего кода?
> Вкусный?

> **[@nonamenobody2795](https://www.youtube.com/channel/UCGTmhHsw0FjMBz6Jr8WhmbQ)** *[06.10.2025 03:52](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgxfP11zD7KH1eKuEP94AaABAg.ANsjrP7XSa0ANvWrcoJuE0)*

> @qwekertarsionov4646 к сожалению количество теоретического материала по программированию значительно превосходит качество, поэтому часто понимание приходит только с опытом. желательно жестким. например в одного внести значительные доработки в легаси-проект. через полгода жесткого кодинга по другому смотришь на многие вещи. ФП как метод предоставляет гораздо большие возможности по оптимизации машинного кода чем ООП. Более того методы ФП, такие как монады и мать всех монад - продолжения математически обосновывают эти возможности. Еще могу посоветовать доклад Дона Сайма F# там он как раз говорит что лучше ООП это ОП)). Вообщем, рецепт хорошего кода - это открытость, расширение кругозора и практика.

---

**[@nonamenobody2795](https://www.youtube.com/channel/UCGTmhHsw0FjMBz6Jr8WhmbQ)** *[05.10.2025 02:14](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgxPoIst16Yc69s50yl4AaABAg)*

Брагилевский сам утверждал что производительность это проблема компилятора, а не языка. с другой стороны продолжения (мать всех монад) как раз делают код линейным, что позволяет оптимизировать машинный код. так что вывод однозначный - ФП. и это уже реализовано в Fidelity framework

---

**[@nonamenobody2795](https://www.youtube.com/channel/UCGTmhHsw0FjMBz6Jr8WhmbQ)** *[05.10.2025 02:46](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugzy_MXMlJuZTBI5NyN4AaABAg)*

Функциональное программирование — это стиль программирования, который подчеркивает использование функций и неизменяемых данных. Типизированное функциональное программирование заключается в том, что функциональное программирование сочетается со статическими типами, например с F#. В целом в функциональном программировании выделяются следующие понятия:

Функции в качестве основных конструкций, которые вы используете
Выражения вместо инструкций
Неизменяемые значения по переменным
Декларативное программирование вместо императивного программирования🤣🤣🤣🤣

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[13.10.2025 01:34](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugzy_MXMlJuZTBI5NyN4AaABAg.ANspWLGCA1sAOCIeukJoD4)*

> А как быть с нашим процессором, в котором никаких функций нет?

> **[@nonamenobody2795](https://www.youtube.com/channel/UCGTmhHsw0FjMBz6Jr8WhmbQ)** *[13.10.2025 07:30](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugzy_MXMlJuZTBI5NyN4AaABAg.ANspWLGCA1sAOCwRCiRZ7A)*

> @AsForJS В блоге SpeakEZ Technologies есть интересные мысли на этот счет например одна из статей How Fidelity Solves The Abstract Machine Model Paradox

---

**[@nonamenobody2795](https://www.youtube.com/channel/UCGTmhHsw0FjMBz6Jr8WhmbQ)** *[05.10.2025 02:46](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgzgcYYralhNVF9KJhl4AaABAg) · 👍 2*

Функциональное программирование, как и другие парадигмы программирования, поставляется с словарем, который в конечном итоге потребуется научиться. Ниже приведены некоторые распространенные термины, которые вы увидите все время:

Функция — это конструкция, которая создает выходные данные при указании входных данных. Более формально он сопоставляет элемент из одного набора с другим набором. Этот формализм переводится в конкретное разными способами, особенно при использовании функций, работающих с коллекциями данных. Это самая базовая (и важная) концепция функционального программирования.
Выражение — выражение — это конструкция в коде, который создает значение. В F# это значение должно быть привязано или явно проигнорировано. Выражение может быть тривиально заменено вызовом функции.
Чистота — чистота является свойством функции, так что ее возвращаемое значение всегда совпадает с теми же аргументами, и что его оценка не имеет побочных эффектов. Чистая функция полностью зависит от его аргументов.
Референциальная прозрачность — ссылочная прозрачность — это свойство выражений, которое может быть заменено их выходными данными, не влияя на поведение программы.
Неизменяемость — неизменяемость означает, что значение не может быть изменено на месте. Это отличается от переменных, которые могут измениться на месте.

---

**[@NikitaTimofeenko](https://www.youtube.com/channel/UCJ3GSljMI45-YEyVt0fEOyw)** *[05.10.2025 08:51](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgxXqXQT-V-caW_RkjZ4AaABAg) · 👍 2*

запись топ, но жаль что перебивают постоянно говорящего

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[13.10.2025 01:28](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgxXqXQT-V-caW_RkjZ4AaABAg.ANtULazYivqAOCHzVoJYre)*

> Простите. Не могу усидеть

---

**[@DeadRabbitCanDance](https://www.youtube.com/channel/UC3n-Ic6Vvk9WhoH_KbJGFVw)** *[05.10.2025 11:52](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwOAfIPGt3b2ZTW8R94AaABAg)*

Здравствуйте уважаемые Виталий Николаевич, Тимур ибн Джафар, Мурыч. Спасибо Вам за проведенную лекцию. Было очень интересно.
Вы упомянули то, что в процессе развития языков, новые парадигмы являлись причиной создания новых возможностей языка, а сейчас, когда многие языки включают в себя многие разные парадигмы и позволяют писать программу в различных стилях, само понятие парадигмы размывается. А меня, как пользователя языка программирования, а не философа, наличие парадигм интересует только с той точки зрения, что "парадигма" - это как "рекомендуемая методика".
А вопрос у меня такой. Как можно использовать "парадигмы" или "рекомендуемые методики" при описании желаемого результата разрабатываемого ПО? Может следует рассматривать парадигмы как паттерны? С другой стороны, кроме паттернов есть ещё общепринятые концепции проектирования ПО, и всё это заметьте - не связанные между собой классификации.

Выделяют несколько парадигм программирования:
- императивную, декларативную,
- функциональную
- объектно-ориентированную.

Методы (паттерны) проектирования:
Model-View-Controller MVC
Model-View-Presenter MVP
Model-View-ViewModel MVVM

Реактивное программирование (Reactive Programming) — _это парадигма?_  программирования, ориентированная на реактивные системы, которые реагируют на события, сообщения или внешние стимулы. В отличие от традиционного подхода, где каждое действие должно быть выполнено по порядку, в реактивной модели приложения могут «реагировать» на изменения и события без ожидания завершения предыдущей операции.

Data-oriented design DOD смещает фокус внимания с объектов (объектно-ориентированной парадигмы) на сами данные: тип данных, их расположение в памяти, способы их считывания и обработки.

Системы, построенные на микросервисах, — это системы, где приложение состоит из множества небольших автономных сервисов, каждый из которых выполняет свою конкретную задачу. Такой подход называется микросервисной архитектурой (microservices architecture, MSA). 

И отдельно идут прижившиеся в практике методики и практики, которые получили свои названия и теперь нет необходимости каждый раз пере-изобретать и пере-описывать эти методики. Тут наверно можно все паттерны перечислить и добавить новых. 

HashMap (хеш-таблица) — основа многих алгоритмов, связанных с хранением и извлечением данных в формате «ключ-значение». Эта структура данных позволяет быстро получать значение по ключу, в отличие от массивов или списков, где для поиска элемента может потребоваться перебор всей структуры.

Контейнеры инверсии зависимостей (IoC-контейнеры) — это специальные объекты-сборщики, которые на основании схемы зависимостей между классами и абстракциями создают граф объектов. Любой IoC-контейнер реализует принцип инверсии зависимостей.

И так далее... Как эти сведения можно структурировать и использовать в проектировании нового ПО?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[13.10.2025 01:55](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwOAfIPGt3b2ZTW8R94AaABAg.ANto3LpiqvgAOCL45U2ya8)*

> Я (Мурыч) не знаю. 
> Лично для себя, я вывел правило, что код нужно писать так, чтобы не было мучительно больно его переписывать.

> **[@DeadRabbitCanDance](https://www.youtube.com/channel/UC3n-Ic6Vvk9WhoH_KbJGFVw)** *[13.10.2025 07:59](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwOAfIPGt3b2ZTW8R94AaABAg.ANto3LpiqvgAOCzi3YTp3Q)*

> @AsForJS Правило конечно хорошее. Но уж очень абстрактное. "Не греши, сын мой! Не пиши кода непонятного, неразумного, перегруженного или исключительно ситуативного".
> 
> При Вашем то громадном опыте, должны сформироваться некие представления о том, какие методики способствуют правильному проектированию, а какие являются признаками того, что конструкция теряет устойчивость и вот-вот начнёт разваливаться.

---

**[@rvant](https://www.youtube.com/channel/UCFRo5LsZzosh2JnAv_QYEJw)** *[05.10.2025 18:39](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugx0gmOIfBEH6A6GScZ4AaABAg) · 👍 1*

Чи вірно я зрозумів, що ми можемо використовувати в одному проекті best practices, які можемо взяти з кожної з парадигм. Наприклад з функціонального ми можемо заадоптити, як мінімум чисті функції?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[13.10.2025 01:25](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugx0gmOIfBEH6A6GScZ4AaABAg.ANuXdA9xZFMAOCHd1s1rl0)*

> Звісно. Якщо для вашої команди це прийнятно.

---

**[@nonamenobody2795](https://www.youtube.com/channel/UCGTmhHsw0FjMBz6Jr8WhmbQ)** *[06.10.2025 07:54](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwfWCUH10DoYIa5UHd4AaABAg) (ред. 07.10.2025 00:00)*

MLIR развивает концепцию SSA

В 1998 году Эндрю Аппель опубликовал статью , ознаменовавшую собой изменение нашего подхода к проектированию компиляторов. В статье «SSA — это функциональное программирование» было показано, что статическая форма с одинарным присваиванием, промежуточное представление, лежащее в основе современных оптимизирующих компиляторов, в точности эквивалентна функциональному программированию с вложенной лексической областью действия. Это понимание имеет глубокие последствия в условиях вступающей в новую эру совместного проектирования аппаратного и программного обеспечения.

Суть объединения работы Эппеля с современным MLIR заключается в следующем:

Функциональное программирование — это не высокоуровневая абстракция, которую нужно компилировать, а естественная структура эффективной компиляции.
Речь идёт не о навязывании функционального программирования при разработке систем. Речь идёт о признании того, что наиболее эффективные представления компиляции (SSA в MLIR) изначально функциональны, что делает функциональные языки естественным выбором для стратегии достижения производительности MLIR.

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[13.10.2025 01:31](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwfWCUH10DoYIa5UHd4AaABAg.ANvxaVRSEumAOCIG0hoa8v) · 👍 1*

> Как Вы думаете, когда это признание наступит?
> Особенно в обстоятельствах, когда условный ChatGPT пишет код, за человека и этот код, генерируется на основании накопленной базы, которая сосем не отвечает представлениям компиляции. 
> 
> Оно вообще ничему не отвечает

---

**[@PetunenkoDV](https://www.youtube.com/channel/UCMAxMmy1Nj-VSsA3bPFsTJg)** *[06.10.2025 08:53](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgyouRFfHL3pnd49FiR4AaABAg) · 👍 3*

Обложка для видоса, - мое почтение! ))

---

**[@AlexanderGranin](https://www.youtube.com/channel/UC8QBEF4ZCjrGaKvGyfxJRGA)** *[06.10.2025 18:51](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugy9mbkfWhN3r0z0X6F4AaABAg) · 👍 3*

У Виталия стоическое терпение. Другим ведущим (особенно тому, который сверху) учиться бы вести цивилизованный диалог. Да и каши в голове у них слишком много.

P.S. Я тот самый Саша Гранин, который написал Functional Design and Architecture. Виталию благодарен за все и считаю честью быть ему другом.

> **[@stepperjumpy](https://www.youtube.com/channel/UCu-Akazh3lW1DwVYxym175Q)** *[07.10.2025 18:10](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugy9mbkfWhN3r0z0X6F4AaABAg.ANx7p-aJXaVANzcvYmgZK1) (ред. 29.11.2025 15:33) · 👍 1*

> @sonboy520 Виталий уже это все прошел, годы, опыт, студенты) Терпение на уровне!

> **[@PetunenkoDV](https://www.youtube.com/channel/UCMAxMmy1Nj-VSsA3bPFsTJg)** *[08.10.2025 12:02](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugy9mbkfWhN3r0z0X6F4AaABAg.ANx7p-aJXaVAO0YaWEDBn0)*

> Вы просто не привыкли к Мурычу )
> Он ведь не интервьювер и не ведущий от слова совсем, местами да душный, но человек в целом хороший
> Но то, что сумел двух таких интересных людей (в целом даже трех) пригласить на один созвон, это мое почтение
> Обычный такой разговор трех совершенно разных девелоперов )

> **[@Son0fBeelzebub](https://www.youtube.com/channel/UChVbSVULfjhPqc1ZhiIXglg)** *[29.10.2025 06:47](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugy9mbkfWhN3r0z0X6F4AaABAg.ANx7p-aJXaVAOr3CerFpJb)*

> Думаете, что Віталій сідел і терпел? Мне кажется, что после первого стріма в таком случае Віталій бы попросту не согласілся. а кніжка у вас прекрасная, спасібо

---

**[@Adventiful](https://www.youtube.com/channel/UCWcFHtGqO3mMnyr-ESZyesg)** *[07.10.2025 14:36](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwPNdAXWNc0EUGPnVl4AaABAg)*

Очень жаль, что Мурычу не дали и он сам не взялся продолжить выразить мысль про Haskell vs C сравнение. У Старострупа было похожее высказывание у Фридмана (он про C++ говорил, правда). Мне кажется, что эту мысль вполне можно было бы развить, накидать примеров. Ведь, по сути, это хороший аргумент к изучению того же ФП - если с этой перспективы/на уровне таких примитивов проще решать целый пласт актуальных сегодня задач, то это перестаёт быть игрушкой в вакууме для саморазвития. И это большой плюс

---

**[@shalidor1619](https://www.youtube.com/channel/UCFt8PeCFYjsm4Er84SyWsbg)** *[07.10.2025 17:41](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgydwwTjAyDZPKx60q14AaABAg)*

Насчет парадигм можно утверждать, что ООП -- эталонная и лучшая парадигма хотя бы просто потому что, она решает и наиболее абстрактную и одновременно наиболее требовательную к производительности проблему: разработка 3д игр. Это невероятно абстрактная область, требующая невероятной производительности. Ни одна другая из парадигм лучше с этим не справляется, нежели ООП. Вот и все. Критерий есть, победитель найден.

> **[@stepperjumpy](https://www.youtube.com/channel/UCu-Akazh3lW1DwVYxym175Q)** *[07.10.2025 18:12](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgydwwTjAyDZPKx60q14AaABAg.ANz_bNYp5lNANzd6zatexh)*

> Casey Muratori посмотрите) про ваше ООП(он как раз и движки игр разрабатывает)

> **[@shalidor1619](https://www.youtube.com/channel/UCFt8PeCFYjsm4Er84SyWsbg)** *[08.10.2025 05:16](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgydwwTjAyDZPKx60q14AaABAg.ANz_bNYp5lNAO-p5OWFAlv)*

> @stepperjumpyединственное, что я по фактам о нем нашел, что он был разработчиком игры the witness, которая использовала самописный движок на плюсах. То есть это буквально единственное его коммерческое достижение как разработчика игр. Другими словами, это человек, не осиливший ООП, не имеющий реальных больших достижений как программист игр, и единственное его достижение и то было написано в ООП на плюсах. Пара пара пам, занавес.

> **[@Son0fBeelzebub](https://www.youtube.com/channel/UChVbSVULfjhPqc1ZhiIXglg)** *[29.10.2025 06:44](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgydwwTjAyDZPKx60q14AaABAg.ANz_bNYp5lNAOr2ow2BmUk)*

> ну і глупость, конечно. взаімодействіе і чіслодробілка с об'ектамі в любой парадігме будет +- одінаковая, особенно после тонны оптімізацій. а на графіку ооп не вліяет нікак, что в іграх, как бы, самое сложное в рамках вычісленій в большінстве случаев.

---

**[@EveryTickGameArt](https://www.youtube.com/channel/UClrShvr-8iMDSchSj4FsrMA)** *[08.10.2025 04:53](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgysalyebytD165U1894AaABAg) (ред. 08.10.2025 17:05)*

Людям не нужно 100500 способов написания одного и того же. Оставьте вы 3-5 способов, хорошо читаемых и производительных. Остальное вырезать! 
Вы же не носите 7 грязных трусов неделька. Вы оденете одни чистые, удобные трусы. 
И спрашивается нафига в js 15 способов не читаемых, не производительных способов. Оставьте вы 3-5 способов, если вы за разнообразие подходов. Нафига, условных 15 нечитаемых, медленных способов. 
Если человек понимает, что он делает. Рефакторинг сводится или к 0 или минимуму, так как нет 15ти видов говнокода. При условии, что компилятор разрешает только условные 3-5 способов написания, решений одной и той же задачи. Получаем: читаемость кода, высокую производительность и отсутствие траты времени, на обдумывание 15-ти способов реализации одной задачи.

---

**[@Adventiful](https://www.youtube.com/channel/UCWcFHtGqO3mMnyr-ESZyesg)** *[09.10.2025 16:12](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=UgwEKhb1C1wSjKV-BDd4AaABAg) (ред. 09.10.2025 16:19)*

2:32:01 а вот это не так, кстати. Буквально вчера на AI Masters от Дьяконова слышал про энкодеры, которые как раз этим занимаются.

Да и ещё в 2020 от Andrew Ng слышал интуитивное интро в эту тему.

То, что сложности в плоскости интерпретации работы моделей есть несомненно. Но вы, светлые головы "классического IT" не разобравшись не в свой огород полезли и навалили чего-то не того на смежные с этим темы. 

Проблема в том, что это плохо прогнозируемые интерпретации. И чтобы понимать "почему так" нужно как раз таки быть хорошим спецом по ML. А ответ "потому что большая кодовая база" правильный. Но ведь модель для этой кодовой базы может быть "наивной", например. И здесь всплывает соотношение сложности языка программирования и естественного языка. LLM-ки то под естественный делаются. Если ЯП соотносим или превосходит, то модель будет наивной.

При всём уважении. Слушать вас было приятно и интересно.

---

**[@sergeykryuchkov8131](https://www.youtube.com/channel/UC6xWMWNLFXKSYCwRNhZpLaA)** *[16.11.2025 12:56](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugx7Uz9SdBSI67ewSlB4AaABAg)*

Весь код (программы) по своей сути императивны, т.е последовательны, для того чтобы не писать повторяющиеся последовательности в разных местах кода, сделали абстракцию функци(выполняет конкретную задачу и по своей сути является декларативкой (что-то положил и что то вышло)), но в программе бывает много функций и много взаимодействующих функций, и что бы не запоминать все функции, появилась новая абстракция, классы(ооп). Вот и все, хочешь, пиши последовательный код, лень повторять, оберни часть кода в функции, если код и с функциями большой, делай классы, но так как любой код имеет порядок действий он даже с классами будет императивным :).

> **[@stepperjumpy](https://www.youtube.com/channel/UCu-Akazh3lW1DwVYxym175Q)** *[25.12.2025 21:47](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugx7Uz9SdBSI67ewSlB4AaABAg.APa3iSdZcgoARARTyP9DUw) (ред. 25.12.2025 21:47)*

> Очень "декларативные функции" - положил на вход и void на выходе, а мир изменился)

> **[@sergeykryuchkov8131](https://www.youtube.com/channel/UC6xWMWNLFXKSYCwRNhZpLaA)** *[26.12.2025 05:39](https://www.youtube.com/watch?v=ES2NPqlDnek&lc=Ugx7Uz9SdBSI67ewSlB4AaABAg.APa3iSdZcgoARBHVkQqNa0)*

> ​@stepperjumpyЧто такое декларация функции в C?
> Любое объявление функции (прототип) является декларацией — оно сообщает компилятору о существовании функции, её имени, возвращаемом типе и параметрах.

---
