---
title: Инструкции и объявления
slug: Web/JavaScript/Reference/Statements
---

{{jsSidebar("Statements")}}

Приложения на JavaScript состоят из инструкций с соответствующим синтаксисом. Одна инструкция может состоять из нескольких строк. На одной строке может находиться несколько инструкций, если они разделены точкой с запятой. Они являются не ключевыми словами, а группами ключевых слов.

## Инструкции и объявления по категориям

Алфавитный список смотрите в боковой панели слева.

### Управление потоком выполнения

- {{jsxref("Statements/return", "return")}}
  - : Определяет значение, возвращаемое функцией.
- {{jsxref("Statements/break", "break")}}
  - : Прерывает текущую инструкцию цикла, ветвления или инструкцию с меткой и передаёт управление на инструкцию, следующую за прерываемой.
- {{jsxref("Statements/continue", "continue")}}
  - : Прерывает выполнение инструкции в текущей итерации текущего цикла или цикла с меткой и продолжает выполнение цикла со следующей итерации.
- {{jsxref("Statements/throw", "throw")}}
  - : Генерирует определённое пользователем исключение.
- {{jsxref("Statements/if...else", "if...else")}}
  - : Выполняет инструкцию, если указанное условие является истинным. Если условие ложно, выполняет другую инструкцию.
- {{jsxref("Statements/switch", "switch")}}
  - : Вычисляет выражение, сопоставляет вычисленное значение с выражением выбора и выполняет инструкции, ассоциированные с этим выбором.
- {{jsxref("Statements/try...catch", "try...catch")}}
  - : Помечает блок инструкций и определяет реакцию на возникновение исключения внутри помеченного блока инструкций.

### Объявления

- {{jsxref("Statements/var", "var")}}
  - : Объявляет переменную, необязательно инициализирует её значением.
- {{jsxref("Statements/let", "let")}}
  - : Объявляет локальную переменную в области видимости блока, необязательно инициализирует её значением.
- {{jsxref("Statements/const", "const")}}
  - : Объявляет именованную константу только для чтения.

### Функции и классы

- {{jsxref("Statements/function", "function")}}
  - : Объявляет функцию с указанными параметрами.
- {{jsxref("Statements/function*", "function*")}}
  - : Функции-генераторы, упрощающие написание [итераторов](/ru/docs/Web/JavaScript/Reference/Iteration_protocols).
- {{jsxref("Statements/async_function", "async function")}}
  - : Объявляет асинхронную функцию с указанными параметрами.
- {{jsxref("Statements/async_function*", "async function*")}}
  - : Асинхронные функции-генераторы, упрощающие написание асинхронных [итераторов](/ru/docs/Web/JavaScript/Reference/Iteration_protocols).
- {{jsxref("Statements/class", "class")}}
  - : Объявляет класс.

### Итерации

- {{jsxref("Statements/do...while", "do...while")}}
  - : Создаёт цикл, выполняющий указанную инструкцию до тех пор, пока проверяющее условие равно `false`. Условие вычисляется после выполнения инструкции, так что указанная инструкция выполнится хотя бы один раз.
- {{jsxref("Statements/for", "for")}}
  - : Создаёт цикл, состоящий из трёх необязательных выражений, заключённых в круглые скобки и разделённым точками с запятой с последующей инструкцией, выполняющейся в цикле.
- {{jsxref("Statements/for...in", "for...in")}}
  - : В случайном порядке проходит по перечислимым свойствам объекта. Выполняет инструкции для каждого уникального свойства.
- {{jsxref("Statements/for...of", "for...of")}}
  - : Проходит по итерируемым объектам (включая {{jsxref("Global_Objects/Array", "массивы", "", 1)}}, массивоподобные объекты, [итераторы и генераторы](/ru/docs/Web/JavaScript/Guide/Iterators_and_generators)), выполняя указанные инструкции для значения каждого отдельного свойства.
- {{jsxref("Statements/for-await...of", "for await...of")}}
  - : Проходит по асинхронным итерируемым объектам, массивоподобным объектам, [итераторам и генераторам](/ru/docs/Web/JavaScript/Guide/Iterators_and_generators), выполняя указанные инструкции для значения каждого отдельного свойства.
- {{jsxref("Statements/while", "while")}}
  - : Создаёт цикл, выполняющий указанную инструкцию до тех пор, пока проверяющее условие равно `true`. Условие вычисляется перед выполнением инструкции..

### Прочее

- {{jsxref("Statements/Empty", "Пустая инструкция", "", 1)}}
  - : Пустая инструкция используется для того, чтобы не указывать никакой инструкции, хотя синтаксис JavaScript предполагает её наличие.
- {{jsxref("Statements/block", "Блок", "", 1)}}
  - : Блок используется для группировки нуля и более инструкций. Блок отделяется парой фигурных скобок.
- {{jsxref("Statements/Expression_statement", "Выражение", "", 1)}}
  - : Вычисляет выражение и игнорирует его результат. Это позволяет использовать побочные эффекты, такие как вызов функции и обновление переменной.
- {{jsxref("Statements/debugger", "debugger")}}
  - : Вызывает любую доступную функциональность отладки. Если функциональность отладки не доступна, эта инструкция ничего не делает.
- {{jsxref("Statements/export", "export")}}
  - : Используется для экспорта подписанным скриптом свойств, функций и объектов в другие подписанные или неподписанные скрипты. Эта древняя функциональность Netscape была удалена и будет пересмотрена модулями ECMAScript 6.
- {{jsxref("Statements/import", "import")}}
  - : Используется для импорта скриптом свойств, функций и объектов из подписанного скрипта, который предоставил эту информацию. Эта древняя функциональность Netscape была удалена и будет пересмотрена модулями ECMAScript 6.
- {{jsxref("Statements/label", "label")}}
  - : Предоставляет инструкцию с идентификатором, на который вы можете сослаться с помощью инструкций `break` или `continue`.
- {{deprecated_inline}} {{jsxref("Statements/with", "with")}}
  - : Расширяет цепочку областей видимости инструкции.

## Спецификации

{{Specifications}}

## Смотрите также

- {{jsxref("Operators", "Операторы", "", 1)}}
