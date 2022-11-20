<template>
  <div class="header">
    <img class="logo" src="../assets/icons/LogoWhite.png" alt="logo" />
    <div class="Menu">
      <a href="">Auctions</a>
      <a href="">Roadmap</a>
      <a href="">Discover</a>
      <a href="">Community</a>
    </div>
    <div class="buttons-header">
      <button class="transparen-button">Contact</button>
      <button class="blue-button">My account</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "topBar",
  props: {
    msg: String,
  },
};
</script>

<style lang="less" scoped>
.header {
  display: flex;
  justify-content: space-between;
  height: 150px;
  align-items: center;
  padding: 48px;

  .logo {
    width: 213px;
    height: 34px;
  }
  .Menu {
    width: 523px;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: flex-start;
    padding: 0px;
    gap: 64px;

    a {
      color: #7780a1;
      font-weight: 600;
      font-size: 16px;
      line-height: 20px;
      display: flex;
      align-items: center;
      text-align: center;
      letter-spacing: 0.2px;
      text-decoration: none;
    }
  }

  .buttons-header {
    display: flex;
    flex-direction: row;
    justify-content: flex-end;
    align-items: center;
    padding: 0px;
    gap: 16px;
    width: 278px;
    height: 52px;

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
    }
  }
}
</style>
