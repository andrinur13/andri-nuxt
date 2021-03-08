<template>
  <b-container class="contact">
    <h1 class="text-center">Contact Me</h1>
    <div class="row justify-content-center">
      <div class="col-lg-10">
        <div class="outer-card">
          <b-card-group>
            <b-card
              v-for="contact in contacts"
              :key="contact.id"
              :title="contact.name"
              img-alt="Image"
              class="mx-1 shadow card-item"
              align="center"
              img-top
              @click="openLink(contact.link)"
            >
              <img :src="contact.img" width="30%" alt="logo" />
              <b-card-text class="m-2">
                <p class="h5">{{ contact.value }}</p>
              </b-card-text>
              
            </b-card>
          </b-card-group>
        </div>
      </div>
    </div>
  </b-container>
</template>

<script>
export default {
  data() {
    return {
      contacts: [
        {
          name: 'Github',
          value: '@andrinur13',
          link: 'http://github.com/andrinur13',
          img: 'github.svg'
        },
        {
          name: 'Email',
          value: 'andribis13@gmail.com',
          link: 'mailto:andribis13@gmail.com',
          img: 'email.svg'
        },
        {
          name: 'Telegram',
          value: '@andrinur13',
          link: 'http://t.me/andrinur13',
          img: 'telegram.svg'
        },
      ],
    }
  },

  methods: {
      openLink: function (link) {
          window.open(link)
      }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Patrick+Hand&display=swap');

.contact {
  font-family: 'Patrick Hand', 'Roboto', sans-serif;
}

.outer-card {
  margin-top: 100px;
  margin-bottom: 100px;
}

.card-item:hover {
  background-color: whitesmoke;
}
</style>
