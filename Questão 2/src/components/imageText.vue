<template lang="">
  <div class="containner">
    <div class="text">
      <p class="first-text">overline</p>
      <div class="big-text">Sapien ipsum scelerisque convallis fusce</div>
      <p class="last-text">
        Ut amet vulputate faucibus vitae semper eget auctor. Diam tempor
        pulvinar ultricies dolor feugiat aliquam commodo.
      </p>
      <div class="buttons">
        <button class="blue-button">Get started</button>
        <button class="transparen-button">Learn more</button>
      </div>
    </div>
    <div class="images">
      <img class="img2" src="../assets/images/tinta1.png" alt="" />
      <img class="img1" src="../assets/images/tinta.png" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "imageText",
  props: {
    msg: String,
  },
};
</script>
<style lang="less" scoped>
.containner {
  width: 1392px;
  height: 616px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 126px;

  .text {
    display: flex;
    flex-direction: column;
    text-align: left;
    width: 590px;
    height: 406px;
    p {
      margin: 0;
    }

    .first-text {
      font-family: "Inter", sans-serif;
      text-align: left;
      font-weight: 500;
      font-size: 15px;
      line-height: 18px;
      letter-spacing: 3px;
      text-transform: uppercase;
      color: #7780a1;
      margin-bottom: 16px;
    }

    .big-text {
      width: 590px;
      height: 192px;
      font-family: "Sora", sans-serif;
      font-style: normal;
      font-weight: 600;
      font-size: 64px;
      line-height: 100%;
      letter-spacing: 0.2px;
      color: #ffffff;
      text-align: left;
      margin-bottom: 32px;
    }
    .last-text {
      font-family: "Inter", sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: 16px;
      line-height: 150%;
      letter-spacing: 0.2px;
      color: #7780a1;
      text-align: left;
      margin-bottom: 48px;
    }
    .blue-button {
      padding: 16px 24px;

      border-radius: 12px;
      background: linear-gradient(104.42deg, #4745d0 0%, #2a27c9 60.23%);
      box-shadow: inset -4px -4px 4px rgba(0, 0, 0, 0.1),
        inset 4px 4px 4px rgba(255, 255, 255, 0.1);
      border: #7780a1;

      font-weight: 600;
      font-size: 16px;
      line-height: 20px;
      text-align: center;
      letter-spacing: 0.2px;
      color: #ffffff;

      margin-right: 16px;
    }
    .transparen-button {
      padding: 16px 24px;

      border: 2px solid #7780a196;
      border-radius: 12px;

      font-weight: 600;
      font-size: 16px;
      line-height: 20px;
      text-align: center;
      letter-spacing: 0.2px;
      color: #7780a1;
    }
  }
  .images {
    position: relative;
    width: 684px;
    height: 616px;
    margin-left: 118px;
    .img1 {
      position: absolute;
      width: 386px;
      height: 386px;
      left: calc(50% - 386px / 2 - 133px);
      top: calc(50% - 386px / 2 + 99px);
      background: rgba(255, 0, 0, 0);
    }

    .img2 {
      position: absolute;
      width: 430px;
      height: 430px;
      left: calc(50% - 430px / 2 + 111px);
      top: calc(50% - 430px / 2 - 77px);
      background: rgba(255, 0, 0, 0);
    }
  }
}
</style>
