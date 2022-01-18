# CSS battle 001 Pilot battle

### Links

[source](https://cssbattle.dev/battle/1)

### Tasks

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
  <summary>#9 - Tesseract</summary>

[Task](https://cssbattle.dev/play/9)

    <p a><p b><p c>
    <style>
      * {
        margin: 0;
        position: absolute
      }
      body {
        background: #222730
      }
      p {
        background:#4CAAB3;
        height:150;
      }
      [a] {
        width: 400;
        top: 75;
      }
      [b] {
        width: 150;
        transform: rotate(45deg);
        margin: 75+125;box-shadow:0+0+0+50px#222730;
      }
      [c] {
        height:50;
        width:50;
        background:#393E46;
        border-radius:50%;
        margin:125+175;
      }
    </style>

</details>

<details>
  <summary>#10 - Cloaked Spirits</summary>

[Task](https://cssbattle.dev/play/10)

    <p a><i></i></p><p b><i></i></p><p a><i></i></p>
    <style>
      body {
        margin: 0 50;
        background: #62306D
      }
      p {
        display: inline-block;
        width: 100;
        height: 100;
        background: #F7EC7D;
      }
      i {
        display: block;
        width: 60;
        height: 60;
        background: #E38F66;
        border: solid 20px #AA445F;
        border-radius: 50%;
        margin-top: -50
      }
      [a]{
        margin-top: 200
      }
      [b]{
        height: 200
      }
      [b] > i {
        background: #AA445F;
        border: solid 20px #E38F66;
      }
    </style>

</details>

<details>
  <summary>#11 - Eye of Sauron</summary>

[Task](https://cssbattle.dev/play/11)

    <div id="l"></div><div id="c"></div><div id="r"></div>
    <style>
      body {
        background: #191210;
        position: relative;
        margin: 0
      }
      div {
        position: absolute;
      }
      #c {
        top: 100;
        left: 150;
        width: 50;
        height: 50;
        background: #84271C;
        border-radius: 50%;
        border: solid #191210 25px;
        box-shadow: 0px 0px 0px 20px #ECA03D;
      }
      #l, #r {
        width: 60;
        height: 30;
        border-radius: 50px 50px 0 0;
        border: solid #ECA03D 20px;
        border-bottom: 0;
      }
      #l {
        top: 150;
        transform: rotate(180deg);
        left: 50;
      }
      #r {
        top: 100;
        left: 250;
      }
    </style>

</details>

<details>
  <summary>#12 - Wiggly Moustache</summary>

[Task](https://cssbattle.dev/play/12)

    <div id="l"></div>
    <div id="c"></div>
    <div id="r"></div>
    <style>
      *{
        background: #F5D6B4;
        position: fixed;
      }
      #l, #r, #c{
        width: 60px;
        height: 30px;
        border: 20px solid #D86F45;
      }
      #l, #r{
        border-radius: 0 0 50px 50px;
        border-top: 0;
      }
      #l{
        margin: 142px 0 0 62px;
      }
      #r{
        margin: 142px 0 0 222px;
      }
      #c{
        margin: 92px 0 0 142px;
        border-radius: 50px 50px 0 0;
        border-bottom: 0;
      }
      #l:before, #r:after{
        content: "";
        width: 20px;
        height: 10px;
        position: absolute;
        background: #D86F45;
        border-radius: 20px 20px 0 0;
        top: -10px;
      }
      #l:before{
        left: -20px;
      }
      #r:after{
        left: 60px;
      }
    </style>

</details>
