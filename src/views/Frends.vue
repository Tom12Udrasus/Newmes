<template>
  <div id="app">{{ info }}</div>
</template>
<script>
export default {
  el: "#app",
  data() {
    return {
      info: null
    };
  },
  methods() {
    axios
      .get("https://api.coindesk.com/v1/bpi/currentprice.json")
      .then(response => (this.info = response));
  }
};
</script>