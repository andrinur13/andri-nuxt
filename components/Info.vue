<template>
  <b-container class="info-container" id="about" v-smooth-scroll>
    <div class="row d-flex justify-content-center p-4">
      <div class="col-lg-4 justify-content-center">
        <img :src="img" alt="andri" width="70%" />
      </div>

      <div class="col-lg-4">
        <div>
          <h3>About Me</h3>
          <p class="mt-4">{{ desc }}</p>
          <div class="skill-path">
            <span class="skill m-1" v-for="skill in skills" :key="skill.id">
              {{ skill }}
            </span>
          </div>
        </div>
      </div>
    </div>
  </b-container>
</template>

<script>
export default {
  data() {
    return {
      desc:
        "Hello, I’m a Andri, Back End Developers based on Yogyakarta Indonesia. I have rich experience in make RESTFUL API and I'm also interested about Front End technlogy",

      skills: ['Go Lang', 'Express JS', 'Laravel', 'Node JS', 'Docker'],
      img: 'info.png',
    }
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Patrick+Hand&display=swap');

.info-container {
  padding-top: 100px;
  font-family: 'Patrick Hand', 'Roboto', sans-serif;
}

.img-info {
  height: 30%;
}

.skill {
  background: #4edbc5ff;
  width: auto;
  display: inline-block;
  padding: 3px;
  border-radius: 5px;
}
</style>
