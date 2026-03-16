---
title: "Расследование бага в OSR (On-Stack Replacement) оптимизации V8"
date: 2025-10-17
tags: ["perf", "17", "v8", "osr", "javascript", "bug"]
videoId: "dgZG-OHOyUs"
duration: "2:32:57"
views: 1081
likes: 63
comments: 2
---
# [Расследование бага в OSR (On-Stack Replacement) оптимизации V8](https://www.youtube.com/watch?v=dgZG-OHOyUs)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 17.10.2025 21:10  
**Тривалість:** 2:32:57  
**Перегляди:** 1081 · **Лайки:** 63 · **Коментарі:** 2
![thumbnail](https://i.ytimg.com/vi/dgZG-OHOyUs/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=dgZG-OHOyUs)
## Таймкоди

- [00:00:00](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=0)   Начало трансляции, проверка звука и изображения
- [00:02:20](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=140)   Введение в тему: оптимизация в V8, баг в OSR (On-Stack Replacement)
- [00:03:58](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=238)   Процесс исследования и обнаружения скрытого бага
- [00:06:48](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=408)   Анекдот о мячике для пинг-понга
- [00:08:59](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=539)   Вопрос об оценке нагрузки команды байт-кода, опции для измерения производительности
- [00:13:29](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=809)   Фазы оптимизации в V8: байт-код, Spark Pluck, Maglev, TurboFan
- [00:15:43](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=943)   Объяснение OSR оптимизации: оптимизация тела цикла
- [00:23:23](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=1403)   Оценка производительности с помощью утилиты `time` и среды `d8` (g-sv)
- [00:27:47](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=1667)   Тестирование функции FPS, влияние внешнего идентификатора на производительность
- [00:35:06](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=2106)   Влияние окружения на производительность, внутренняя проблема V8
- [00:38:10](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=2290)   Система тестирования производительности V8: переход от микробенчмарков к "in-wild" тестам
- [00:40:43](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=2443)   Типы кода в JavaScript: функции, глобальное окружение, eval, модули
- [00:43:24](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=2604)   Начало расследования с использованием логов V8
- [00:47:09](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=2829)   Проверка кода в Node.js, патчи и отключение оптимизаций
- [00:51:34](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=3094)   Анализ логов V8: трассировка оптимизации, фаза Maglev
- [00:54:49](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=3289)   Оптимизация функций domain и inner, деоптимизация и кэширование
- [00:58:12](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=3492)   Сравнение логов оптимизации для медленной и быстрой функций
- [01:02:11](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=3731)   Анализ проблемы с OSR: отключение OSSR нормализует результаты
- [01:09:22](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=4162)   Подтверждение бага в алгоритме OSR с помощью опции --trace-ossr
- [01:10:35](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=4235)   Оптимизация функций в циклах, разница между оптимизацией всей функции и OSR
- [01:13:55](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=4435)   Форсирование оптимизации функции domain для устранения проблем OSR
- [01:19:56](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=4796)   Вывод: проблема связана со срабатыванием OSR оптимизации и различиями в генерируемом коде
- [01:22:19](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=4939)   Опции для анализа кода: вывод оптимизированного кода, комментарии, трассировка
- [01:27:08](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=5228)   Проблемы с многопоточностью при анализе, опция single
- [01:30:05](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=5405)   Получение машинного кода, анализ без углубления в ассемблер
- [01:32:41](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=5561)   Сравнение логов и кода для "медленной" и "быстрой" версий
- [01:38:09](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=5889)   Анализ оптимизаций: обнаружение инлайнинга функции в "быстрой" версии
- [01:45:56](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=6356)   Важность инлайнинга функций для оптимизации, работа компиляторов
- [01:50:07](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=6607)   Анализ логов: использование глобального онлайн-кэша в "быстрой" версии
- [01:57:17](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=7037)   Проблема оптимизации: ключевая оптимизация не срабатывает при определенных условиях
- [02:03:41](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=7421)   Решение проблемы: инкапсуляция функции внутри цикла, сокращение времени выполнения
- [02:04:41](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=7481)   Анализ проблемы: отсутствие фидбек-вектора для функций вне глобального окружения
- [02:08:46](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=7726)   Обсуждение проблем с оптимизацией до Maglev и TurboFan
- [02:10:29](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=7829)   Отключение Maglev не решает проблему, возраст бага более 5 лет
- [02:12:48](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=7968)   Роль TurboFan в инлайнинге функций, проблемы с фидбек-вектором
- [02:16:02](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=8162)   Рекомендации по оптимизации: инлайнить код в локальной функции для циклов
- [02:17:24](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=8244)   Ограничения микробенчмарков, необходимость серьезной базы данных для анализа
- [02:19:10](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=8350)   Проблемы с кэшем процессора, влияние размера кэша на оптимизацию
- [02:21:31](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=8491)   Нюансы профилирования канвас-анимаций, использование типизированных массивов
- [02:27:03](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=8823)   Будущее семантической верстки в контексте AI (ChatGPT) и поисковых систем
- [02:31:25](https://www.youtube.com/watch?v=dgZG-OHOyUs&t=9085)   Завершение трансляции, благодарности и контакты
## Коментарі (2 · відповідей: 0)

**[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[17.10.2025 22:15](https://www.youtube.com/watch?v=dgZG-OHOyUs&lc=Ugw6XMNB8d9lLMs8dOB4AaABAg)*

В продолжение трансялции, я еще скажу об этом отдельно, я с смого начала неверно понял фразу Максима @Jaood_xD про два дополнительных ключа: --trace-maglev-inlining --trace-turbo-inlining
использование которых, сразу бы обратили внимание на важное отличие одного кода от другого, без необходимости пугать себя логами с машинным кодом

То есть путь исследования был бы на много короче и намного более простым

---

**[@PimiTree](https://www.youtube.com/channel/UC7MJhschnxT0Pskc320fLzA)** *[20.10.2025 11:03](https://www.youtube.com/watch?v=dgZG-OHOyUs&lc=UgyaPS7O1OSU8padnBV4AaABAg)*

топовый анекдот про мячики для пинг-понга

---
