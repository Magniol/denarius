<template>
  <v-app>
<!--    <v-app-bar-->
<!--      app-->

<!--      color="#D84315"-->
<!--      dark-->
<!--    >-->
<!--      <div class="d-flex align-center">-->

<!--        <v-img-->
<!--          alt="Vuetify Logo"-->
<!--          class="shrink mr-2"-->
<!--          contain-->
<!--          src="https://scontent.fyhu1-1.fna.fbcdn.net/v/t1.15752-9/78571187_999310250401874_2848791403016749056_n.jpg?_nc_cat=103&_nc_ohc=-8ZXmHp0TeAAQmkMzPwJcotoSZHZEWqbYzdvxmjkzIpiivCWsupLmwvqA&_nc_ht=scontent.fyhu1-1.fna&oh=351eaff038ef1229a6dac1424903bc8b&oe=5E82C8D6"-->
<!--          transition="scale-transition"-->
<!--          width="150"-->
<!--        />-->
<!--      </div>-->

<!--      <v-spacer>-->
<!--      </v-spacer>-->

<!--      <div class="container">-->
<!--        <v-row class="ligne">-->
<!--          <v-btn icon>-->
<!--            <h>About Us</h>-->
<!--          </v-btn>-->

<!--          <v-btn icon>-->
<!--            <h>What We Do</h>-->
<!--          </v-btn>-->

<!--          <v-btn icon>-->
<!--            <h>Ressources</h>-->
<!--          </v-btn>-->

<!--          <v-btn icon>-->
<!--            <h>History of Coin</h>-->
<!--          </v-btn>-->

<!--          <v-btn icon>-->
<!--            <h>Careers</h>-->
<!--          </v-btn>-->

<!--          <v-btn icon>-->
<!--            <h>Client Registration</h>-->
<!--          </v-btn>-->

<!--          <v-btn icon>-->
<!--            <h>About Us</h>-->
<!--          </v-btn>-->
<!--        </v-row>-->

<!--      </div>-->

    <v-card flat>
      <v-toolbar
              color="error"
              dark
              extended
              flat
              style="opacity: 0.9"
      >

                <v-img
                  alt="Vuetify Logo"
                  class="shrink mr-2"
                  contain
                  src="https://scontent.fyhu1-1.fna.fbcdn.net/v/t1.15752-9/78571187_999310250401874_2848791403016749056_n.jpg?_nc_cat=103&_nc_ohc=-8ZXmHp0TeAAQmkMzPwJcotoSZHZEWqbYzdvxmjkzIpiivCWsupLmwvqA&_nc_ht=scontent.fyhu1-1.fna&oh=351eaff038ef1229a6dac1424903bc8b&oe=5E82C8D6"
                  transition="scale-transition"
                  width="150"
                />

      </v-toolbar>

      <v-card
              class="mx-auto"
              max-width="700"
              style="margin-top: -64px;"
      >
        <v-toolbar flat max-width="200%" style="position: relative">
<!--          <v-toolbar-title class="grey&#45;&#45;text">Title</v-toolbar-title>-->
<!--          <v-toolbar-title class="grey&#45;&#45;text">yes</v-toolbar-title>-->
          <v-row style="position: absolute">

            <v-toolbar-title class="blackt">
              <v-btn style="color: black">
                About Us
              </v-btn>
            </v-toolbar-title>

            <v-toolbar-title class="blackt">
              <v-btn class="boutton" style="color: black">
                What We Do
              </v-btn>
            </v-toolbar-title>

            <v-toolbar-title class="blackt">
              <v-btn  class="boutton" style="color: black">
                Ressources
              </v-btn>
            </v-toolbar-title>


            <v-toolbar-title class="blackt">
              <v-btn class="boutton" style="color: black">
                History of Coin
              </v-btn>
            </v-toolbar-title>



            <v-toolbar-title class="blackt">
              <v-btn class="boutton"  style="color: black">
                Careers
              </v-btn>
            </v-toolbar-title>

          </v-row>

          <v-spacer></v-spacer>

<!--          <v-btn icon>-->
<!--            <v-icon>mdi-magnify</v-icon>-->
<!--          </v-btn>-->

          <v-btn icon>
            <v-icon>mdi-apps</v-icon>
          </v-btn>

<!--          <v-btn icon>-->
<!--            <v-icon>mdi-dots-vertical</v-icon>-->
<!--          </v-btn>-->
        </v-toolbar>
      </v-card>
    </v-card>












<!--      <v-btn-->
<!--        href="https://github.com/vuetifyjs/vuetify/releases/latest"-->
<!--        target="_blank"-->
<!--        text-->
<!--      >-->
<!--        <span class="mr-2">Latest Release</span>-->
<!--        <v-icon>mdi-open-in-new</v-icon>-->
<!--      </v-btn>-->


<!--    </v-app-bar>-->

    <v-content >
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

  .ligne{
    display: flex;
    justify-content: space-around;
  }

  .boutton:hover{
      background-color: aquamarine;
      color: aqua;

  }
</style>

