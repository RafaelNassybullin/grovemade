<template>
  <div class="footer">
    <div class="footer-wrapper">
      <div @click="moveTop()" class="go-up"><p>go</p>
        <p>up</p></div>
      <div class="footer-items">
        <ul class="list">
          <li>Shop</li>
          <li>About</li>
          <li>Journal</li>
          <li>Support</li>
          <li>COVID-19 Info</li>
          <li>Order Status</li>
          <li>Corporate Sales</li>
        </ul>
        <div class="subscribe">
          <h3>Newsletter Signup</h3>
          <p>Sign up to our Newsletter to hear about new product releases, learn about our design process, and
            everything else going on behind the scenes at Grovemade.</p>
          <label for="sub">
            <input id="sub" type="text">
          </label>
        </div>
      </div>
    </div>
    <div class="privacy">
      <p>© 2020 Grovemade</p>
      <p>Terms & Conditions</p>
      <p>Privacy Policy</p>
      <p>Site by Department</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'footer',
  methods: {
    moveTop() {
      window.scroll({
        top: 0,
        left: 0,
        behavior: 'smooth'
      })
    }
  }
}
</script>

<style scoped lang="scss">
.footer {
  width: 100%;
  padding: 0 3.472vw;
  background: #F9F9F9;
  @media(max-width: 433px) {
    //background: #F9F9F9;
  }

  .footer-wrapper {
    width: 100%;
    height: 23.958vw;
    display: flex;
    align-items: flex-end;
    position: relative;
    @media(max-width: 433px) {
      height: 172.958vw;
      align-items: flex-start;

    }
  }

  .footer-items {
    display: flex;
    align-items: flex-end;
    @media(max-width: 433px) {
      align-items: flex-start;
      flex-direction: column;
    }
  }

  .list {
    list-style: none;
    font-size: 1.528vw;
    @media(max-width: 433px) {
      font-size: 6.528vw;
      margin-top: 7vw;
    }

    li {
      margin-bottom: 0.8vw;
      @media(max-width: 433px) {
        margin-bottom: 3.8vw;
      }
    }
  }

  .subscribe {
    width: 24.167vw;
    margin-bottom: 4.583vw;
    margin-left: 0.903vw;
    @media(max-width: 433px) {
      width: 89.167vw;
      margin-top: 6vw;
    }

    h3 {
      margin-bottom: 1.597vw;
      font-size: 1.597vw;
      font-weight: 400;
      @media(max-width: 433px) {
        margin-bottom: 5.597vw;
        font-size: 9.597vw;
      }
    }

    p {
      margin-bottom: 4.556vw;
      font-size: 0.972vw;
      color: #A0A0A0;
      @media(max-width: 433px) {
        font-size: 4.972vw;
      }
    }
  }

  input {
    width: 22.222vw;
    border: none;
    background: none;
    outline: none;
    border-bottom: 0.090vw solid black;
    font-size: 1.597vw;
    @media(max-width: 433px) {
      width: 80.222vw;
      border-bottom: 0.69vw solid black;
      font-size: 4.597vw;
    }
  }

  .go-up {
    width: 5.694vw;
    height: 5.694vw;
    background: black;
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    position: absolute;
    top: 0;
    right: 0;
    font-size: 1.597vw;
    font-weight: 300;
    text-transform: uppercase;
    cursor: pointer;
    @media(max-width: 433px) {
      width: 16.694vw;
      height: 16.694vw;
      font-size: 4.597vw;
    }
  }

  .privacy {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: flex-end;
    margin-top: 6.319vw;
    padding-bottom: 3vw;
    @media(max-width: 433px) {
      flex-direction: column;
    }

    p {
      color: gray;
      font-size: 1vw;
      margin: 0 1.319vw;
      @media(max-width: 433px) {
        font-size: 5vw;
        margin: 2.319vw;
      }
    }

    p:last-child {
      color: black;
      @media(max-width: 433px) {

      }
    }
  }
}
</style>