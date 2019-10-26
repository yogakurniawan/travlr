<template>
  <header id="header" class="header">
    <div class="header__desktop full-width">
      <div class="container">
        <div class="header__logo">
          <a href="https://www.travlr.com/">
            <img src="https://www.travlr.com/assets/images/logo-dark.svg" />
          </a>
        </div>
        <div class="header__menu">
          <div class="header__menu-nav">
            <ul>
              <li>
                <a href="/inspiration">Inspire Me</a>
              </li>
              <li>
                <a href="/my/shortlist">Plan My Trip</a>
              </li>
              <li>
                <a href="/deals-and-offers">Book My Trip</a>
              </li>
              <li>
                <a href="/deals-and-offers">Deals</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="header__shortcut">
          <div class="header__search">
            <span class="header__search-icon">
              <search-icon></search-icon>
            </span>
            <input class="header__search-input" name="search" type="text" placeholder="Search..." />
          </div>
          <div class="header__auth">
            <a
              href="https://www.travlr.com/login?redirect=https%3A%2F%2Fwww.travlr.com%2Fdeals-and-offers%2Fdetails%2F40-off-at-balis-newest-and-hottest-beach-club-tropicola-beach-club-7%3F"
              class="header__login-link"
            >Login</a>
            <a
              href="https://www.travlr.com/login?redirect=https%3A%2F%2Fwww.travlr.com%2Fdeals-and-offers%2Fdetails%2F40-off-at-balis-newest-and-hottest-beach-club-tropicola-beach-club-7%3F"
              class="header__signup-link"
            >Sign Up</a>
          </div>
        </div>
      </div>
    </div>
    <div class="header__mobile full-width"></div>
  </header>
</template>

<script>
import SearchIcon from "./search-icon.vue";

export default {
  components: {
    SearchIcon
  }
};
</script>

<style lang="scss" scoped>
.header {
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 1002;
  box-shadow: 0 1px 3px 0 rgba(27, 27, 27, 0.1),
    0 4px 8px 0 rgba(27, 27, 27, 0.1);
  background: #fff;
  border-bottom: 1px solid #ddd;
  justify-content: space-between;
  align-items: center;
  display: flex;
  flex-wrap: wrap;
}

.header__logo {
  width: 150px;
  padding: 8px 0;
}

.header__shortcut {
  display: flex;
  flex-wrap: wrap;
  justify-content: flex-end;
  align-items: center;
  height: 63px;
}

.header__auth {
  display: flex;
  align-items: center;
  padding-right: 15px;
}

.header__login-link {
  font-size: 13px;
  font-weight: 500;
  color: #333;
  margin-right: 15px;
  text-transform: capitalize;
  display: block;
  padding: 9px 13px;
}

.header__signup-link {
  font-size: 13px;
  font-weight: 500;
  color: #fff;
  text-transform: uppercase;
  display: block;
  background-color: #006272;
  padding: 9px 13px;
  border-radius: 3px;
}

.header__search {
  width: 220px;
  display: flex;
  align-items: center;
  height: 63px;
  position: relative;
}

.header__search-icon {
  position: absolute;
  top: 21px;
  left: 8px;
  z-index: 999999999;
}

.header__search-input {
  height: auto;
  transition: all 0.5s ease;
  float: right;
  border: 1px solid #ddd;
  background-color: #f5f5f5;
  box-shadow: none;
  padding: 7px 30px 7px 40px;
  border-radius: 4px;
  font-weight: 500;
  display: block;
  width: 200px;
  line-height: 1.42857143;
  color: #555;
  background-image: none;
  &:focus {
    border-color: #66afe9;
    outline: 0;
    -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075),
      0 0 8px rgba(102, 175, 233, 0.6);
    box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075),
      0 0 8px rgba(102, 175, 233, 0.6);
  }
}

.header__menu {
  width: calc(100% - 570px);
  padding-left: 32px;
  padding-right: 28px;
}

.header__menu-nav {
  flex: 1;
  ul {
    display: flex;
    align-items: center;
  }
  li {
    position: relative;
  }
  a {
    text-transform: capitalize;
    font-size: 14px;
    font-weight: 500;
    color: #333;
    padding: 23px 20px 22px;
    display: block;
    transition: all 0.5s ease;
    position: relative;
  }
}

.container {
  display: flex;
  flex-wrap: wrap;
  position: relative;
  width: 1170px;
  max-width: 100%;
  margin: auto;
}

.full-width {
  width: 100%;
}

.header__desktop {
  @media screen and (max-width: 1106px) {
    display: none;
  }
}

.header__mobile {
  @media screen and (max-width: 1106px) {
    display: block;
  }
}
</style>