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
