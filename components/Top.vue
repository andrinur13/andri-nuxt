<template>
  <div class="topBar">
    <div class="row d-flex justify-content-center p-4">
      <div class="col-lg-6">
        <div class="custom-hello">Hello !</div>
        <div class="mt-2 name-style">{{ name }}</div>
        <br />
        <div class="bg-danger backend">Back End Developers</div>
        <br />
        <br />
        <span v-for="skill in skills" :key="skill.id">
          {{ skill.skill }} <br />
        </span>
      </div>

      <div class="col-lg-6">
        <div class="d-flex justify-content-center">
          <img src="/andri.png" alt="andri" width="70%" />
        </div>
      </div>
    </div>
    <hr />
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: 'Andri Nur Hidayatulloh',
      descInfo:
        "Hello my name is Andri Nur Hidayatulloh, I am a Back End Developers. But I'am interested about technology in Front End Developers",
    }
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Patrick+Hand&display=swap');

.topBar {
  font-family: 'Patrick Hand', 'Roboto', sans-serif;
  margin-top: 100px;
}

.custom-hello {
  background-color: #4edbc5ff;
  color: black;
  width: auto;
  display: inline-block;
  padding: 10px;
  border-radius: 5px;
  font-size: 15pt;
}

.backend {
  background-color: #dc3545;
  color: white;
  width: auto;
  display: inline-block;
  padding: 10px;
  border-radius: 5px;
  font-size: 20pt;
}

.name-style {
  font-size: 35pt;
}
</style>
