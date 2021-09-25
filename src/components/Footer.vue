<template>
  <footer>
    <Logo />
    <a
      href="https://github.com/ohminkwon/"
      target="_blank">
      (c){{ new Date().getFullYear() }} This site was built by OHMIN KWON
    </a>
  </footer>
</template>

<script>
import Logo from '~/components/Logo'

export default {
  components: {
    Logo
  },
  computed: {
    name() {
      return this.$store.state.about.name
    }
  }
}
</script>

<style lang="scss" scoped>
footer {
  padding: 70px 0;
  text-align: center;
  opacity: .3;
  .logo {
    display: block;
    margin-bottom: 10px;
  }
  a{
    color: $gray-600;
    text-decoration: none;
    cursor: pointer; 
  }
}
</style>
