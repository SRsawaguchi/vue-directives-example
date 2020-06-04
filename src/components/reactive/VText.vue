<template>
  <section>
    <h3>v-text</h3>
    <p>入力内容に応じて、textContentが変わる。</p>
    <p>
      <input type="text" v-model="message" />
      &nbsp;=&nbsp;
      <span v-text="message"></span>
    </p>
  </section>
</template>

<script>
export default {
  name: 'VText',
  data: function() {
    return {
      message: '',
    };
  },
};
</script>

<style></style>
