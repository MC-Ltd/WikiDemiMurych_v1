---
title: "⎡tips:11⎦ JavaScript Tips: Один символ и производительность"
date: 2023-12-19
tags: []
videoId: "u_bsXuBOO74"
duration: "1:26:36"
views: 6459
likes: 194
comments: 22
---
# [⎡tips:11⎦ JavaScript Tips: Один символ и производительность](https://www.youtube.com/watch?v=u_bsXuBOO74)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 19.12.2023 22:51  
**Тривалість:** 1:26:36  
**Перегляди:** 6459 · **Лайки:** 194 · **Коментарі:** 22
![thumbnail](https://i.ytimg.com/vi/u_bsXuBOO74/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=u_bsXuBOO74)
## Коментарі (15 · відповідей: 7)

**[@dmitriykret8938](https://www.youtube.com/channel/UCHAAqvO5RQN2Manq8fQmB-Q)** *[19.12.2023 11:41](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgxJKmBAIxioE4sP7SR4AaABAg) · 👍 2*

👍👍 👍

---

**[@ART-kh1yy](https://www.youtube.com/channel/UCd_c5eLHvnNdnH0uu6bXj0w)** *[19.12.2023 11:59](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=Ugwqanu4UG5BMj5xK-54AaABAg)*

С Вашим умом  можно попробовать в шахматы поиграть

> **[@MrDima123123](https://www.youtube.com/channel/UCQxUqpRVLjJHOZWE8uyvq0Q)** *[21.12.2023 13:33](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=Ugwqanu4UG5BMj5xK-54AaABAg.9yVfOl5Gsfy9y_zk1v6pd7) · 👍 1*

> нет, он  только будет срать всем в уши о том, что остальные кроме него не играют в шахматы по спецификации

> **[@leon83935](https://www.youtube.com/channel/UCQWoq45oCaF2rcWStxBAnYA)** *[22.12.2023 13:46](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=Ugwqanu4UG5BMj5xK-54AaABAg.9yVfOl5Gsfy9yc_yIufgm9) (ред. 13.06.2024 23:45)*

> в шахматах знание дебютов кардинально меняет ситуацию на доске, каждый разрядник использует эти паттерны, сделовательно одерживает победу, со спецификацией аналогичная ситуация.@MrDima123123

---

**[@gyglejid](https://www.youtube.com/channel/UCy-LzPS8rpgK9PptmHNEVvg)** *[19.12.2023 12:11](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgyvWi6wS8fMxRJTtrl4AaABAg) (ред. 19.12.2023 12:29)*

Запускал на вкладке Sources в Chrome (120.0.6099.110):
 (
    ()=>{
        "use strict";
	function doSum(theInc) {
	var start = performance.now();
		var theSummator = 0;
		for (var theLimit = 0; theLimit < 1073741824; theLimit++) {
			theSummator += theInc;
		}
         console.log(performance.now() - start)
	      return theSummator;
         }
        console.log(doSum(1), doSum(-1), doSum(0.1));
    }
)()
Итог: 
   Если var theSummator = 0; то время выполнения:               625.3000000007451      626.5           984.2999999970198 (~620, ~620, ~980мс)
   Если var theSummator = -0; то время выполнения:              986.5                     998.3000000007451          981.3000000007451  (все разы по ~980мс)

Код идентичный приведённому в видео выдал ~2.2-2.3c для theSummator = 0       и      ~3с для theSummator = -0.
Помогите, пжл, правильно понять и сделать правильные выводы из полученного результата. 
Из видео услышал, что сборка особо не влияет, но пишу на всякий случай: 11th Gen Intel(R) Core(TM) i5-11400 + 16 Gb

---

**[@NickAnisimov](https://www.youtube.com/channel/UCrLTOKViVXeMGzJQVTDl00w)** *[19.12.2023 12:24](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgxgSpky2zdijELqaiF4AaABAg) · 👍 3*

К вопросу воспроизводимости. У меня в  хроме 120 и в ноде 21.4  результат с 0 и c -0  не отличается (разница <2% то в одну, то в другую сторону)

> **[@Гооол-й4ч](https://www.youtube.com/channel/UCI_uKeDGw-qUumxR37GgSLA)** *[19.12.2023 15:31](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgxgSpky2zdijELqaiF4AaABAg.9yViBNgXMZH9yW2eReOLfH) · 👍 1*

> та же тема в d8. Наличие деоптимизации (not a smi) завсит от 0 или -0, но само время выполнения прыгает на уровне погрешности.

---

**[@VladBurlutsky](https://www.youtube.com/channel/UCqQNsPPMk_UwncP-6sGOL1w)** *[19.12.2023 14:39](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgwQI5dtIBqqaPT3Kxd4AaABAg)*

Отлично, возобновил трансляции

---

**[@EvilYou](https://www.youtube.com/channel/UCmEdFUN2gODWCHvETEX2zEw)** *[19.12.2023 16:26](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgwwsApgPbgkufCjpMd4AaABAg) (ред. 19.12.2023 16:57) · 👍 6*

С нулем понятно, а как насчет других чисел?

P.S. Хотя у меня с var summator = -0 процентов на 15-20 наоборот медленнее работает данный код (проверял в Chrome и яндекс браузере, результат одинаковый, уменьшение limit на 1 ничего не дало):

'use strict';

(
    () => {
        var start = performance.now();

        function sum(inc) {
            var summator = 0;

            for (var limit = 0; limit < 1073741823; limit++) {
                summator += inc;
            }

            return summator;
        }

        console.log(
            sum(1),
            sum(-1),
            sum(0.1)
        )

        console.log(performance.now() - start);
    }
)();

---

**[@Boortwint](https://www.youtube.com/channel/UC1f_N0jDDOe992KFLVbDk9Q)** *[19.12.2023 16:34](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgxZyo0hiWvrcwjeGvJ4AaABAg)*

Полагаю, объекты с различными наборами свойств, тоже влияют на производительность кода? Где-то слышал, что удалять или добавлять свойства в объекте - не самая лучшая практика, потому как рантайм оптимизирует выполнение функции в случае передачи в неё объектов с одинаковым интерфейсом. Как только функция получает объект с отличным набором свойств, всё в моменте скатывается в деоптимизацию.

> **[@Boortwint](https://www.youtube.com/channel/UC1f_N0jDDOe992KFLVbDk9Q)** *[20.12.2023 09:07](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgxZyo0hiWvrcwjeGvJ4AaABAg.9yW9pMNI2iQ9yXwSJfl_83) (ред. 14.06.2024 00:17)*

> @MyName-tg8ek ты волен делать всё, что твоей душе угодно. Всем до фени. 
> Я же подожду, вдруг Мурыч ответит на мой вопрос в комментарии, которого ты не увидел.

> **[@Boortwint](https://www.youtube.com/channel/UC1f_N0jDDOe992KFLVbDk9Q)** *[20.12.2023 11:35](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgxZyo0hiWvrcwjeGvJ4AaABAg.9yW9pMNI2iQ9yYCPujjHRa) (ред. 14.06.2024 00:17)*

> @MyName-tg8ek Object.freeze - и вот из объекта больше нельзя ничего удалить и нельзя ничего в него добавить.
> Вопрос вообще был о другом. Меня интересует, насколько сильно агент уходит в деоптимизацию в случае передачи в функцию объектов с разным набором свойств.

---

**[@cyrilanisimov](https://www.youtube.com/channel/UCYYgfFTHCMLZzpAdL3QP5ow)** *[19.12.2023 17:52](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgyuM4zEETtRU6Vbkw94AaABAg)*

Как -0 и +0? А как же комплиментарный код?

> **[@AsForJS](https://www.youtube.com/channel/UC8aUxVCtAmBtKXmYdPmzjeA)** *[22.12.2023 12:51](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgyuM4zEETtRU6Vbkw94AaABAg.9yWIn-RbLMg9ycUiFXe-Sw) · 👍 1*

> Всегда есть существенная разница, между тем что следует делать в рамках архитектуры языка, и тем что можно делать в рамках того, где он не доглядел.
> 
> Язык JavaScript это анархия. И таким будет всегда. И потому будет жить вечно.
> 
> Как следствие, рекомендации, подобные этим, в первую очередь следует понимать не как те, которые раскрывают суть самого языка, но как те, которые показывают чем он является в тот самый момент, когда об этой рекомендации говорят.
> 
> Я посвятил в видео немало времени, чтобы пояснить почему сейчас и в каких условиях это имеет значение. 
> 
> И именно это важно, для формирования специалиста

---

**[@ИнкОгнито-ф2в](https://www.youtube.com/channel/UCL7xVAsjcoz7FAkwI7URcHw)** *[27.12.2023 06:26](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgyvNQQ19qB1eJuwOG94AaABAg) · 👍 1*

чёт у меня это выглядит как обратная оптимизация. с 3.5 до 4.2 время выполнения растёт. возможно что в новом хроме эта оптимизация теперь по умолчанию сделана

---

**[@djekiseven1336](https://www.youtube.com/channel/UCtcVDa349MnFKaRtN8eV4fA)** *[03.01.2024 08:32](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgzkJFb1G517X9yNYBx4AaABAg) · 👍 1*

Ох и нудятина, то что можно было объяснить за 10 минут растянуто на полтора часа

> **[@slaviksemen4919](https://www.youtube.com/channel/UCup0Z-2H-IunGALbzZt4cvw)** *[10.02.2024 04:02](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgzkJFb1G517X9yNYBx4AaABAg.9z5vcjcMpI0A-cHtpUEqoc) (ред. 10.02.2024 04:02)*

> братан, может еще пожевать и в рот положить?

---

**[@darksessence](https://www.youtube.com/channel/UCtE9WrNZfNou4zh3bAS-yrA)** *[06.01.2024 11:04](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgwaUEoJGIqXwpCsOmd4AaABAg) (ред. 06.01.2024 11:33)*

Похоже что-то изменилось в алгоритмах оптимизации V8, в Хроме у меня нет разницы, а вот в Firefox есть разница >10% (как на видео)
Хром: Версия 122.0.6226.2 (Официальная сборка), dev (64 бит)
Firefox: 121.0 (64-разрядный)
код:
'use strict';
var theStart=performance.now();
function doSum(theInc) {
	var theSummator=-0;
	for(var theLimit=0; theLimit<107374182; theLimit++) {
		theSummator+=theInc;
	}
	return theSummator;
}
console.log(
	doSum(1),
	doSum(-1),
	doSum(0.1),
)
console.log(performance.now()-theStart);

---

**[@slaviksemen4919](https://www.youtube.com/channel/UCup0Z-2H-IunGALbzZt4cvw)** *[10.02.2024 04:01](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgyHNvRgnzZ9khg3Dvp4AaABAg)*

спасибо вам за ваши труды.

---

**[@whenparty](https://www.youtube.com/channel/UCqHbpRDA1WNCBhU4iO2I_hA)** *[18.02.2024 11:02](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgwR-_d1yvTqmPzBaE94AaABAg) (ред. 18.02.2024 11:03)*

Интересное утверждение о повторяемости результатов эксперимента на разных машинах. 

Как вы смотрите на идею о том, что для определённых процессоров время, затраченное на операции деоптимизации, существенно меньше разницы во времени выполнения операций над целыми числами и числами с плавающей точкой? 

В данном случае возможно, что выполнение трех циклов с арифметическими операциями над числами с плавающей точкой займет больше времени, чем выполнение двух циклов с арифметическими операциями над целыми числами, за которыми следует операция деоптимизации, а затем еще один цикл с арифметическими операциями над числами с плавающей точкой.

---

**[@FrankBakulov](https://www.youtube.com/channel/UC73lSQURf81UCdJHJ884tJA)** *[15.03.2024 16:54](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgyLrMtba00OEjJ51D54AaABAg)*

Почему -0 не понизил производительность суммирования целых чисел?

---

**[@AndreyChursin](https://www.youtube.com/channel/UC5JrSe1DyoNVeehFrixIeYw)** *[22.03.2024 13:30](https://www.youtube.com/watch?v=u_bsXuBOO74&lc=UgwpT4znQtfySOPo9xJ4AaABAg)*

Чувствую боль в голове😊 хорошо как☺️👍

---
