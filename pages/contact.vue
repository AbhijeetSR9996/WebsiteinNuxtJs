<template>
  <div class="container">
    <main>
      <Header />
      <h1>Contact Us</h1>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis neque
        corrupti autem, odio quam beatae voluptatem esse ipsa nulla incidunt eos
        harum itaque debitis ducimus, nobis vero delectus! Quis, omnis nihil
        labore ullam iure quam nulla et possimus hic ratione!
      </p>
      <p></p>
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
      title: "Contact Us",
    };
  },
};
</script>
<style>
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
</style>
