<script>
  const mainPerson = "images/mv-circle.svg";
  const mainLine = "images/main-line.svg";
  const decoOrange = "images/deco-orange.svg";
  const decoGreen = "images/deco-green.svg";
</script>

<section class="grid items-center justify-center grid-cols-2">
  <div class="left-content mx-auto">
    <div class="relative">
      <img class="absolute -top-12 -left-12" src={decoOrange} alt="" />
      <h2 class="relative title mx-auto text-4xl">From Design to Coding</h2>
    </div>
    <p
      class="text tracking-wider text-justify mx-auto mt-6 leading-7 text-gray-400"
    >
      デザインからフロントエンド開発まで全てお任せください。画面設計はぜひご相談を。ReactやVueなどのライブラリ、CMS開発まで幅広く対応いたします。
    </p>
  </div>
  <div class="right-content">
    <div class="relative">
      <img class="negative-z absolute right-1/3" src={decoGreen} alt="" />
      <img src={mainPerson} alt="" />
      <img class="absolute -bottom-10 right-1/2" src={decoGreen} alt="" />
    </div>
  </div>
  <div class="line negative-z absolute left-0 top-80">
    <img class="w-full" src={mainLine} alt="" />
  </div>
</section>

<style lang="scss">
  h2 {
    font-family: Inter;
    font-weight: 900;
    font-style: italic;
  }

  .deco {
    background-repeat: no-repeat;
  }

  .negative-z {
    z-index: -1;
  }

  .left-content {
    width: 405px;
  }
  .title {
    width: 405px;
  }
  .text {
    width: 405px;
  }
  .line {
    width: 100vw;

    img {
      max-width: 100vw;
    }
  }
</style>
