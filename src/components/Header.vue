<template>
  <div class="content--bg">
    <div class="content--overlay">
      <header class="header">
        <div class="header--brand">
          <h3>SAGARA</h3>
        </div>
        <nav class="header--nav">
          <ul class="header--nav_list">
            <li class="header--nav__item">
              <a href="#" class="header--nav__item-link">Login</a>
            </li>
          </ul>
        </nav>
      </header>
      <div class="container header--cover">
        <h1 class="head--cover_title">Get Your Account</h1>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Pariatur, fugiat.</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.content {
  &--bg {
    background: url("https://placeimg.com/1000/800/tech") center;
    background-size: cover;
    background-position: center;
    color: #fff;
  }
  &--overlay {
    background: linear-gradient(260deg, #84504982, #873425db);
    min-height: 50vh;
    position: relative;
  }
}
.header {
  padding: 0.5rem 4rem;
  display: flex;
  align-items: center;
  margin-bottom: 2rem;
  &--nav {
    text-align: right;
    width: 100%;
    &_list {
      list-style: none;
      padding: 0;
    }
    &__item {
      margin-top: 1rem;
      display: block;
      &-link {
        color: #fff;
        font-weight: bold;
      }
    }
  }
  &--cover {
    margin: 3rem 0;
  }
}

@media (max-width: 900px) {
  .header {
    padding: 0 2rem;
  }
  .content {
    &--overlay {
      min-height: auto;
      padding: 2rem 0;
    }
  }
}
</style>