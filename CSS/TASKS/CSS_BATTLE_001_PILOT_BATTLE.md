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
    </style>

</details>

<details>
  <summary>#7 - Leafy Trail</summary>

  [Task](https://cssbattle.dev/play/7)

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
    </style>

</details>

<details>
  <summary>#8 - Forking Crazy</summary>

  [Task](https://cssbattle.dev/play/8)

    <div class="bg">
      <div class="upward-circle"></div>
      <div class="upward-circle left-margin"></div>
      <div class="upward-circle left-margin"></div>
      <div class="upward-circle left-margin"></div>
    </div>
    <div id="striped"></div>
    <div class="bg darker">
      <div class="downward-circle left-margin"></div>
      <div class="downward-circle left-margin"></div>
      <div class="downward-circle left-margin"></div>
    </div>
    <div id="bottom"></div>
    <div id="stick"></div>

    <style>
      body {
        padding: 42px 122px 0;
        background: #6592CF;
      }
      .bg {
        font-size: 0;
        width: 140px;
        height: 20px;
      }
      .darker {
        background: #060F55;
      }
      .left-margin {
        margin-left: 20px;
      }
      #striped {
        width: 140px;
        height: 70px;
        background: repeating-linear-gradient(
          to right,
          #060F55 0px,
          #060F55 20px,
          #6592CF 20px,
          #6592CF 40px);
      }
      #bottom {
        width: 140px;
        height: 90px;
        background: #060F55;
        border-radius: 0 0 100px 100px;
      }
      .upward-circle {
        width: 20px;
        height: 20px;
        background: #060F55;
        border-radius: 20px 20px 0 0;
        display: inline-block;
      }
      .downward-circle {
        width: 20px;
        height: 20px;
        background: #6592CF;
        border-radius: 0 0 20px 20px;
        display: inline-block;
      }
      #stick {
        width: 20px;
        height: 60px;
        z-index: 1;
        position: relative;
        top: -10px;
        background: #060F55;
        margin-left: 60px;
      }
    </style>

</details>

<details>
  <summary>#8 - Forking Crazy</summary>

  [Task](https://cssbattle.dev/play/8)

    <div class="bg">
      <div class="upward-circle"></div>
      <div class="upward-circle left-margin"></div>
      <div class="upward-circle left-margin"></div>
      <div class="upward-circle left-margin"></div>
    </div>
    <div id="striped"></div>
    <div class="bg darker">
      <div class="downward-circle left-margin"></div>
      <div class="downward-circle left-margin"></div>
      <div class="downward-circle left-margin"></div>
    </div>
    <div id="bottom"></div>
    <div id="stick"></div>

    <style>
      body {
        padding: 42px 122px 0;
        background: #6592CF;
      }
      .bg {
        font-size: 0;
        width: 140px;
        height: 20px;
      }
      .darker {
        background: #060F55;
      }
      .left-margin {
        margin-left: 20px;
      }
      #striped {
        width: 140px;
        height: 70px;
        background: repeating-linear-gradient(
          to right,
          #060F55 0px,
          #060F55 20px,
          #6592CF 20px,
          #6592CF 40px);
      }
      #bottom {
        width: 140px;
        height: 90px;
        background: #060F55;
        border-radius: 0 0 100px 100px;
      }
      .upward-circle {
        width: 20px;
        height: 20px;
        background: #060F55;
        border-radius: 20px 20px 0 0;
        display: inline-block;
      }
      .downward-circle {
        width: 20px;
        height: 20px;
        background: #6592CF;
        border-radius: 0 0 20px 20px;
        display: inline-block;
      }
      #stick {
        width: 20px;
        height: 60px;
        z-index: 1;
        position: relative;
        top: -10px;
        background: #060F55;
        margin-left: 60px;
      }
    </style>

</details>
