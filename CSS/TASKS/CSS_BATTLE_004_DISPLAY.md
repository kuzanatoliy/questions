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

<details>
  <summary>#25 - Blossom</summary>

  [Task](https://cssbattle.dev/play/25)

    <div><p><p></div><div><p><p></div>
    <style>
      body {
        margin: 44px 0 0 110px;
        background: #998235;
      }
      div {
        float: left;
        margin-right: 20px;
      }
      div + div {
        transform: rotate(180deg) rotateY(180deg);
      }
      p {
        width: 80px;
        height: 100px;
        background: #1A4341;
        border-radius: 0 50px;
      }
      p + p {
        height: 60px;
        background: #F3AC3C;
        margin-top: 20px;
      }
    </style>

</details>

<details>
  <summary>#26 - Smiley</summary>

  [Task](https://cssbattle.dev/play/26)

    <p><p a><p>
    <style>
      body {
        margin: 40px 40px;
        display: flex;
        background: #6592CF;
      }
      p {
        margin: 0;
        width: 80px;
        height: 40px;
        border-radius: 100px 100px 0 0;
        border: solid 20px #060F55;
        border-bottom: 0;
      }
      p + p {
        margin-left: -20px;
      }
      [a] {
        align-self: flex-end;
        transform: rotateX(180deg);
      }
    </style>

</details>

<details>
  <summary>#27 - Lock Up</summary>

  [Task](https://cssbattle.dev/play/27)

    <p><p a><p b><p c>
    <style>
      body {
        margin: 50px 100px;
        background: #AA445F;
        box-shadow: 0 0 0 100vw #E38F66;
        border-radius: 50%;
      }
      p {
        position: absolute;
        width: 70px;
        height: 70px;
        background: #F7EC7D;
        border-radius: 0 100% 0 0;
        margin: 30px 100px;
      }
      [a], [c] {
        background: #AA445F;
        width: 40px;
        height: 40px;
        margin-top: 60px;
      }
      [b], [c] {
        border-radius: 0 0 0 100px;
        margin: 100px 30px;
      }
      [c] {
        margin-left: 60px;
      }
    </style>

</details>

<details>
  <summary>#28 - Cups & Balls</summary>

  [Task](https://cssbattle.dev/play/28)

    <p a><p c b><p b><p c a><p c d><p a><p c a><p d>
    <style>
      body {
        background: #1A4341;
        margin: 80px 60px;
      }
      p {
        float: left;
        width: 50px;
        height: 50px;
        background: #998235;
        margin: 10px;
      }
      [c] {
        background: #F3AC3C;
      }
      [a] {
        border-radius: 50%;
      }
      [b] {
        border-radius: 50% 50% 0 0;
      }
      [d] {
        border-radius: 0 0 50% 50%;
      }
    </style>

</details>