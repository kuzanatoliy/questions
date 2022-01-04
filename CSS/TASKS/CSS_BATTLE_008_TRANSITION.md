# CSS battle 008 Transition

## Links
[source](https://cssbattle.dev/battle/8)

## Tasks

<details>
  <summary>#42 - Baby</summary>

  [Task](https://cssbattle.dev/play/42)

    <div><p a><p a><p b>
    <style>
      body {
        margin: 50px 100px;
        background: #293462;
      }
      div {
        position: relative;
        height: 100%;
        background: #FE5F55;
        border-radius: 100% 100% 50% 50%;
        overflow: hidden;
      }
      p {
        width: 60px;
        height: 60px;
        background: #FFF1C1;
        border-radius: 50%;
        position: absolute;
        top: 74px;
        left: 20px;
      }
      p + p {
        left: 120px;
      }
      [a] {
        box-shadow: 0px -120px 0 20px #FFF1C1;
      }
      [b] {
        width: 40px;
        height: 10px;
        top: 154px;
        left: 80px;
        border-radius: 10px;
      }
    </style>

</details>

<details>
  <summary>#43 - Wrench</summary>

  [Task](https://cssbattle.dev/play/43)

    <p><p>
    <style>
      body {
        margin: 30px 0 0 145px;
      background: #6592CF;
      }
      p {
        margin: 0;
        width: 40px;
        height: 182px;
        border: solid 30px #243D83;
        border-radius: 0 100px 100px 0;
        border-left: none;
        float: left;
      }
      p + p {
        margin-left: -30px;
        transform: rotate(180deg);
      }
    </style>

</details>
