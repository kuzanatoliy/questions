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
