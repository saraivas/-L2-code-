<template lang="">
  <div class="all-footer">
    <div class="left">
      <img class="logo" src="../assets/icons/LogoWhite.png" alt="Logo" />
      <div class="small-menu">
        <a href="">Support</a>
        <a href="">Term of service</a>
        <a href="">License</a>
      </div>
    </div>

    <div class="mid">
      <div class="menu">
        <a href="">Auctions</a>
        <a href="">Roadmap</a>
        <a href="">Discover</a>
        <a href="">Community</a>
      </div>
      <button class="blue-button">My account</button>
      <div class="social-media">
        <img
          clas="social-icons"
          src="../assets/icons/face.png"
          alt="Facebook"
        />
        <img
          clas="social-icons"
          src="../assets/icons/link.png"
          alt="LinkedIn"
        />
        <img clas="social-icons" src="../assets/icons/git.png" alt="Git" />
        <img clas="social-icons" src="../assets/icons/tw.png" alt="Twitter" />
        <img
          clas="social-icons"
          src="../assets/icons/insta.png"
          alt="Instagram"
        />
      </div>
    </div>

    <div class="right">
      <div class="text">
        <p>
          Auctions Nibh volutpat, aliquam id sagittis elementum. Pellentesque
          laoreet velit, sed egestas in. Id nam semper dolor tellus vulputate
          eget turpis.
        </p>
      </div>

      <div class="input-area">
        <input type="text" placeholder="Newsletter"/>
        <button href="">Sign in</button>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "footerPage",
  props: {
    msg: String,
  },
};
</script>
<style lang="less" scoped>
.all-footer {
  flex-direction: row;
  width: 1392px;
  display: flex;
  height: 397px;
  margin-bottom: 120px;
  box-sizing: border-box;

  .left {
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 48px;
    border: 1px solid #7780a196;
    border-radius: 20px 0px 0px 20px;

    .logo {
      width: 213px;
      height: 34px;
    }

    .small-menu {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      width: 294px;

      a {
        font-family: "Inter", sans-serif;
        font-weight: 400;
        color: #7780a1;
        font-size: 14px;
        color: #7780a1;
        text-decoration: none;
      }
    }
  }
  .mid {
    flex: 1;
    padding: 48px 0 40px 48px;
    border: 1px solid #7780a196;
    border-style: solid none;
    justify-content: space-between;
    .menu {
      display: flex;
      flex-direction: column;
      display: flex;
      gap: 16px;

      a {
        font-weight: 600;
        font-size: 16px;
        line-height: 20px;
        color: #ffffff;
        text-decoration: none;
      }
    }
    .blue-button {
      padding: 16px 24px;
      margin: 40px 0 69px 0;

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
    .social-media {
      display: flex;
      width: 200px;
      justify-content: space-between;

      .social-icons {
        width: 20px;
        height: 20px;

        &:hover {
          cursor: pointer;
        }
      }
    }
  }
  .right {
    flex: 1;
    padding: 48px;
    height: 100%;
    border: 1px solid #7780a196;
    border-radius: 0px 20px 20px 0px;
    display: flex;
    flex-direction: column;
    align-items: center;
    position: relative;

    .text {
      p {
        width: 367px;
        font-family: "Inter", sans-serif;
        text-align: left;
        font-style: normal;
        font-weight: 400;
        font-size: 14px;
        line-height: 150%;
        letter-spacing: 0.2px;
        color: #7780a1;
      }
    }
    .input-area {
      display: flex;
      justify-content: center;
      align-items: center;
      position: absolute;
      bottom: 40px;
      width: 367px;

      input {
        height: 52px;
        background: #ffffff;
        border-radius: 20px 0px 0px 20px;
        padding: 16px 0 16px 32px;
        appearance: unset;
        border: 0px;
        &::placeholder{
            color: #7780A1;
        }
      }
      button {
        height: 52px;
        background: #ffffff;
        padding: 16px 24px;
        border-radius: 0 20px 20px 0px;
        border: 0px ;
        color: #2a27c9;
        font-weight: 600;
        font-size: 16px;
        line-height: 20px;
        
        &:hover{
            cursor: pointer;
        }
      }
    }
  }
}
</style>
