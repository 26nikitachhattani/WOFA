<template>
  <v-row class="justifi">
    <v-col cols="12" sm="8" md="6">
      <v-card class="card-class px-10" elevation="0" height="500px">
        <v-card-title class="headline">
          Book 1:1 calls with experts
          <br />
          get instant ️advice
        </v-card-title>
        <v-card-text class="">
          <div class="d-flex">
            <v-text-field
              solo
              placeholder="Search"
              prepend-inner-icon="mdi-magnify"
              elevation="0"
              class="rounded-r-0"
            ></v-text-field>
            <v-btn
              height="48px"
              color="green"
              dark
              class="common-btn rounded-l-0"
              >Search</v-btn
            >
          </div>
          <div class="popular-search-class mx-2">
            popular Search

            <v-chip-group
              v-model="selection"
              active-class="deep-purple accent-4 white--text"
              column
            >
              <v-chip
                class="mx-1"
                style="color: black; font-size: 15px"
                outlined
                >Sport</v-chip
              >
              <v-chip
                class="mx-1"
                outlined
                style="color: black; font-size: 15px"
                >Diet</v-chip
              >
            </v-chip-group>
          </div>
        </v-card-text>
      </v-card>
    </v-col>
    <v-col cols="12" sm="8" md="6">
      <home-image-slider />
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>
<style scoped>
.card-class {
  background-image: url('@/assets/images/hero-bg-desktop.svg');
  background-size: cover;
  background-position: center;
}

.inputField-search {
  box-shadow: none;
  box-sizing: content-box;
}

.headline {
  color: #1d1d1f;
  font-size: 36px;
  font-weight: 700;
  line-height: 42px;
  font-family: 'Poppins', sans-serif !important;
  text-align: left;
}

.popular-search-class {
  color: #1d1d1f;
  display: flex;
  font-size: 16px;
  font-weight: 600;
  text-align: center;
  align-items: center;
}
</style>
