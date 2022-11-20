<template lang="">
  <div class="icons">
    <div class="square-icons">
      <div class="icon"><img src="../assets/icons/user.png" alt="" /></div>
      <h2>300k</h2>
      <p>Users Active</p>
    </div>
    <div class="square-icons">
      <div class="icon"><img src="../assets/icons/Group.png" alt="" /></div>
      <h2>52,5k</h2>
      <p>Artworks</p>
    </div>
    <div class="square-icons">
      <div class="icon"><img src="../assets/icons/Artist.png" alt="" /></div>
      <h2>17,5k</h2>
      <p>Artists</p>
    </div>
    <div class="square-icons">
      <div class="icon"><img src="../assets/icons/Wallet.png" alt="" /></div>
      <h2>35.58</h2>
      <p>ETH Spent</p>
    </div>
  </div>
</template>
<script>
export default {
  name: "sectionIcons",
  props: {
    msg: String,
  },
};
</script>
<style lang="less" scoped>
.icons {
  width: 920px;
  height: 135px;
    
  margin-bottom: 200px;

  display: flex;
  justify-content: center;
  align-items: center;

  .square-icons {
    flex: 1;

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    

    h2 {
      margin-top: 16px;
      font-weight: 600;
      font-size: 48px;
      line-height: 115%;
      color: white;
    }

    p {
      margin: 0;
      font-family: "Inter", sans-serif;
      font-weight: 400;
      font-size: 16px;
      line-height: 150%;

      text-align: center;
      letter-spacing: 0.2px;

      /* On White/Grey 100 */

      color: #7780a1;
    }
  }
}
</style>
