<template>
  <v-app>
    <v-app-bar
      app
      color="rgb(153, 51, 0"
      dark
    >
      <div class="d-flex align-center">

        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://scontent.fyhu1-1.fna.fbcdn.net/v/t1.15752-9/78571187_999310250401874_2848791403016749056_n.jpg?_nc_cat=103&_nc_ohc=-8ZXmHp0TeAAQmkMzPwJcotoSZHZEWqbYzdvxmjkzIpiivCWsupLmwvqA&_nc_ht=scontent.fyhu1-1.fna&oh=351eaff038ef1229a6dac1424903bc8b&oe=5E82C8D6"
          transition="scale-transition"
          width="150"
        />
      </div>

      <v-spacer>
      </v-spacer>

      <div class="container">
        <v-btn icon>
          <h>About Us</h>
        </v-btn>

        <v-btn icon>
          <h>What We Do</h>
        </v-btn>

        <v-btn icon>
          <h>Ressources</h>
        </v-btn>

        <v-btn icon>
          <h>History of Coin</h>
        </v-btn>

        <v-btn icon>
          <h>Careers</h>
        </v-btn>

        <v-btn icon>
          <h>Client Registration</h>
        </v-btn>

        <v-btn icon>
          <h>About Us</h>
        </v-btn>




      </div>














<!--      <v-btn-->
<!--        href="https://github.com/vuetifyjs/vuetify/releases/latest"-->
<!--        target="_blank"-->
<!--        text-->
<!--      >-->
<!--        <span class="mr-2">Latest Release</span>-->
<!--        <v-icon>mdi-open-in-new</v-icon>-->
<!--      </v-btn>-->
    </v-app-bar>

    <v-content>
      <HelloWorld/>
    </v-content>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
    HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>

<style>
  .container {
    display: flex;
    justify-content: space-between;
   }
</style>

