<script>
  const about = "images/about.svg";
</script>

<section id="about" class="grid grid-cols-2 items-center">
  <div class="mx-auto relative">
    <div class="circle-1 absolute -left-24" />
    <img class="relative" src={about} alt="" />
  </div>
  <div class="content-right ml-8 mr-auto">
    <h2 class="font-bold text-4xl text-center">About me</h2>
    <p class="tracking-wider mt-16 leading-7 text-gray-400 text-justify">
      閲覧ありがとうございます。まさると申します。
      JavaScriptやCSS、デザインを作るのが大好きです。
      業務では円滑なコミュニケーションを意識しつつ、快適にお仕事を進められるようお手伝いいたします。
    </p>
    <div class="circle-2 absolute right-0" />
  </div>
</section>

<style lang="scss">
  h2 {
    font-family: Inter;
    font-weight: 900;
    font-style: italic;
  }

  .content-right {
    width: 400px;
  }

  .circle-1 {
    width: 300px;
    height: 300px;
    border: 20px solid rgba(255, 232, 206, 0.5);
    border-radius: 50%;
  }
  .circle-2 {
    width: 400px;
    height: 400px;
    border: 20px solid rgba(255, 232, 206, 0.23);
    border-radius: 50%;
  }
</style>
