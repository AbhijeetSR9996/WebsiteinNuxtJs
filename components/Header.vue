<template>
     <header>
      <h3 class="logo">Nuxt Website</h3>
      <ul>
        <li><nuxt-link to="/">Home</nuxt-link></li>
        <li><nuxt-link to="/about">About</nuxt-link></li>
        <li><nuxt-link to="/contact">Contact</nuxt-link></li>
        <li><nuxt-link to='/donate'>Donate</nuxt-link></li>
      </ul>
    </header>
</template>

<style lang="scss" scoped>
header {
  background: lightskyblue;
  color: #e8eef2;
  width: calc(100% - 14em);
  padding: 0 7em;
  height: 8em;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;

  h3.logo {
    font-size: 3em;
    font-weight: 300;
  }

  ul {
    padding: 0;
    margin: 0;
    list-style: none;
    display: flex;
    flex-direction: row;

    li {

      &, a {
        padding: 1em .5em;
      }
      a {
        color: inherit;
        text-decoration: none;
      }
    }
  }
}
</style>