# CSS battle 001 Pilot battle

## Links
[source](https://cssbattle.dev/battle/1)

## Tasks

<details>
  <summary>#1 - Simply Square</summary>

  [Task](https://cssbattle.dev/play/1)

    <div></div>
    <style>
      div {
        margin: -8px;
        width: 200px;
        height: 200px;
        background: #b5e0ba;
        box-shadow: 0 0 0 200px #5d3a3a;
      }
    </style>

</details>

<details>
  <summary>#2 - Carrom</summary>

  [Task](https://cssbattle.dev/play/2)

    <div></div><div></div><div></div><div></div>
    <style>
      body {
        margin: 0;
        background: #62374e;
      }
      div {
        margin: 50px;
        float: left;
        width: 50px;
        height: 50px;
        background: #fdc57b;
      }
      div:nth-of-type(2n + 1) {
        margin-right: 150px;
      }
    </style>

</details>

<details>
  <summary>#3 - Push Button</summary>

  [Task](https://cssbattle.dev/play/3)

    <div><div>
    <style>
      body {
        margin: 0;
        padding: 75px 50px;
        background: #6592CF;
      }
      div {
        height: 150px;
        background: #243D83;
      }
      div div {
        margin: 0 75px;
        border: solid 50px #243D83;
        box-shadow: 0 0 0 50px #6592CF;
        border-radius: 50%;
        width: 50px;
        height: 50px;
        background: #EEB850;
      }
    </style>

</details>

<details>
  <summary>#4 - Ups n Downs</summary>

  [Task](https://cssbattle.dev/play/4)

    <div></div><div></div><div></div><div></div><div></div><div>
    <style>
      body {
        margin: 0;
        background: #62306D;
        padding: 50px;
      }
      div {
        float: left;
        width: 100px;
        height: 100px;
      }
      div:nth-of-type(2n) {
        background: #F7EC7D;
        border-radius: 50% 50% 0 0;
      }
      div:nth-of-type(2n + 4) {
        transform: rotate(180deg);
      }
    </style>

</details>

<details>
  <summary>#5 - Acid Rain</summary>

  [Task](https://cssbattle.dev/play/5)

    <div></div><div></div><div></div>
    <style>
      body {
        margin: 0;
        background: #0B2429;
        position: relative;
      }
      div {
        position: absolute;
        right: 80px;
        top: 30px;
        width: 120px;
        height: 120px;
        background: #F3AC3C;
        border-radius: 50% 50% 50% 0;
      }
      div + div {
        right: 140px;
        top: 90px;
        transform: rotate(0.5turn);
      }
      div + div + div {
        right: 200px;
        top: 150px;
      }
      div:nth-of-type(2n) {
        background: #998235;
      }
    </style>

</details>

<details>
  <summary>#6 - Missing Slice</summary>

  [Task](https://cssbattle.dev/play/6)

    <div class=a></div><div class=b></div><div class=c></div>
    <style>
      body {
        margin: 0;
        background: #E3516E;
        padding: 50px 100px;
      }
      div {
        width: 100px;
        height: 100px;
        background: #dd6b4d;
        float: left;
      }
      .a {
        background: #51B5A9;
        border-radius: 100% 0 0 0;
      }
      .b {
        background: #FADE8B;
        border-radius: 0 100% 0 0;
      }
      .c {
        background: #F7F3D7;
        border-radius: 0 0 0 100%;
      }
    </style>z

</details>
