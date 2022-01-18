# CSS battle 002 Visibility

### Links

[source](https://cssbattle.dev/battle/2)

### Tasks

<details>
  <summary>#13 - Totally Triangle</summary>

[Task](https://cssbattle.dev/play/13)

    <p>
    <style>
      body {
        margin: 0;
        background: #0B2429
      }
      p {
        margin: -100;
        width: 200;
        height: 200;
        transform: rotate(45deg);background: #F3AC3C;
      }
    </style>

</details>

<details>
  <summary>#14 - Web Maker Logo</summary>

[Task](https://cssbattle.dev/play/14)

    <p t1><p t2>
    <style>
      body {
        background: #F2F2B6;
      }
      p {
        margin: 0;
        height: 0;
        width: 0;
        position: absolute;
        border: solid 75px rgba(0,0,0,0);
      }
      [t1] {
        top: 85;
        left: 60;
        border-top: solid 130px #FF6D00;
        filter: drop-shadow(20px 0px #FD4602);
      }
      [t2] {
        bottom: 85;
        right: 80;
        border-bottom: solid 130px #FD4602;
        filter: drop-shadow(20px 0px #FF6D00);
      }
    </style>

</details>

<details>
  <summary>#15 - Overlap</summary>

[Task](https://cssbattle.dev/play/15)

    <p>
    <style>
      * {
        margin: 0px;
        background: #09042A;
      }
      p {
        position: absolute;
        top: 75px;
        left: 75px;
        width: 150px;
        height: 150px;
        border-radius: 50%;
        box-shadow: 100px 0px #E78481, inset 100px 0px #7B3F61;
      }
    </style>

</details>

<details>
  <summary>#16 - Eye of the Tiger</summary>

[Task](https://cssbattle.dev/play/16)

    <p>
    <style>
      * {
        background: #0B2429;
      }
      p {
        width: 200px;
        height: 200px;
        margin: 50px 92px;
        background: radial-gradient(#0b2429 25px,0,#f3ac3c 70px,0,#0b2429 90px,0,#998235);
        border-radius: 50% 0;
        transform: rotate(45deg);
      }
    </style>

</details>

<details>
  <summary>#17 - Fidget Spinner</summary>

[Task](https://cssbattle.dev/play/17)

    <p t><p a><p b><p c><p d>
    <style>
      * {
        background: #09042A;
        position: absolute;
      }
      p {
        width: 60px;
        height: 60px;
        background: #F5BB9C;
        border-radius: 50px;
      }
      [t] {
        height: 50px;
        top: 100px;
        left: 140px;
        background: #E78481;
        width: 100px;
      }
      [a] {
        top: 33px;
      }
      [b] {
        top: 139px;
      }
      [c] {
        left: 92px;
      }
      [d] {
        left: 212px;
      }
      [a],[b] {
        left: 152px;
        border: solid 10px #09042A;
      }
      [c],[d] {
        top: 86px;
        border: solid 10px #E78481;
        background: #09042A;
      }
    </style>

</details>

<details>
  <summary>#18 - Matrix</summary>

    [Task](https://cssbattle.dev/play/18)

    <p><p a><p><p a><p a><p><p a><p><p><p a><p><p a>
    <style>
      body {
        margin: 0;
        background: #5C434C;
      }
      p {
        margin: 10px;
        float: left;
        width: 80px;
        height: 80px;
        background: #F09462;
        border-radius: 100% 0 0;
      }
      [a] {
        background: #F5D6B4;
      }
    </style>

</details>
