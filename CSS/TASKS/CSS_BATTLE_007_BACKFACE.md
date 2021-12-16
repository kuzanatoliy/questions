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