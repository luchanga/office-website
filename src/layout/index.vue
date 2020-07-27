<template>
  <div class="app-wrapper">
    <app-header/>
    <router-view></router-view>
    <app-footer/>
  </div>
</template>

<script>
import Header from './components/Header';
import Footer from './components/Footer';
export default {
  name: 'Layout',
  components: {
    'app-header': Header,
    'app-footer': Footer
  },
  mixins: [],
  computed: {
  },
  methods: {
  }
}
</script>

<style lang="scss" scoped>
</style>
