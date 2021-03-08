<template>
  <div class="education" id="education">
    <h1 class="text-center">Education</h1>
    <b-container>
      <div
        class="card-box col-lg-8 mx-auto"
        v-for="edu in educations"
        :key="edu.id"
      >
        <b-card no-body class="overflow-hidden shadow box-item">
          <b-row no-gutters>
            <b-col md="3">
              <b-card-img
                :src="edu.img"
                alt="Image"
                class="rounded-0 p-2"
              ></b-card-img>
            </b-col>
            <b-col md="5">
              <b-card-body>
                <h4> {{edu.name}} </h4>
                <span class="badge badge-primary"> {{edu.year}} </span>
                <br>
                <span> {{edu.title}} </span>
              </b-card-body>
            </b-col>
          </b-row>
        </b-card>
      </div>
    </b-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      educations: [
        { name: 'University of Ahmad Dahlan Yogyakarta', year: '2018-2022', title: 'Informatics Engineering', img:'uad.png' },
        { name: 'SMK Negeri 1 Bantul', year: '2014-2017', title: 'Computer & Network Engineering', img:'smk.jpeg' },
        { name: 'SMP Negeri 2 Bantul', year: '2011-2014', img:'smp.png' },
        { name: 'SD Muhammadiyah 34 Cikupa', year: '2004-2011', img:'sd.png' },
      ],
    }
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Patrick+Hand&display=swap');

.education {
  font-family: 'Patrick Hand', 'Roboto', sans-serif;
  margin-top: 100px;
  margin-bottom: 50px;
}

.card-box {
  margin-top: 50px;
}
</style>
