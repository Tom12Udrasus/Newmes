<template>
  <div>
    <v-row class="text-left">
      <v-col cols="10">
        <h1 class="green--text text--darken-2">
          <v-icon large color="green darken-2">mdi-account-outline</v-icon>Иван Иванов
        </h1>
      </v-col>
    </v-row>
    <v-row class="text-left">
      <v-col cols="2">
        <img src="https://randomuser.me/api/portraits/men/7.jpg" style="max-width: 100%" />
      </v-col>
      <v-col cols="10" class="text-left">
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
  </div>
</template>

<script>
// new Vue({
//   el: "#appp",
//   data() {
//     return {
//       info: null
//     };
//   },
//   mounted() {
//     axios
//       .get("https://api.coindesk.com/v1/bpi/currentprice.json")
//       .then(response => (this.info = response));
//   }
// });
</script>