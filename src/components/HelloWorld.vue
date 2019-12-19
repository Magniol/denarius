<template>
  <v-container class="conteneur"  >
      <v-card
              class="mx-auto"
              max-width="400"
      >
        <v-img
                class="white--text align-end"
                height="200px"
                src="./argent.jpg"
                style="margin-top: -250%"
        >
          <v-card-title>Welcome to Denarius</v-card-title>
        </v-img>

<!--        <v-card-subtitle class="pb-0">Number 10</v-card-subtitle>-->

        <v-card-text class="text--primary">
          <div>Pour de plus amples renseignements relatifs aux opérations de change des entreprises, n'hésitez pas à communiquer avec Denarius. Vos questions et vos commentaires sont extrêmement importants pour Denarius</div>

<!--          <div>Whitsunday Island, Whitsunday Islands</div>-->
        </v-card-text>

        <v-card-actions>
          <v-btn
                  color="#FFFFFF"
                  text
                  style="font-size: xx-large; margin-top: -220%"
          >
            Thursday, December 19  12:34 PM
          </v-btn>


        </v-card-actions>
      </v-card>
  </v-container>
</template>

<script>
export default {
  name: 'HelloWorld',

  data: () => ({

  }),
};
</script>


<style>
  .conteneur{

    max-height: 100%;
    max-width: 100%;
    width: 100%;
    height: 100%;
    /*background-color: #757575;*/
  }

  .image{
    width: 100%;
    height: 100%;
  }
</style>