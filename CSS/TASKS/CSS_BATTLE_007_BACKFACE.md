# CSS battle 007 Backface

## Links
[source](https://cssbattle.dev/battle/7)

## Tasks

<details>
  <summary>#33 - Birdie</summary>

  [Task](https://cssbattle.dev/play/33)

    <p><p><p a>
    <style>
      * {
        margin: 0;
        background: #1A4341;
      }
      p {
        position: fixed;
        width: 75px;
        height: 150px;
        top: 75px;
        left: 125px;
        background: #998235;
        border-radius: 100px 0 0 100px;
      }
      p + p {
        width: 100px;
        height: 100px;
        top: 50px;
        left: 200px;
        background: #F3AC3C;
        border-radius: 0 100px 0 0;
      }
      [a] {
        width: 30px;
        height: 30px;
        top: 105px;
        left: 155px;
        background: #0B2429;
        border-radius: 50%;
      }
    </style>

</details>

<details>
  <summary>#34 - Chrismas Tree</summary>

  [Task](https://cssbattle.dev/play/34)

    <p><p a><p b>
    <style>
      body {
        background: #007065;
      }
      p {
        position: fixed;
        bottom: 21px;
        left: 75px;
        width: 250px;
        height: 100px;
        background: #FFEECF;
        border: solid 125px #007065;
        border-top: none;
        box-sizing: border-box;
        border-bottom-color: #00A79D;
        overflow: hidden;
        transform: rotateX(37deg);
      }
      [a] {
        bottom: 71px;
        border-bottom-color: #F5C181;
      }
      [b] {
        bottom: 121px;
        border-bottom-color: #FFEECF;
      }
    </style>

</details>

<details>
  <summary>#35 - Ice Cream</summary>

  [Task](https://cssbattle.dev/play/35)

    <p a><p b><p c>
    <style>
      body {
        margin: 50px 150px;
        background: #293462;
      }
      [a] {
        margin-bottom: 0;
        width: 100px;
        height: 150px;
        background: #FFF1C1;
        border-radius: 100px 100px 40px 40px;
      }
      [b], [c] {
        margin: 0 35px;
        height: 10px;
        width: 30px;
        background: #A64942;
      }
      [c] {
        height: 40px;
        border-radius: 0 0 10px 10px;
        background: #FE5F55;
      }
    </style>

</details>

<details>
  <summary>#36 - Interleaved</summary>

  [Task](https://cssbattle.dev/play/36)

    <p a><p><p a><p><p a>
    <style>
      body {
        margin: 0 25px;
        background: #1A4341;
        display: flex;
        justify-content: space-between;
      }
      p {
        margin: 0;
        width: 50px;
        height: 200px;
        background: #998235;
        border-radius: 0 0 50px 50px;
      }
      [a] {
        align-self: flex-end;
        transform: rotateX(180deg);
        background: #F3AC3C;
      }
    </style>

</details>

<details>
  <summary>#37 - Tunnel</summary>

  [Task](https://cssbattle.dev/play/37)

    <div><div a>
    <style>
      * {
        position: relative;
        width: 100%;
        height: 100%;
      }
      body {
        margin: 25px 75px;
        width: 250px;
        height: 250px;
        background: #243D83;
        box-shadow: 0 0 0 75px #6592CF;
      }
      div {
        top: 50px;
        left: 50px;
        width: 150px;
        height: 150px;
        transform: rotate(15deg);
        background: #6592CF;
      }
      [a] {
        top: 38px;
        left: 38px;
        width: 75px;
        height: 75px;
        background: #243D83;
      }
    </style>

</details>

<details>
  <summary>#38 - Not Simply Square</summary>

  [Task](https://cssbattle.dev/play/38)

    <p><p a><p b>
    <style>
      * {
        margin: 0;
        background: #293462;
      }
      p {
        width: 200px;
        height: 200px;
        background: #FFF1C1;
      }
      p {
        position: fixed;
        height: 200px;
        width: 300px;
        background: linear-gradient(#FE5F55 75%, 0, #A64942);
      }
      [a] {
        transform: rotate(-90deg);
        top: 50px;
        left: -50px;
      }
      [b] {
        width: 200px;
        background: #FFF1C1;
      }
    </style>

</details>

<details>
  <summary>#39 - Sunset</summary>

  [Task](https://cssbattle.dev/play/39)

    <div><p><div>
    <style>
      body {
        margin: 25px 75px;
        background: #1A4341;
      }
      * {
        position: absolute;
      }
      div {
        width: 250px;
        height: 250px;
        border-radius: 50%;
        overflow: hidden;
      }
      div > div {
        margin: 25px;
        width: 200px;
        height: 200px;
        border-radius: 50%;
        background: #998235;
      }
      p {
        margin-top: 55px;
        height: 140px;
        width: 100%;
        background: repeating-linear-gradient(#1A4341, #1A4341 20px, #F3AC3C 20px, #F3AC3C 40px);
        z-index: 1;
      }
    </style>

</details>
<details>
  <summary>#40 - Letter B</summary>

  [Task](https://cssbattle.dev/play/40)

    <div><p>
    <style>
      body {
        margin: 50px 100px;
        background: #6592CF;
      }
      div {
        height: 100%;
        background: #6592CF;
        border-radius: 0 50% 50%;
        box-shadow: inset 0 0 0 50px #243D83;
      }
      p {
        width: 50px;
        height: 100px;
        margin: 0 50px;
        background: #6592CF;
      }
    </style>

</details>
