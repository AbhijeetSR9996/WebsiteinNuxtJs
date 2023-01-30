<template>
  <div class="container">
    <main>
    <Header/>
      <h1>About Us</h1>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Facilis pariatur cupiditate, provident accusantium atque repudiandae facere quis non quas ducimus incidunt autem amet, eaque ratione? Consectetur laborum cupiditate, nam pariatur obcaecati quas quos odio at perferendis sunt amet vitae fugit quo earum tempora dolorem blanditiis soluta illo! Provident, inventore est.</p>
    </main>
  </div>
</template>

<script>
import Header from '../components/Header.vue'
export default {
  components: {
    Header
  },
  head() {
    return {
      title: "About Us"
    }
  }
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