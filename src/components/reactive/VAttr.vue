<template>
  <section>
    <h3>v-attr</h3>
    <p>v-attrは削除されたので、代わりにv-bindをつかう。</p>
    <input type="number" v-model="inputWidth" placeholder="widthを入力" /><br />
    <img src="../../assets/logo.png" v-bind="{width: inputWidth}" alt="" />
  </section>
</template>

<script>
export default {
  name: 'VAttr',
  data: function() {
    return {
      inputWidth: 200,
    };
  },
};
</script>

<style></style>
