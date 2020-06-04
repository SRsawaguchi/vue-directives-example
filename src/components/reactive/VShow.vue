<template>
  <section>
    <h3>v-show</h3>
    <p>
      true or
      falseに応じて表示したり、隠したりする。v-ifと違って、条件がfalseの場合でも要素自体はDOM上にある。CSSで表示するか否か切り替えているだけ。j
    </p>
    <input type="checkbox" v-model="showMessage" />
    <span v-show="showMessage">ON</span>
  </section>
</template>

<script>
export default {
  name: 'VShow',
  data: function() {
    return {
      showMessage: false
    };
  },
};
</script>

<style></style>
