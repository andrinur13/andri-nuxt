<template>
  <div>
    <navbar />
    <b-container>
      <top />
    </b-container>
    <info/>
    <education />
    <skills />
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import Top from '~/components/Top.vue'
import Info from '~/components/Info.vue'
import Education from '~/components/Education.vue'

export default {
  components: { Top, Navbar, Info },
}

<style>
/* .container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
} */
</style>
