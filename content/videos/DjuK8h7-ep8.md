---
title: "Производительность Math.trunc vs Or"
date: 2026-05-17
tags: ["perf", "21", "v8", "js", "", "trunc", "or", "javascript"]
videoId: "DjuK8h7-ep8"
duration: "2:36:56"
views: 933
likes: 39
comments: 3
---
# [Производительность Math.trunc vs Or](https://www.youtube.com/watch?v=DjuK8h7-ep8)

**Канал:** [As For JS](https://www.youtube.com/@asforjs)  
**Дата:** 17.05.2026 03:43  
**Тривалість:** 2:36:56  
**Перегляди:** 933 · **Лайки:** 39 · **Коментарі:** 3
![thumbnail](https://i.ytimg.com/vi/DjuK8h7-ep8/hqdefault.jpg)

▶ [Дивитись на YouTube](https://www.youtube.com/watch?v=DjuK8h7-ep8)
## Коментарі (3 · відповідей: 0)

**[@Andrew-NaN](https://www.youtube.com/channel/UCvEyMg75ev6ICAbl2yxUBpg)** *[17.05.2026 05:32](https://www.youtube.com/watch?v=DjuK8h7-ep8&lc=Ugy0sX56ETaxCrbVw994AaABAg) · 👍 1*

16:06 как делать тест

---

**[@mcltdtm420](https://www.youtube.com/channel/UCu4YeW9ZlE51GwOEbpAox3w)** *[17.05.2026 15:45](https://www.youtube.com/watch?v=DjuK8h7-ep8&lc=UgzixlGn1nKY-hi6Qw14AaABAg)*

// Старт в конце файла.

var _size = 16 * 1024; // Размер массива
var _cpow = Math.floor(10_000_000_000 / _size); // Количество повторений тестов
var _data = new Float64Array(_size);

var random = (min, max) => {
  return (Math.random() * (max - min)) + min + Math.random()
};

// Заполнить массив случайными float
// Максимальное число 2 млрд (2^31),
// чтобы при |0 не получить отрицательное число
var i = 0;
var min = 1;
var max = 2_000_000_000;
for (i = 0; i < _size; i++) {
  _data[i] = (random(min, max))
};


// Math.floor
var do_floor = () => {
  var i = 0;
  var data = _data;
  var size = _size;
  var value = 0;

  for (i = 0; i < size; i++) {
    value += Math.floor(data[i]);
  }

  return value;
};

// Math.trunc
var do_trunc = () => {
  var i = 0;
  var data = _data;
  var size = _size;
  var value = 0;

  for (i = 0; i < size; i++) {
    value += Math.trunc(data[i]);
  }

  return value;
};


// Bitwise OR
var do_bitor = () => {
  var i = 0;
  var data = _data;
  var size = _size;
  var value = 0;

  for (i = 0; i < size; i++) {
    value += data[i] | 0;
  }

  return value;
};


// Bitwise double-NOT
var do_dbnot = () => {
  var i = 0;
  var data = _data;
  var size = _size;
  var value = 0;

  for (i = 0; i < size; i++) {
    value += ~~data[i];
  }

  return value;
};


/**
 * Функция обертка
 * @param {() => {}} func — функция для теста
 * @param {string} name   — название функции для вывода в консоль
 */
var do_calc = (func, name) => {
  var i = 0;
  var retry = _cpow;
  var itime = Date.now();
  var value = 0;

  // Выполнить тестовую функцию N раз
  for (i = 0; i < retry; i++) {
    value += func();
  }

  // Итого функция перебрала ≈ 10 млрд элементов
  // Засечь потраченное время
  itime = Date.now() - itime;

  console.log(`\n=== ${name} ===`);
  console.log(`Time: ${(itime/1000).toFixed(3)} seconds`);
  console.log(`Value: ${value}`);
};


// Прогрев массива (на всякий случай 😜)
// Вызывает сам себя ещё 3 раза
// Через setTimeout(() => do_init(counter+1), 1000);
// После вызывает do_start
var do_init = (counter) => {
  var size = _size;
  var data = _data;

  var sum = 0;
  var num = 0;
  var log = console.log;

  for (i = 0; i < size; i++) {
    num = data[i];
    sum += num % 2 === 0
      ? (num / 100)
      : (num / 100) * -1;
  }

  if (counter > 3) {
    do_start();
  } else {
    log(`warm up ${counter}`);
    setTimeout(() => do_init(counter+1), 1000);
  }
};

// Вызов тестов по очереди
var do_start = () => {
  var log = console.log;
  var calc = do_calc;
  var floor = do_floor;
  var trunc = do_trunc;
  var bitor = do_bitor;
  var dbnot = do_dbnot;

  log(`START:`);

  calc(floor, "Math.floor");
  calc(trunc, "Math.trunc");
  calc(bitor, "Bitwise OR");
  calc(dbnot, "Bitwise Double-NOT");
}


// Старт
do_init(1);

---

**[@demimurych1](https://www.youtube.com/channel/UCesD1HRn9NPKXcyXV0-8oMg)** *[26.05.2026 05:43](https://www.youtube.com/watch?v=DjuK8h7-ep8&lc=UgyX9cyiZZT8T1AAFdx4AaABAg)*

0:00:00 Вступление: обсуждение вопроса подписчика о производительности Math.trunc и оператора OR
0:05:40 Демонстрация оригинального кода теста и повторение результатов
0:12:09 Разбор того, что именно делают Math.trunc и битовый OR
0:16:55 Написание собственного теста для проверки производительности
0:21:49 Анализ результатов и поиск причин странного поведения
0:34:44 Разница между оптимизированным и неоптимизированным кодом в V8
0:56:18 Изоляция тестируемого кода: почему важно отключать внешние влияния
1:06:00 Сравнение производительности при вынесении логики во внешнюю функцию
1:12:14 Вывод о том, что тест измерял не скорость операций, а особенности работы с данными
1:26:44 Обсуждение приведения типов (ToInt32) и ограничений 32-битной архитектуры
1:56:48 Разбор сгенерированного машинного кода и Pointer Compression
2:31:25 Итоговый вывод: почему возникала разница и как правильно тестировать производительность

---
