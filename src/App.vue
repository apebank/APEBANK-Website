<template>
  <v-app class="pos-mask ov-a" style="background: transparent">
    <v-app-bar app dark color="rgba(39, 39, 39, 0.73)">
      <div class="d-flex align-center">
        <v-img
          class="shrink mr-3"
          contain
          src="img/logo192.png"
          transition="scale-transition"
          width="40"
        />
        <h1 style="font-size: 22px">APE BANK</h1>
      </div>

      <v-spacer></v-spacer>

      <!-- <v-btn href="https://twitter.com/apebankdao" target="_blank" icon>
        <v-icon>mdi-twitter</v-icon>
      </v-btn> -->
    </v-app-bar>

    <v-main style="min-height: 70vh">
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",
};
</script>
