<template>
  <section>
    <h3>v-pre</h3>
    <p>子要素のコンパイルはスキップされます。</p>
    <p v-pre>{{ message }}</p>
  </section>
</template>

<script>
export default {
  name: 'VPre',
  data: function () {
      return {
          message: 'Hello!',
      };
  },
};
</script>

<style></style>
