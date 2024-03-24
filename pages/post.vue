<template>
    <div>

        <v-row justify="center" align="center">
            <v-col cols="12" sm="8" md="4">
                <v-tabs>
                    <v-tab>Rent Spaces</v-tab>
                    <v-tab>Buy Spaces</v-tab>
                </v-tabs>
                <posts />
            </v-col>
        </v-row>
    </div>
</template>
<script>
export default {
    name: 'CommonPage',
    layout: 'auth'
}
</script>