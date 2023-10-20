<template>
  <div>
    <Banner />
    <div class="main-container">
      <h1>Monte o seu burger</h1>
      <BurgerForm />
    </div>
  </div>
</template>

<script>
import Banner from "../components/banner/Banner.vue";
import BurgerForm from "../components/form/BurgerForm.vue";

export default {
  name: "Home",
  components: {
    Banner,
    BurgerForm,
  },
};
</script>
