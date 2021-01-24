<script>
  const figma = "images/figma-icon.svg";
  const tailwind = "images/tailwindcss-icon.svg";
  const gatsby = "images/gatsby-icon.svg";
  const nuxt = "images/nuxt-icon.svg";
  const skillsPerson = "images/skills-person.svg";
  const decoGreen = "images/deco-green.svg";
</script>

<section class="section-parent relative mt-64 grid grid-cols-2 justify-center">
  <div class="left-text ml-auto mr-8 relative">
    <img class="absolute -left-20 -top-12" src={decoGreen} alt="" />
    <h2 class="relative font-bold text-4xl text-center">Skills</h2>
    <div class="grid grid-cols-4 mt-16">
      <img src={figma} alt="" />
      <img src={tailwind} alt="" />
      <img src={nuxt} alt="" />
      <img src={gatsby} alt="" />
    </div>
    <p class="tracking-wider leading-7 text-gray-400 mt-12 text-justify">
      よく使う4つのツール、フロントエンド開発が主です。コーディングはぜひともお任せください。どんなことでもお気軽にご相談を。
    </p>
  </div>
  <div class="right-content mx-auto">
    <img class="relative" src={skillsPerson} alt="" />
  </div>
</section>

<style lang="scss">
  h2 {
    font-family: Inter;
    font-weight: 900;
    font-style: italic;
  }

  .section-parent {
    &::before {
      content: "";
      position: absolute;
      height: 350px;
      width: 70%;
      top: 5%;
      background: linear-gradient(
        270deg,
        rgba(255, 232, 206, 1) 0,
        rgba(136, 113, 87, 0) 100%
      );
      opacity: 0.5;
    }

    &::after {
      content: "";
      position: absolute;
      z-index: -1;
      width: 30%;
      height: 380px;
      background: rgba(255, 200, 135, 0.4);
      display: block;
      top: -10%;
      right: 0;
    }
  }
  .left-text {
    max-width: 400px;
  }
  .right-content {
    &::before {
      content: "";
      position: absolute;
      bottom: 10%;
      left: 55%;
      width: 125px;
      height: 125px;
      background: rgba(255, 200, 135, 0.1);
    }
  }
</style>
