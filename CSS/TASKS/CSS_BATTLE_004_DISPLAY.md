# CSS battle 004 Display

## Links
[source](https://cssbattle.dev/battle/4)

## Tasks

<details>
  <summary>#21 - SitePoint Logo</summary>

  [Task](https://cssbattle.dev/play/21)

    <div a><p/><p/></div><div b><p/><p/></div>
    <style>
      body {
        background: #222;
      }
      div {
        position: fixed;
      }
      [a] {
        transform: rotate(-45deg);
        left: 138px;
        top: 85px;
      }
      [b] {
        transform: rotate(135deg);
        right: 140px;
        bottom: 86px;
      }
      [a] > p {
        background: #F2994A;
      }
      [b] > p {
        background: #2D9CDB;
      }
      p {
        margin: 0;
        width: 100px;
        height: 30px;
        border-radius: 10px 0 0;
      }
      p + p {
        margin: -1px 0;
        width: 29px;
        height: 51px;
        border-radius: 0 0 5px;
      }
    </style>

</details>

<details>
  <summary>#22 - Cloud</summary>

  [Task](https://cssbattle.dev/play/22)

    <p a><p b><p c>
    <style>
      * {
        background: #F5D6B4;
      }
      p {
        background: #D86F45;
        width: 100px;
        height: 100px;
        position: fixed;
        border-radius: 50%;
      }
      [a] {
        left: 99px;
        top: 99px;
      }
      [b] {
        left: 180px;
        top: 69px;
      }
      [c] {
        width: 170px;
        height: 50px;
        border-radius: 25px;
        left: 130px;
        top: 149px;
      }
    </style>

</details>

<details>
  <summary>#23 - Boxception</summary>

  [Task](https://cssbattle.dev/play/23)

    <div>
    <style>
      * {
        background: #F3AC3C;
      }
      div {
        position: fixed;
        width: 100px;
        height: 100px;
        left: 100px;
        top: 150px;
        box-shadow: 50px -50px 0 50px #1A4341, inset 50px 50px #998235;
      }
    </style>

</details>

<details>
  <summary>#24 - Switches</summary>

  [Task](https://cssbattle.dev/play/24)

    <p a><p b><p c><p d>
    <style>
      * {
        margin: 0;
        background: #62306D;
      }
      p {
        position: fixed;
        width: 100px;
        height: 100px;
        top: 100px;
        left: 80px;
        background: #F7EC7D;
        border-radius: 100px;
      }
      [c], [b] {
        left: 220px;
      }
      [a], [b] {
        height: 150px;
      }
      [a] {
        top: 50px;
        background: #AA445F;
      }
      [b] {
        left: 220px;
        background: #E38F66;
      }
    </style>

</details>
