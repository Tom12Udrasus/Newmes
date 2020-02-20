<template>
  <div>
    <v-row align="center" justify="end">
      <v-col cols="10" align="center" justify="end">
        <h1 class="green--text text--darken-2">
          <v-icon large color="green darken-2">mdi-account-outline</v-icon>Иван Иванов
        </h1>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="2" align="center" justify="end">
        <img src="https://randomuser.me/api/portraits/men/7.jpg" style="max-width: 100%" />
      </v-col>
      <v-col align="center" justify="end">
        <p>
          Веб-сайт:
          <a href="..." target="_blank">...</a>
        </p>
        <p>
          E-mail:
          <a href="mailto:...">...</a>
        </p>
        <p>Город: ...</p>
        <p>Место работы: ...</p>
      </v-col>
    </v-row>ОСТАЛЬНОЕ СОДЕРЖИМОЕ СТРАНИЦЫ
    <!-- {{info}} -->
  </div>
</template>
<style>
</style>
<script>
export default {
  data() {
    return {
      info: null
    };
  },
  mounted() {
    this.$axios
      .get("https://api.coindesk.com/v1/bpi/currentprice.json")
      .then(response => (this.info = response));
  }
};
</script>