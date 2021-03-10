<template>
  <div>
    <navbar />
    <b-container>
      <top />
    </b-container>
    <info/>
    <education />
    <skills />
    <contact />
    <FooterCustom />
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import Top from '~/components/Top.vue'
import Info from '~/components/Info.vue'
import Education from '~/components/Education.vue'
import FooterCustom from '~/components/Footer'

// import vueSmoothScroll from 'vue2-smooth-scroll'
// Vue.use(vueSmoothScroll)

export default {
  components: { Top, Navbar, Info, FooterCustom },

  data() {
    return{
      title: 'Andri Nur Hidayatulloh'
    }
  },

  head() {
    return {
      title: this.title
    }
  }
}

</script>

<style>

</style>
