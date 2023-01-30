<template>
  <div class="container">
    <main>
      <Header />
      <h1>Donate to us!!</h1>
      <p>
        Lorem ipsum dolor sit, amet consectetur adipisicing elit. Repellendus,
        at tempora accusantium sequi laboriosam adipisci eos nihil ratione atque
        labore modi fugit asperiores aliquam architecto veritatis possimus
        minima impedit sint in alias cupiditate reprehenderit? Eaque vel non
        deserunt eveniet sed maxime aspernatur nobis, repellat natus! Sit
        incidunt minus optio omnis!
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
      title: "Donate to Us!!",
    };
  },
};
</script>
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
