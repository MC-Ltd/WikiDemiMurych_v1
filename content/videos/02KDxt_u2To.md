---
title: "⎡dlgs:01⎦   JavaScript Беседы: Service Worker-ы"
date: 2023-11-19
tags: []
videoId: "02KDxt_u2To"
duration: "3:08:11"
views: 3971
likes: 169
comments: 7
---
# [⎡dlgs:01⎦   JavaScript Беседы: Service Worker-ы](https://www.youtube.com/watch?v=02KDxt_u2To)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 19.11.2023 10:49  
**Тривалість:** 3:08:11  
**Перегляди:** 3971 · **Лайки:** 169 · **Коментарі:** 7
![thumbnail](https://i.ytimg.com/vi/02KDxt_u2To/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=02KDxt_u2To)
## Таймкоди

- [00:00:00](https://www.youtube.com/watch?v=02KDxt_u2To&t=0)   Музыка
- [00:04:30](https://www.youtube.com/watch?v=02KDxt_u2To&t=270)   Настройка
- [00:12:10](https://www.youtube.com/watch?v=02KDxt_u2To&t=730)   Вопрос из чата: Почему заполнение объекта в цикле быстрее, чем заполнение new Map
- [00:30:00](https://www.youtube.com/watch?v=02KDxt_u2To&t=1800)   Что такое Web Workers и для чего они нужны
- [00:37:00](https://www.youtube.com/watch?v=02KDxt_u2To&t=2220)   О много поточном JS и агентах
- [00:47:10](https://www.youtube.com/watch?v=02KDxt_u2To&t=2830)   О Web Workers и их виды
- [00:57:20](https://www.youtube.com/watch?v=02KDxt_u2To&t=3440)   О Service Worker
- [01:07:00](https://www.youtube.com/watch?v=02KDxt_u2To&t=4020)   Ищем какие запросы перехватывает Service Worker
- [01:18:45](https://www.youtube.com/watch?v=02KDxt_u2To&t=4725)   Service Worker на примере
- [01:27:50](https://www.youtube.com/watch?v=02KDxt_u2To&t=5270)   Как запускать несколько Service Workers на одной странице
- [01:35:15](https://www.youtube.com/watch?v=02KDxt_u2To&t=5715)   Об организации приложения на основе Web Workers
- [01:39:30](https://www.youtube.com/watch?v=02KDxt_u2To&t=5970)   Ремарка о работе Service Worker
- [01:47:45](https://www.youtube.com/watch?v=02KDxt_u2To&t=6465)   О каких важных API Service Worker - а необходимо знать веб программисту
- [01:55:00](https://www.youtube.com/watch?v=02KDxt_u2To&t=6900)   О генерации и кэшировании байт кода Service Worker - ом
- [02:16:05](https://www.youtube.com/watch?v=02KDxt_u2To&t=8165)   Какими инструментами пользоваться при работе с Service Worker - ами
- [02:21:30](https://www.youtube.com/watch?v=02KDxt_u2To&t=8490)   Как кэшируется JS файлы без/с использованием Service Worker - ов
- [02:45:00](https://www.youtube.com/watch?v=02KDxt_u2To&t=9900)   На примере как Service Worker кэширует JS файлы скомпилированные в байт код
- [02:55:30](https://www.youtube.com/watch?v=02KDxt_u2To&t=10530)   Краткое игого
## Коментарі (7 · відповідей: 0)

**[@nikto1851](https://www.youtube.com/channel/UC3m-4PpnRuVjLw3iM1rTkag)** *[25.11.2023 13:02](https://www.youtube.com/watch?v=02KDxt_u2To&lc=Ugz8FEhdQavOqiO4U594AaABAg) · 👍 1*

спасибо!

---

**[@gyglejid](https://www.youtube.com/channel/UCy-LzPS8rpgK9PptmHNEVvg)** *[11.12.2023 20:05](https://www.youtube.com/watch?v=02KDxt_u2To&lc=UgwcfaJ2b66FrnnCRIF4AaABAg)*

Снимаю шляпу...
Благодарочка...

---

**[@dobernike_](https://www.youtube.com/channel/UC4Wc7Z15IRGU8M56A7p_lEw)** *[10.05.2024 12:10](https://www.youtube.com/watch?v=02KDxt_u2To&lc=UgyrvRhx9U1oTbL4RIR4AaABAg)*

Очень годно, большое спасибо!
Подписываюсь!

---

**[@Ant3rn](https://www.youtube.com/channel/UCrJ1pBwILPLxSr8rEsMugzg)** *[11.08.2024 00:36](https://www.youtube.com/watch?v=02KDxt_u2To&lc=Ugxmj-y7egfNvk9ffAJ4AaABAg) (ред. 11.08.2024 00:57)*

Касательно ordered/unordered для object vs Map. (ecma 24.1.1.1)  Set map.[[MapData]] to a new empty List. Когда берём итератор у Map-a - он опирается на [[MapData]] - на List. Для List же в (6.2.2) описано "When an algorithm iterates over the elements of a List without specifying an order, the order used is the order of the elements in the List.". Есть смотреть глубже - [[ownPropertyKeys]] у Object-a - тоже List, но в Map добавление новой энтри явно говорит сделать "append to M.[[MapData]]". Для объектов, если я ничего не упускаю - описано лишь то, что [[Set]] новой проперти приведёт к созданию рекорда, и ничего явного про то, куда новый key засунуть.

---

**[@blackbirdchannel-c7b](https://www.youtube.com/channel/UC_5EjvuuSinSqYR2C4dKEkA)** *[10.12.2024 18:49](https://www.youtube.com/watch?v=02KDxt_u2To&lc=UgxasQh6VAuRvSMvA614AaABAg)*

Очень интересные предпочтения к выбору *подарков, причем они почти полностью совпадают с моими требованиями, 99%

---

**[@blackbirdchannel-c7b](https://www.youtube.com/channel/UC_5EjvuuSinSqYR2C4dKEkA)** *[10.12.2024 18:58](https://www.youtube.com/watch?v=02KDxt_u2To&lc=UgzrwKdZV3ILU68pdCp4AaABAg)*

Мыщъх - помним!

---

**[@qaload](https://www.youtube.com/channel/UC1LdgjPJSr6u_E7CAv8y-wQ)** *[26.06.2025 09:02](https://www.youtube.com/watch?v=02KDxt_u2To&lc=Ugze4ZJgb6QkrDr7lyR4AaABAg)*

Приятно было слушать! Послушаю еще раз

---
