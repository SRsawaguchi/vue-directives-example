<template>
  <section>
    <h3>v-class</h3>
    <p>削除されたので、代わりにv-bind:classを使う。</p>
    <ul>
      <li>
        <input id="vclass-large" type="checkbox" v-model="fontLarge" />
        <label for="vclass-large">.font-large</label>
      </li>
      <li>
        <input id="vclass-blue" type="checkbox" v-model="fontBlue" />
        <label for="vclass-blue">.font-blue</label>
      </li>
    </ul>
    <p v-bind:class="textStyle">ここにクラスをつけます。</p>
  </section>
</template>

<script>
export default {
  name: 'VClass',
  data: function() {
    return {
      fontLarge: false,
      fontBlue: false,
    };
  },
  computed: {
    textStyle() {
      return {
        'font-large': this.fontLarge,
        'font-blue': this.fontBlue,
      };
    },
  },
};
</script>

<style>
.font-large {
  font-size: 1.61em;
}

.font-blue {
  color: #55f;
}
</style>
