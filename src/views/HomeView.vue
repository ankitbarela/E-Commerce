<template>
  <div class="home">
    <slider-component/>
  </div>
</template>

<script>
// .. imports removed for brevity
import SliderComponent  from '../components/SliderComponent.vue'

export default {
  name: "HomeView",
  components :{
    SliderComponent
  },
  methods: {
    // Log the user in
    login() {
      this.$auth.loginWithRedirect();
    },
    // Log the user out
    logout() {
      this.$auth.logout({
        returnTo: window.location.origin
      });
    }
  }
};
</script>