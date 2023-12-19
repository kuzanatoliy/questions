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
