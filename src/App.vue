<script>
import NavbarView from './components/Navigation/NavbarView.vue';

export default {
  components: {
    NavbarView
  }
}
</script>

<template>
  <header>
    <NavbarView/>
  </header>
  <RouterView/>
</template>


