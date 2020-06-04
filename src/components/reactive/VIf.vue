<template>
  <section>
    <h3>v-if</h3>
    <p>
      条件に応じてDOMに追加する要素を切り替えることができる。（DOMからとったり、追加したりする。）
    </p>
    <input id="v-if-add" type="checkbox" v-model="add" />
    <label for="v-if-add">写真をDOMに追加する。</label>
    <div v-if="add" class="image-frame"></div>
  </section>
</template>

<script>
export default {
  name: 'VIf',
  data: function() {
    return {
      add: false,
    };
  },
};
</script>

<style>
.image-frame {
  background-image: url('../../assets/logo.png');
  background-size: cover;
  width: 250px;
  height: 250px;
}
</style>
