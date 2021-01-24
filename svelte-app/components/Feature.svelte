<script>
  const devIcon = "images/dev-icon.svg";
  const desSystemIcon = "images/des-system-icon.svg";
  const desIcon = "images/des-icon.svg";
  const ribbon = "images/feature-ribbon.svg";
</script>

<section class="relative mt-32">
  <div class="ribbon" style="background-image: url('{ribbon}');" />
  <div class="reverse-ribbon" style="background-image: url('{ribbon}');" />
  <div class="section-parent relative mx-auto grid grid-cols-3 pt-24">
    <section class="section mx-auto">
      <div
        class="feature-deco mx-auto"
        style="background-image: url('{devIcon}');"
      />
      <h2 class="text-2xl mt-14 text-center">Develop</h2>
      <p class="mt-8 tracking-wider leading-7 text-gray-400 text-justify">
        本業ではNuxt.jsを用いた開発をメインに。前職ではCMS開発を行っていました。その他にもGatsbyやNext.jsなど幅広く触っています。
      </p>
    </section>
    <section class="section mx-auto">
      <div
        class="feature-deco mx-auto"
        style="background-image: url('{desSystemIcon}');"
      />
      <h2 class="text-2xl mt-14 text-center">Design System</h2>
      <p class="mt-8 tracking-wider leading-7 text-gray-400 text-justify">
        既存プロジェクトに則りコーディング・構築。Atomic
        Design、アクセシビリティやSEOにも気を使ったコーディングを。
      </p>
    </section>
    <section class="section mx-auto">
      <div
        class="feature-deco mx-auto"
        style="background-image: url('{desIcon}');"
      />
      <h2 class="text-2xl mt-14 mb-8 text-center">Design</h2>
      <p class="mt-8 tracking-wider leading-7 text-gray-400 text-justify">
        UIデザインでプロダクトの問題を解決。本業ではウェブアプリケーションのUIデザイン、LPサイトの作成を担当しています。
      </p>
    </section>
  </div>
</section>

<style lang="scss">
  h2 {
    font-family: Inter;
    font-weight: 900;
    font-style: italic;
  }

  section {
    background: rgba(255, 251, 245, 0.5);
  }
  .section-parent {
    max-width: 1100px;
    min-height: 450px;

    &::before,
    &::after {
      position: absolute;
      content: "";
      width: 100px;
      height: 100px;
      background: rgba(255, 200, 135, 0.2);
      border-radius: 50%;
    }

    &::before {
      left: 10px;
      top: -50px;
    }
    &::after {
      left: 60px;
      top: -20px;
    }
  }

  .ribbon {
    position: absolute;
    display: block;
    width: 609px;
    height: 180px;
    background-repeat: no-repeat;
    bottom: -90px;
    left: 0;
  }

  .reverse-ribbon {
    position: absolute;
    display: block;
    width: 609px;
    height: 180px;
    background-repeat: no-repeat;
    top: -90px;
    right: 0;
    transform: rotate(180deg);
  }

  .section {
    max-width: 300px;
  }

  .feature-deco {
    width: 70px;
    height: 70px;
    border-radius: 50%;
    background-color: #fff;
    box-shadow: 0px 4px 4px 0px rgba(46, 217, 255, 0.25);
    background-repeat: no-repeat;
    background-position: center center;
  }
</style>
