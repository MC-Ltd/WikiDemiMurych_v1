---
title: "Оптимизируем главную страницу HexLet до PageSpeed 90+"
date: 2026-04-26
tags: ["seo", "5", "web", "pagespeed", "lighthouse", "hexlet"]
videoId: "zXITWw0ctDM"
duration: "2:37:40"
views: 3274
likes: 128
comments: 12
---
# [Оптимизируем главную страницу HexLet до PageSpeed 90+](https://www.youtube.com/watch?v=zXITWw0ctDM)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 26.04.2026 12:16  
**Тривалість:** 2:37:40  
**Перегляди:** 3274 · **Лайки:** 128 · **Коментарі:** 12
![thumbnail](https://i.ytimg.com/vi/zXITWw0ctDM/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=zXITWw0ctDM)
## Таймкоди

- [00:00:00](https://www.youtube.com/watch?v=zXITWw0ctDM&t=0)   Приветствие и объявление темы стрима
- [00:01:30](https://www.youtube.com/watch?v=zXITWw0ctDM&t=90)   Цель: поднять главную HexLet с 57 до 90+
- [00:04:41](https://www.youtube.com/watch?v=zXITWw0ctDM&t=281)   Объяснение PageSpeed и его влияния на SEO
- [00:13:21](https://www.youtube.com/watch?v=zXITWw0ctDM&t=801)   Создаём локальную копию страницы через wget
- [00:18:16](https://www.youtube.com/watch?v=zXITWw0ctDM&t=1096)   Ошибки локальной копии из-за кросс-доменов
- [00:22:28](https://www.youtube.com/watch?v=zXITWw0ctDM&t=1348)   Удаляем preload/preconnect — баллы растут
- [00:32:35](https://www.youtube.com/watch?v=zXITWw0ctDM&t=1955)   Разбор метрики LCP (первая область отображения)
- [00:35:22](https://www.youtube.com/watch?v=zXITWw0ctDM&t=2122)   Анализ тяжёлых файлов: CSS 360КБ, JS 762КБ
- [00:40:20](https://www.youtube.com/watch?v=zXITWw0ctDM&t=2420)   Эксперимент: удаление CSS/JS даёт 99 баллов
- [00:45:51](https://www.youtube.com/watch?v=zXITWw0ctDM&t=2751)   Влияние скриптов Яндекс.Метрики на скорость
- [00:53:15](https://www.youtube.com/watch?v=zXITWw0ctDM&t=3195)   Импортируем CSS напрямую в HTML
- [00:56:24](https://www.youtube.com/watch?v=zXITWw0ctDM&t=3384)   Результат: почти 90 баллов
- [01:00:18](https://www.youtube.com/watch?v=zXITWw0ctDM&t=3618)   Переносим JavaScript в конец body
- [01:06:47](https://www.youtube.com/watch?v=zXITWw0ctDM&t=4007)   Инлайним JS в HTML — прирост +3 балла
- [01:11:56](https://www.youtube.com/watch?v=zXITWw0ctDM&t=4316)   Выясняем: JS блокирует отрисовку LCP
- [01:18:17](https://www.youtube.com/watch?v=zXITWw0ctDM&t=4697)   Откладываем загрузку JS на 10 секунд
- [01:22:17](https://www.youtube.com/watch?v=zXITWw0ctDM&t=4937)   Успех: страница получает 96 баллов
- [01:28:06](https://www.youtube.com/watch?v=zXITWw0ctDM&t=5286)   Отложенная загрузка JS ускорила метрики в 2 раза
- [01:33:17](https://www.youtube.com/watch?v=zXITWw0ctDM&t=5597)   Внедряем ленивую загрузку изображений
- [01:37:48](https://www.youtube.com/watch?v=zXITWw0ctDM&t=5868)   Временно заменяем картинки на прозрачную заглушку
- [01:45:55](https://www.youtube.com/watch?v=zXITWw0ctDM&t=6355)   Дробим монолитный JS на модули под требования
- [01:46:51](https://www.youtube.com/watch?v=zXITWw0ctDM&t=6411)   Удаляем из кода Метрики и всё лишнее
- [01:59:06](https://www.youtube.com/watch?v=zXITWw0ctDM&t=7146)   Запускаем счётчики не сразу, а через 1.5 секунды
- [02:08:03](https://www.youtube.com/watch?v=zXITWw0ctDM&t=7683)   Оптимизация шрифтов: атрибут swap и подрезка
- [02:09:34](https://www.youtube.com/watch?v=zXITWw0ctDM&t=7774)   Отказываемся от иконочных шрифтов в пользу SVG
- [02:14:27](https://www.youtube.com/watch?v=zXITWw0ctDM&t=8067)   Инлайним SVG-иконки, а не подключаем спрайты
- [02:16:53](https://www.youtube.com/watch?v=zXITWw0ctDM&t=8213)   Напоминание о правилах вложения тегов в HTML5
- [02:23:24](https://www.youtube.com/watch?v=zXITWw0ctDM&t=8604)   Обсуждение особенностей и багов Safari
- [02:31:57](https://www.youtube.com/watch?v=zXITWw0ctDM&t=9117)   Performance API как инструмент для точной оптимизации
- [02:35:05](https://www.youtube.com/watch?v=zXITWw0ctDM&t=9305)   Проблема современных LLM: они учатся на плохом коде
- [02:36:09](https://www.youtube.com/watch?v=zXITWw0ctDM&t=9369)   Предложение зрителям: присылайте "тяжёлые" сайты на разбор
- [02:37:05](https://www.youtube.com/watch?v=zXITWw0ctDM&t=9425)   Завершение стрима, благодарность зрителям
## Коментарі (10 · відповідей: 2)

**[@drevitsky](https://www.youtube.com/channel/UCcNnGd3r4XTIwsogluajzjQ)** *[26.04.2026 12:20](https://www.youtube.com/watch?v=zXITWw0ctDM&lc=UgxsvnD4jItQ9asJ-uh4AaABAg)*

Будь здоров

---

**[@alexgolim2198](https://www.youtube.com/channel/UCNzgXjCG1CyHquoEnErDiPQ)** *[26.04.2026 13:30](https://www.youtube.com/watch?v=zXITWw0ctDM&lc=UgwXLNQ2uLpZ6AQppTB4AaABAg)*

спасибо. Интерестно

---

**[@Andrew-NaN](https://www.youtube.com/channel/UCvEyMg75ev6ICAbl2yxUBpg)** *[26.04.2026 17:48](https://www.youtube.com/watch?v=zXITWw0ctDM&lc=UgwvOMezC3jPWT9omTJ4AaABAg) · 👍 3*

Мурыч контент огонь!

---

**[@alexperemey6046](https://www.youtube.com/channel/UCchNS6618CdinWR5iznDcAQ)** *[27.04.2026 05:13](https://www.youtube.com/watch?v=zXITWw0ctDM&lc=UgyeKYRI4Y8UM-2lCul4AaABAg) · 👍 1*

Самое противное здесь то, что это все - родовые проблемы фреймворка, а не тупость отдельного программиста. Т.е. этот неоптимальный код рожает реакт по умолчанию.

---

**[@Andrew-NaN](https://www.youtube.com/channel/UCvEyMg75ev6ICAbl2yxUBpg)** *[27.04.2026 18:23](https://www.youtube.com/watch?v=zXITWw0ctDM&lc=UgxVRfnAugwVm64ybhJ4AaABAg)*

14:38 wget

--page-requisites downloads everything needed to display a page correctly - images, CSS, JavaScript, fonts. Without this, you'd get the HTML but it would render broken.
--convert-links rewrites links in the downloaded HTML so they point to your local copies instead of the original URLs. Makes the offline version actually navigable.
--adjust-extension adds the correct file extension if it's missing - so a URL serving HTML without a .html extension gets renamed properly on disk.
--span-hosts allows wget to follow links to other domains. Normally wget stays on the domain you started with, so this is needed when assets (fonts, CDN-hosted scripts, etc.) live on a different host.
--no-parent restricts the crawl to the directory you specify and below - it won't crawl upward to parent paths. Keeps the download scoped to what you actually want

---

**[@alisherzaitov](https://www.youtube.com/channel/UCKvSKAgRgEC6ImyVS3h7YPQ)** *[27.04.2026 18:58](https://www.youtube.com/watch?v=zXITWw0ctDM&lc=Ugzni88wjCnxMkNnDgJ4AaABAg)*

Уважаемый Деми Мурыч, хочу кэшировать страницы и картинки как вы. Расскажите какой cache-control хэдер использовать чтобы в ус не дуть и для SEO было хорошо.

Вот вижу на mila-butz вы используете max-age=31536000, public, no-cache​  для html и max-age=31536000, public, immutable​ для картинок. Вижу также, что картинки у вас без хэшей. И я так хочу. Только не очень понимаю как быть если картинки я планирую иногда редактировать, с вашими же настройками они на год сохраняются в браузере.

Также не понимаю в чем хитрость использовать max-age=31536000, public, no-cache​ вместо `max-age=0, must-revalidate` если результат одинаковый? Просто дело вкуса или ваш вариант лучше.

Сам я в кэшировании нуб,
Сайт делаю статический на astro,
Размещаю все это дело на "cloudflare worker",
Проксирую тоже через cloudflare,
Картинки у меня без хэшей: ../article-1/image-1.webp.

Пока пришел к такому для html и контентных картинок:
Cache-Control: public, max-age=14400, must-revalidate

И к такому для js/css и декоративных картинок:
Cache-Control: public, max-age=31536000, immutable

---

**[@rodigy](https://www.youtube.com/channel/UCDbVwcOGci1hdYziHyPYXzQ)** *[27.04.2026 19:40](https://www.youtube.com/watch?v=zXITWw0ctDM&lc=UgwRUqQxInIJH1bXP1B4AaABAg)*

C SPA (например современные vue/angular) такое можно провернуть без server side render?

> **[@alexErtemenko](https://www.youtube.com/channel/UCUAZW4LEsRRWhKwK8xxMZcw)** *[28.04.2026 16:13](https://www.youtube.com/watch?v=zXITWw0ctDM&lc=UgwRUqQxInIJH1bXP1B4AaABAg.AW6vmR0zJb1AW97rO0YMYQ)*

> Неа, vue/angular  попаболь для сошника. так как это придумывалось веб приложений а не для сайтов

---

**[@cpa3259](https://www.youtube.com/channel/UCgSw5LuFf3hZ_xOnKqxBBkQ)** *[29.04.2026 10:42](https://www.youtube.com/watch?v=zXITWw0ctDM&lc=UgwTBdY5nxRyZbsZfuJ4AaABAg)*

мои все сайты 100, 100, 100, 100 :D и не заметил разницы. сайты у которых было 75-80 по шкале PageSpeed они были в топ3, я в на 7-8 позиции

> **[@Ivan-o9w8w](https://www.youtube.com/channel/UC80H52S-R1kGJaxHxORx1YA)** *[11.05.2026 20:38](https://www.youtube.com/watch?v=zXITWw0ctDM&lc=UgwTBdY5nxRyZbsZfuJ4AaABAg.AWB6lg9bY0PAWg4Zp2D7km)*

> Ну так это не единственная метрика для сео

---

**[@Andrew-NaN](https://www.youtube.com/channel/UCvEyMg75ev6ICAbl2yxUBpg)** *[05.05.2026 04:36](https://www.youtube.com/watch?v=zXITWw0ctDM&lc=UgzcBMhc9_BsWilsFRN4AaABAg) (ред. 08.05.2026 17:55) · 👍 1*

1:09:54 правило мурыча на размер index.html - не более 110kb в сжатом виде
1:11:05 defer, async don’t use
1:35:10 как не надо интегрировать img
1:39:10 пример как надо интегрировать img
1:40:35  srcset & sizes or picture tags
2:09:34 FontAwesome только для прототипов, в продакшен инлайн эсвэгэ
2:10:54 как правильно использовать фонтосом - with css :before & :after
2:11:33 за <span>icon</span> надо увольнять
2:14:57 про сжатие иконок
2:16:56 вопрос: почему нельзя вкладывать див в спан в хтмл5. 2:18:26 Ответ
2:19:26 вопрос про тег а. 2:20:53 ответ
2:25:32 как надо добавлять скрипт вместо события лоад
2:31:58 намек: события перформанс api

---

**[@Ivan-o9w8w](https://www.youtube.com/channel/UC80H52S-R1kGJaxHxORx1YA)** *[11.05.2026 20:38](https://www.youtube.com/watch?v=zXITWw0ctDM&lc=UgyNS25HuC4eoKCcolh4AaABAg)*

Так вы ещё и ВПН наверное не отключили

---
