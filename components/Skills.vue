<template>
  <b-container class="skills" id="skills">
    <h1 class="text-center text-skills">Skills</h1>
    <div class="row justify-content-center row-skills">
      <div class="col-lg-5">
        <h3 class="text-center">Technical Skills</h3>

        <b-progress
          :max="max"
          height="2rem"
          v-for="skill in skills"
          :key="skill.id"
          class="mt-4"
        >
          <b-progress-bar :value="skill.value">
            <span class="text-inner-bar"
              >{{ skill.skills }}:
              <strong>{{ skill.value.toFixed(2) }} / {{ max }}</strong></span
            >
          </b-progress-bar>
        </b-progress>
      </div>
      <div class="col-lg-5">
        <h3 class="text-center">Personal Skills</h3>

        <b-progress
          :max="max"
          height="2rem"
          v-for="skill in personalSkills"
          :key="skill.id"
          class="mt-4"
          variant="success"
        >
          <b-progress-bar :value="skill.value">
            <span class="text-inner-bar"
              >{{ skill.skills }}:
              <strong>{{ skill.value.toFixed(2) }} / {{ max }}</strong></span
            >
          </b-progress-bar>
        </b-progress>
      </div>
    </div>
  </b-container>
</template>

<script>
export default {
  data() {
    return {
      value: 75,
      max: 100,

      skills: [
        { skills: 'GO Lang', value: 75 },
        { skills: 'Express JS', value: 60 },
        { skills: 'Laravel PHP', value: 90 },
        { skills: 'Docker', value: 50 },
      ],

      personalSkills: [
        { skills: 'Communication', value: 90 },
        { skills: 'Team Work', value: 85 },
        { skills: 'Project Mangement', value: 80 },
        { skills: 'Creativity', value: 85 },
      ],
    }
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Patrick+Hand&display=swap');

.skills {
  padding-top: 150px;
  margin-bottom: 100px;
  font-family: 'Patrick Hand', 'Roboto', sans-serif;
}

.row-skills {
  margin-top: 75px;
}

.text-inner-bar {
  text-align: left;
  margin-left: 10px;
}
</style>
