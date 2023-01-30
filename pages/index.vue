<template>
  <div class="container">
    <Header />
    <main>
      <h1>This is a website made using Nuxtjs!!</h1>
      <p>
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ea doloribus
        iusto alias eveniet officia ab recusandae, accusantium provident, rem
        dignissimos quasi atque illum consequuntur illo? Aut excepturi
        perspiciatis consequatur dolorum.
      </p>
    </main>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
export default {
  components: {
    Header,
  },
  head() {
    return {
      title: "Nuxt Website",
    };
  },
  mounted () {
    this.$nextTick(() => {
      this.$nuxt.$loading.start()

      setTimeout(() => this.$nuxt.$loading.finish(), 500)
    })
  }
};
</script>

<style lang="scss">
html {
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  font-size: 16px;

  &,
  body {
    width: 100%;
    height: 100vh;
    margin: 0;
    padding: 0;
  }
}

.container {
  width: 100%;
  margin: 0 auto;
  height: auto;

  main {
    width: 100%;
    height: auto;
    display: flex;
    flex-direction: column;
    align-items: center;

    h1 {
      font-size: 3em;
    }
    p {
      text-indent: 3em;
      font-size: 1.25em;
      line-height: 1.5;
      margin-top: 0;
      width: 80%;
    }
  }
  .page-enter-active {
    animation: bounce-in .8s;
}

.page-leave-active {
    animation: bounce-out .5s;
}

@keyframes bounce-in {
    0% {
        transform: scale(0);
    }
    50% {
        transform: scale(1.1);
    }
    100% {
        transform: scale(1);
    }
}

@keyframes bounce-out {
    0% {
        transform: scale(1);
    }
    50% {
        transform: scale(1.1);
    }
    100% {
        transform: scale(0);
    }
}
}
</style>



