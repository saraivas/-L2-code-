<template lang="">
  <div class="all-header">
    <div class="center-text">
      <p class="top-text">NON FUNGIBLE TOKENS</p>
      <div class="frame">
        <div class="line1">
          A new NFT <img src="../assets/icons/VectorGreen.png" alt="" />
        </div>
        <div class="line2">
          <img src="../assets/icons/redBlue.png" alt="" />Experience
        </div>
      </div>
      <p class="bottom-text">Discover, collect and sell</p>
    </div>
    <div class="logotypes">
      <img class="logo" src="../assets/icons/RS.png" alt="" />
      <img class="logo" src="../assets/icons/nike.png" alt="" />
      <img class="logo" src="../assets/icons/adidas.png" alt="" />
      <img class="logo" src="../assets/icons/nh.png" alt="" />
    </div>
  </div>
</template>
<script>
export default {
  name: "HeaderPage",
  components: {},
};
</script>
<style lang="less" scoped>
.all-header {
  height: calc(100vh - 150px);
  margin: 0px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 180px;
  position: relative;

  position: relative;
  .center-text {
    .top-text {
      height: 18px;
      font-family: "Inter", sans-serif;
      font-style: normal;
      font-weight: 500;
      font-size: 15px;
      line-height: 18px;
      text-align: center;
      letter-spacing: 3px;
      text-transform: uppercase;
      color: #7780a1;
      text-align: center;
    }

    .frame {
      width: 837px;
      font-weight: 600;
      font-size: 120px;
      line-height: 100%;
      text-align: center;
      letter-spacing: 0.2px;
      color: #ffffff;
      padding: 34px 0;
      width: 837px;

      .line1 {
        margin-right: 90px;
        img {
          margin-left: 10px;
        }
      }
      .line2 {
        margin-left: 90px;
        img {
          margin-right: 20px;
        }
      }
      .line1,
      .line2 {
        display: flex;
        justify-content: center;
        align-items: center;
      }
    }
    .bottom-text {
      height: 36px;
      left: calc(50% - 285px / 2);
      top: calc(50% - 36px / 2 + 160.5px);
      font-family: "Inter", sans-serif;
      font-style: normal;
      font-weight: 400;
      font-size: 24px;
      line-height: 150%;
      letter-spacing: 0.2px;
      color: #7780a1;
      text-align: center;
    }
  }

  .logotypes {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: flex-start;
    width: 670px;
    height: 45px;
  }
}
</style>
