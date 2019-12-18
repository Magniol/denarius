<template>
    <v-app>
        <v-card>
            <v-toolbar
                    color="#993300"
                    dark
                    flat
            >
<!--                <v-app-bar-nav-icon></v-app-bar-nav-icon>-->
                <v-col style="justify-content: center">

<!--                    <v-col>-->
<!--                        <span style="font-family: Calibri">Groupe Financier</span>-->
<!--                    </v-col>-->
                    <v-col style="justify-items: center; align-items: start">
                        <span style="font-family: Castellar; font-size: xx-large"> DENARIUS </span>
                    </v-col>


<!--                    <v-col>-->
<!--                        <span style="font-family: Calibri">Financial Group</span>-->
<!--                    </v-col>-->

                </v-col>

<!--                <v-toolbar-title>Page title</v-toolbar-title>-->

                <v-spacer></v-spacer>

                <v-btn style="background-color: #FFFFFF;" color="#000000" class="button" text>
                    français
                </v-btn>


                <template v-slot:extension>
                    <v-tabs
                            v-model="currentItem"
                            background-color="transparent"
                            fixed-tabs
                            slider-color="white"
                    >


                        <v-row  class="title" >

                            <v-menu
                                    offset-y
                                    v-if="more.length"
                                    bottom
                                    left
                            >
                                <template v-slot:activator="{ on }">

                                    <v-btn
                                            text
                                            class="align-self-center mr-4"
                                            v-on="on"
                                    >
                                        About Us
                                        <v-icon right>mdi-menu-down</v-icon>
                                    </v-btn>

                                </template>

                                <v-list class="grey lighten-3">
                                    <v-list-item
                                            v-for="item in more"
                                            :key="item"
                                            @click="addItem(item)"
                                    >
                                        <v-list-item-title>{{ item }}</v-list-item-title>
                                    </v-list-item>
                                </v-list>
                            </v-menu>




                            <v-menu
                                    offset-y
                                    v-if="more.length"
                                    bottom
                                    left
                            >
                                <template v-slot:activator="{ on }">
                                    <v-btn
                                            text
                                            class="align-self-center mr-4"
                                            v-on="on"
                                    >
                                        What We Do
                                        <v-icon right>mdi-menu-down</v-icon>
                                    </v-btn>

                                </template>

                                <v-list class="grey lighten-3">
                                    <v-list-item
                                            v-for="item in more"
                                            :key="item"
                                            @click="addItem(item)"
                                    >
                                        <v-list-item-title>{{ item }}</v-list-item-title>
                                    </v-list-item>
                                </v-list>
                            </v-menu>



                            <v-menu
                                    offset-y
                                    v-if="more.length"
                                    bottom
                                    left
                            >
                                <template v-slot:activator="{ on }">
                                    <v-btn
                                            text
                                            class="align-self-center mr-4"
                                            v-on="on"
                                    >
                                        Ressources
                                        <v-icon right>mdi-menu-down</v-icon>
                                    </v-btn>

                                </template>

                                <v-list class="grey lighten-3">
                                    <v-list-item
                                            v-for="item in more"
                                            :key="item"
                                            @click="addItem(item)"
                                    >
                                        <v-list-item-title>{{ item }}</v-list-item-title>
                                    </v-list-item>
                                </v-list>
                            </v-menu>





                            <v-menu
                                    offset-y
                                    v-if="more.length"
                                    bottom
                                    left
                            >
                                <template v-slot:activator="{ on }">
                                    <v-btn
                                            text
                                            class="align-self-center mr-4"
                                            v-on="on"
                                    >
                                        History of Coin
                                        <v-icon right>mdi-menu-down</v-icon>
                                    </v-btn>

                                </template>

                                <v-list class="grey lighten-3">
                                    <v-list-item
                                            v-for="item in more"
                                            :key="item"
                                            @click="addItem(item)"
                                    >
                                        <v-list-item-title>{{ item }}</v-list-item-title>
                                    </v-list-item>
                                </v-list>
                            </v-menu>







                            <v-menu
                                    offset-y
                                    v-if="more.length"
                                    bottom
                                    left
                            >
                                <template v-slot:activator="{ on }">
                                    <v-btn
                                            text
                                            class="align-self-center mr-4"
                                            v-on="on"
                                    >
                                        Client Registration
                                        <v-icon right>mdi-menu-down</v-icon>
                                    </v-btn>

                                </template>

                                <v-list class="grey lighten-3">
                                    <v-list-item
                                            v-for="item in more"
                                            :key="item"
                                            @click="addItem(item)"
                                    >
                                        <v-list-item-title>{{ item }}</v-list-item-title>
                                    </v-list-item>
                                </v-list>
                            </v-menu>






                            <v-menu
                                    offset-y
                                    v-if="more.length"
                                    bottom
                                    left
                            >
                                <template v-slot:activator="{ on }">
                                    <v-btn
                                            text
                                            class="align-self-center mr-4"
                                            v-on="on"
                                    >
                                        Contact
                                        <v-icon right>mdi-menu-down</v-icon>
                                    </v-btn>

                                </template>

                                <v-list class="grey lighten-3">
                                    <v-list-item
                                            v-for="item in more"
                                            :key="item"
                                            @click="addItem(item)"
                                    >
                                        <v-list-item-title>{{ item }}</v-list-item-title>
                                    </v-list-item>
                                </v-list>
                            </v-menu>


                        </v-row>


                    </v-tabs>
                </template>
            </v-toolbar>
        </v-card>




        <v-content  class="composant">
            <HelloWorld/>
        </v-content>

<!--        <v-card-->
<!--                class="affichedate"-->
<!--                max-width="250"-->
<!--                elevation="7"-->
<!--                loading="rgb(33, 33, 33)"-->
<!--                loader-height="6"-->
<!--        >-->
<!--            <v-card-title style="font-size: xx-large" class="pb-0">Monday,</v-card-title>-->

<!--            <v-card-title style="font-size: xx-large" class="pb-0">December 16</v-card-title>-->

<!--            <v-card-text class="text&#45;&#45;primary">-->
<!--                <div> </div>-->
<!--                <div> </div>-->
<!--                <div style="font-size: larger; margin-left: 20%; margin-top: 5%;">1:05 AM</div>-->
<!--            </v-card-text>-->
<!--        </v-card>-->










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
            currentItem: 'tab-Web',
            items: [
                'Web', 'Shopping', 'Videos', 'Images',
            ],
            more: [
                'News', 'Maps', 'Books', 'Flights', 'Apps',
            ],
            text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.',
        }),


        methods: {
            addItem (item) {
                const removed = this.items.splice(0, 1)
                this.items.push(
                    ...this.more.splice(this.more.indexOf(item), 1)
                )
                this.more.push(...removed)
                this.$nextTick(() => { this.currentItem = 'tab-' + item })
            },
        },

    };
</script>

<style>
    .title {
        /*display: flex;*/
        justify-content: center;
        /*z-index: 3;*/
        /*margin-left: 5%;*/
        /*!*margin-top: 20vh;*!*/
        /*margin-top: 12vmax;*/
        /*background-color: rgb(33,33,33);*/
        /*border-radius: 0px 0px 10px 10px;*/

    }

    .v-app-bar{
        position: relative;
        z-index: 0;
    }

    .button:hover{
        z-index: 5;
        color: rgb(153, 51, 0);
    }

    .affichedate{
        position: absolute;
        bottom: 0;
        /*bottom: 50%;*/
    }


    .composant{
        position: relative;
    }

</style>






