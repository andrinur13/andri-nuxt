<template>
  <div class="topBar">
    <div class="row d-flex justify-content-center p-4">
      <div class="col-lg-6">
        <h3>{{name}}</h3>
        <br />
        <span
          >{{descInfo}}</span
        >
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
      skills: [
        {
          id: 1,
          skill: 'Go Lang',
        },
        {
          id: 2,
          skill: 'Express JS',
        },
        {
          id: 3,
          skill: 'Laravel PHP',
        },
      ],
      name: "Andri Nur Hidayatulloh",
      descInfo : "Hello my name is Andri Nur Hidayatulloh, I am a Back End Developers. But I'am interested about technology in Front End Developers"
    }
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400&display=swap');

.topBar {
  font-family: 'Roboto', sans-serif;
}

.topBar {
  margin-top: 50px;
}
</style>
