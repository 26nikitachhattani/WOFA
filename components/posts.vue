<template>
    <div>
        <v-row>
        <v-col cols="12" sm="8" md="4" v-for="i in 5" :key="i">
        <v-card v-for="i in 5" :key="i" :loading="loading" class="mx-auto card-class my-12" width="100%">
            <template slot="progress">
                <v-progress-linear color="deep-purple" height="10" indeterminate></v-progress-linear>
            </template>
            <!-- <v-card-title class="my-0"><v-col class="ma-0 pa-0" cols="2">
                    <v-avatar>
                        <img src="https://cdn.vuetifyjs.com/images/john.jpg" alt="John">
                    </v-avatar>
                </v-col>
                <v-col class="ma-0 pa-0">
                    <div style="line-height: 15px; font-size: 20px;">Cafe Badilico</div>
                </v-col>
            </v-card-title> -->

           <div class=" pa-2">
            <v-img height="250" src="https://cdn.vuetifyjs.com/images/cards/cooking.png" class="image-class"></v-img>
           </div>
            <div class="my-2 d-flex">
                <v-icon class="mx-2 ">mdi-heart-outline</v-icon>
                <v-icon class="mx-2 ">mdi-comment-outline</v-icon>
                <v-icon class="mx-2 ">mdi-send-outline</v-icon>
            </div>
            <v-card-text>
                <v-row align="center" class="mx-0">
                    <!-- <v-rating :value="4.5" color="amber" dense half-increments readonly size="14"></v-rating> -->
                    <div class="black--text ">
                        18,352 likes
                    </div>
                </v-row>

                <div class="my-4 text-subtitle-1">
                    $ • Italian, Cafe
                </div>

                <div class="black--text">Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.
                </div>
            </v-card-text>

            <v-divider class="mx-4"></v-divider>

            <!-- <v-card-title>Tonight's availability</v-card-title>

            <v-card-text>
                <v-chip-group v-model="selection" active-class="deep-purple accent-4 white--text" column>
                    <v-chip>5:30PM</v-chip>

                    <v-chip>7:30PM</v-chip>

                    <v-chip>8:00PM</v-chip>

                    <v-chip>9:00PM</v-chip>
                </v-chip-group>
            </v-card-text> -->

            <v-card-actions>
                <v-btn width="100%" class="common-btn white--text" color="black lighten-2"  @click="reserve">
                    Reserve
                </v-btn>
            </v-card-actions>
        </v-card>
        </v-col>
        </v-row>
    </div>
</template>
<script>
export default {
    data: () => ({
        loading: false,
        selection: 1,
    }),

    methods: {
        reserve() {
            this.loading = true

            setTimeout(() => (this.loading = false), 2000)
        },
    },
}
</script>
<style scoped>
.card-class{
    border-radius: 10px;
}
.image-class{
    border-radius: 10px;
}
</style>