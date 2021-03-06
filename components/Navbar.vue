<template>
  <div>
    <b-navbar toggleable="lg" type="light" variant="light">
      <b-container>
        <b-navbar-brand> <nuxt-link to="/" class="linkNuxt">Andri</nuxt-link> </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-navbar-nav>
              <b-nav-item> <nuxt-link to="/home" class="linkNuxt">About</nuxt-link> </b-nav-item>
              <b-nav-item> <nuxt-link to="/home" class="linkNuxt">Education</nuxt-link> </b-nav-item>
              <b-nav-item> <nuxt-link to="/home" class="linkNuxt">Skills</nuxt-link> </b-nav-item>
              <b-nav-item> <nuxt-link to="/home" class="linkNuxt">"Karya Saya"</nuxt-link> </b-nav-item>
              <b-nav-item> <nuxt-link to="/home" class="linkNuxt">Contact</nuxt-link> </b-nav-item>
            </b-navbar-nav>
          </b-navbar-nav>
        </b-collapse>
      </b-container>
    </b-navbar>
  </div>
</template>

<script>
export default {}
</script>

<style>

    .linkNuxt {
        color: black;
    }

    .linkNuxt:hover {
        color: "027bfeff";
        text-decoration: none;
    }

</style>
