<template>
  <section>
    <h3>v-once</h3>
    <p>最初の1回だけレンダリングされ、それ以降は更新されない。</p>
    <p>
      <input type="text" v-model="message" />
      &nbsp;=&nbsp;
      <span v-once>入力したのは「{{ message }}」ですね。</span>
    </p>
  </section>
</template>

<script>
export default {
  name: 'VOnce',
  data: function() {
    return {
      message: 'First message',
    };
  },
};
</script>

<style></style>
