---
title: min-height
slug: Web/CSS/min-height
---

{{CSSRef}}

Свойство [CSS](/ru/docs/Web/CSS) **`min-height`** устанавливает минимальную высоту элемента. Оно предотвращает [используемое значение](/ru/docs/conflicting/Web/CSS/CSS_cascade/Value_processing_67ecc2d1089286b6003d201c901ee7218b8f627858ae89823dc40509095cd65b) свойства {{ Cssxref("height") }} от становления меньше, чем значение, указанное для `min-height`.

{{InteractiveExample("CSS Demo: min-height")}}

```css interactive-example-choice
min-height: 150px;
```

```css interactive-example-choice
min-height: 7em;
```

```css interactive-example-choice
min-height: 75%;
```

```css interactive-example-choice
min-height: 10px;
```

```html interactive-example
<section class="default-example" id="default-example">
  <div class="transition-all" id="example-element">
    This is a box where you can change the minimum height. <br />If there is
    more content than the minimum the box will grow to the height needed by the
    content.
  </div>
</section>
```

```css interactive-example
#example-element {
  display: flex;
  flex-direction: column;
  background-color: #5b6dcd;
  justify-content: center;
  color: #ffffff;
}
```

Высота элемента принимает значение `min-height` всякий раз, когда `min-height` больше чем {{ Cssxref("max-height") }} или {{Cssxref("height")}}.

## Синтаксис

```css
/* Ключевые слова */
min-height: max-content;
min-height: min-content;
min-height: fit-content;
min-height: fill-available;

/* <length> значения */
min-height: 3.5em;

/* <percentage> значения */
min-height: 10%;

/* Глобальные значения */
min-height: inherit;
min-height: initial;
min-height: unset;
```

### Значения

- {{cssxref("&lt;length&gt;")}}
  - : Минимальная высота выражается как {{cssxref("&lt;length&gt;")}}. Отрицательные значения делают свойство недействительным.
- {{cssxref("&lt;percentage&gt;")}}
  - : Минимальная высота выражается как {{cssxref("&lt;percentage&gt;")}} от высоты родительского блока. Отрицательные значения делают свойство недействительным.

#### Значения-ключевые слова

- `auto`
  - : Минимальная высота для flex-элементов по умолчанию, предоставляет более разумное значение по умолчанию, чем 0 для других способов разметки.

<!---->

- `max-content` {{ experimental_inline() }}
  - : Внутренняя предпочтительная высота.
- `min-content` {{ experimental_inline() }}
  - : Внутренняя минимальная высота.
- `fill-available`{{ experimental_inline() }}
  - : Высота родительского блока минус вертикальные `margin`, `border`, и `padding`. (Обратите внимание, что некоторые браузеры реализуют устаревшее имя для этого ключевого слова., `available`.)
- `fit-content` {{ experimental_inline() }}
  - : Согласно CSS3 Box, это синоним `min-content`. CSS3 Sizing определяет более сложный алгоритм, но ни один браузер не реализует его даже экспериментальным путём.

### Формальный синтаксис

{{csssyntax}}

## Примеры

```css
table {
  min-height: 75%;
}

form {
  min-height: 0;
}
```

## Спецификации

{{Specifications}}

{{cssinfo}}

## Совместимость с браузерами

{{Compat}}

## Смотрите также

- {{ Cssxref("height") }}, {{ Cssxref("max-height") }}
- [Блочная модель](/ru/docs/Web/CSS/CSS_box_model/Introduction_to_the_CSS_box_model), {{ Cssxref("box-sizing") }}
