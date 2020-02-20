<template>
  <v-app id="app">
    <v-navigation-drawer v-model="drawer" app clipped>
      <!-- <v-list dense> -->
      <v-list-item two-line>
        <v-list-item-avatar>
          <img :src="'http://msuedu.ru/u/526/avatar3219.jpg'" />
        </v-list-item-avatar>
        <v-list-item-content class="text-left">
          <v-list-item-title class="font-weight-black">Sosiallink</v-list-item-title>
          <v-list-item-subtitle>Marcus Obrien</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>
      <v-divider class="my-3"></v-divider>
      <div aligen="center">
        <v-list-item link to="Home">
          <v-list-item-action>
            <v-icon>mdi-home-circle</v-icon>
          </v-list-item-action>

          <v-list-item-content>
            <v-list-item-title class="text-left">Home page</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link to="Neus">
          <v-list-item-action>
            <v-icon>mdi-hand-heart</v-icon>
          </v-list-item-action>

          <v-list-item-content>
            <v-list-item-title class="text-left">Timeline</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link to="Frends">
          <v-list-item-action>
            <v-icon>mdi-account-multiple</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Frends</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link to="Musik">
          <v-list-item-action>
            <v-icon>mdi-music-box</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>My music</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link to="Login">
          <v-list-item-action>
            <v-icon>mdi-login</v-icon>
          </v-list-item-action>

          <v-list-item-content>
            <v-list-item-title class="text-left">Login</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </div>
    </v-navigation-drawer>
    <!-- </v-list> -->
    <v-content class="px-12 py-3">
      <v-container fluid>
        <router-view />
      </v-container>
    </v-content>

    <v-app-bar app clipped-left>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-toolbar-title>Estrampava</v-toolbar-title>
    </v-app-bar>

    <v-footer app>
      <span>&copy; ceberpank</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  props: {
    source: String
  },
  data: () => ({
    drawer: null
  }),
  created() {
    this.$vuetify.theme.dark = true;
  }
};
</script>