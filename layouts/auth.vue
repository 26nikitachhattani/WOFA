<template>
    <v-app>
        <v-main style="background: #f4f5f9;">
            <v-container>
                <Nuxt />
            </v-container>
        </v-main>
    </v-app>
</template>
<script>
export default {
    name: 'DefaultLayout',
    data() {
        return {
            clipped: false,
            drawer: false,
            fixed: false,
            items: [
                {
                    icon: 'mdi-apps',
                    title: 'Welcome',
                    to: '/',
                },
                {
                    icon: 'mdi-chart-bubble',
                    title: 'Inspire',
                    to: '/inspire',
                },
            ],
            miniVariant: false,
            right: true,
            rightDrawer: false,
            title: 'Vuetify.js',
        }
    },
}
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
*{
  font-family: poppins;
}
</style>