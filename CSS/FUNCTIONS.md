# Functions

<details>
  <summary>What is an abs function?</summary>

The `abs()` CSS function returns the absolute value of the argument, as the same type as the input.

Example:

    div {
      --deg: -45deg;
      background-image: linear-gradient(abs(var(--deg)), blue, red);
    }

[More >>](https://developer.mozilla.org/en-US/docs/Web/CSS/abs)

</details>

<details>
  <summary>What is an acos function?</summary>

The `acos()` CSS function is a trigonometric function that returns the inverse cosine of a number between `-1` and `1`. The function contains a single calculation that returns the number of radians representing an angle between `0deg` and `180deg`.

Example:

    div.box-1 {
      transform: rotate(acos(1));
    }
    div.box-2 {
      transform: rotate(acos(0.5));
    }

[More >>](https://developer.mozilla.org/en-US/docs/Web/CSS/acos)

</details>

<details>
  <summary>What is an asin function?</summary>

The `asin()` CSS function is a trigonometric function that returns the inverse sine of a number between `-1` and `1`. The function contains a single calculation that returns the number of radians representing an angle between `-90deg` and `90deg`.

Example:

    div.box-1 {
      transform: rotate(asin(1));
    }
    div.box-2 {
      transform: rotate(asin(0.5));
    }

[More >>](https://developer.mozilla.org/en-US/docs/Web/CSS/asin)

</details>

<details>
  <summary>What is an atan function?</summary>

The `atan()` CSS function is a trigonometric function that returns the inverse tangent of a number between `-∞` and `+∞`. The function contains a single calculation that returns the number of radians representing an angle between `-90deg` and `90deg`.

Example:

    div.box-1 {
      transform: rotate(atan(1));
    }
    div.box-2 {
      transform: rotate(atan(0.5));
    }

[More >>](https://developer.mozilla.org/en-US/docs/Web/CSS/atan)

</details>

<details>
  <summary>What is an atan2 function?</summary>

The `atan2()` CSS function is a trigonometric function that returns the inverse tangent of two values between `-infinity` and `infinity`. The function accepts two arguments and returns the number of radians representing an angle between `-180deg` and `180deg`.

Example:

    div.box-1 {
      transform: rotate(atan2(3, 2));
    }
    div.box-2 {
      transform: rotate(atan2(-1, 0.5));
    }

[More >>](https://developer.mozilla.org/en-US/docs/Web/CSS/atan2)

</details>

<details>
  <summary>What is an attr function?</summary>

The `attr()` CSS function is used to retrieve the value of an attribute of the selected element and use it in the stylesheet. It can also be used on pseudo-elements, in which case the value of the attribute on the pseudo-element's originating element is returned.

Example:

    <p data-foo="hello">world</p>

    [data-foo]::before {
      content: attr(data-foo) " ";
    }

[More >>](https://developer.mozilla.org/en-US/docs/Web/CSS/attr)

</details>

<details>
  <summary>What is a calc function?</summary>

The `calc()` CSS function lets one to perform calculations when specifying CSS property values. It can be used with `length`, `frequency`, `angle`, `time`, `percentage`, `number` or `integer` values.

Example:

    width: calc(100% - 80px);

[More >>](https://developer.mozilla.org/en-US/docs/Web/CSS/calc)

</details>

<details>
  <summary>What is a clamp function?</summary>

The `clamp()` CSS function clamps a middle value within a range of values between a defined minimum bound and a maximum bound. The function takes three parameters: a minimum value, a preferred value, and a maximim allowed value.

Example:

    h1 {
      letter-spacing: 2px;
      font-size: clamp(1.8rem, 2.5vw, 2.8rem);
    }

[More >>](https://developer.mozilla.org/en-US/docs/Web/CSS/clamp)

</details>

<details>
  <summary>What is a cos function?</summary>

The `cos()` CSS function is a trigonometric function that returns the cosine of a number, which is a value between `-1` and `1`. The function contains a single calculation that must resolve to either a number or an angle by interpreting the result of the argument as radians. That is, `cos(45deg)`, `cos(0.125turn)`, and `cos(3.14159 / 4)` all represent the same value, approximately `0.707`.

Example:

    div.rotated-scaled-diamond {
      width: calc(100px * cos(45deg));
      height: calc(100px * cos(45deg));
      margin: calc(100px / 4 * cos(45deg));
      transform: rotate(45deg);
      transform-origin: center;
      background-color: green;
    }

[More >>](https://developer.mozilla.org/en-US/docs/Web/CSS/cos)

</details>

<details>
  <summary>What is a counter function?</summary>

The `counter()` CSS function returns a string representing the current value of the named counter, if there is one.

Example:

    ol {
      counter-reset: listCounter;
      padding-left: 5em;
    }
    li {
      counter-increment: listCounter;
    }
    li::marker {
      content:
        "Item #" counter(listCounter) " is: ";
    }
    li::after {
      content:
        "[" counter(listCounter, decimal-leading-zero) "] == ["
        counter(listCounter, upper-roman) "]";
    }

[More >>](https://developer.mozilla.org/en-US/docs/Web/CSS/counter)

</details>

<details>
  <summary>What is a counters function?</summary>

The `counters()` CSS function enables combining markers when nesting counters. The function returns a string that concatenates the current values of the named and nested counters. The function returns a string that concatenates the current values of the named and nested counters, if any are present, with the string provided. The third, optional parameter enables defining the list style.

Example:

    ol {
      counter-reset: listCounter;
    }
    li {
      counter-increment: listCounter;
    }
    li::marker {
      content:
        counters(listCounter, ".", upper-roman) ") ";
    }
    li::before {
      content:
        counters(listCounter, ".") " == "
        counters(listCounter, ".", lower-roman);
    }

[More >>](https://developer.mozilla.org/en-US/docs/Web/CSS/counters)

</details>

<details>
  <summary>What is a cross-fade function?</summary>

The `cross-fade()` CSS function can be used to blend two or more images at a defined transparency. It can be used for many simple image manipulations, such as tinting an image with a solid color or highlighting a particular area of the page by combining an image with a radial gradient.

Example:

    .crossfade {
      width: 300px;
      height: 300px;
      background-image: -webkit-cross-fade(url("br.png"), url("tr.png"), 75%);
      background-image: cross-fade(url("br.png"), url("tr.png"), 75%);
    }

[More >>](https://developer.mozilla.org/en-US/docs/Web/CSS/cross-fade)

</details>

<details>
  <summary>What is an element function?</summary>

The `element()` CSS function defines an image value generated from an arbitary HTML element. This image is live, meaning that if the HTML element is changed, the CSS properties using the resulting value are automatically updated.

Example:

    #css-result {
      background: -moz-element(#css-source) no-repeat;
      width: 256px;
      height: 32px;
      background-size: 80%;
      border: dashed;
    }

[More >>](https://developer.mozilla.org/en-US/docs/Web/CSS/element)

</details>
