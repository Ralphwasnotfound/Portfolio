<template>
  <header>
    <NavbarView/>
  </header>
  <RouterView/>
</template>

<script>
import NavbarView from './components/Navigation/NavbarView.vue';

export default {
  components: {
    NavbarView
  }
}
</script>

