<template>
    <v-row justify="center"  align="center">
        <v-col cols="12" sm="8" md="5">
            <div >
            <v-card class="login-card pa-3 align-self-center">
                <v-card-text>
                    <div>Mobile Number*</div>
                    <v-text-field height="40" label="Outlined" outlined></v-text-field>
                </v-card-text>
                <v-card-text>
                    <v-btn width="100%" color="black" dark elevation="0"  nuxt to="/inspire">Next</v-btn> 
                    <div class="mx-3 my-1 text-center">
                        By Continuing, you agree to our Terms of Service and Privacy Policy.
                    </div>
                </v-card-text>

            </v-card>
            </div>
        </v-col>
    </v-row>
</template>
<script>
export default {
    name: 'CommonPage',
    layout: 'auth'
}
</script>
<style>
.login-card {
    border-radius: 12px !important;
    align-items: center;
}
</style>