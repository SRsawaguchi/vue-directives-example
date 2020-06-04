<template>
  <section>
    <h3>v-html</h3>
    <p>入力内容に応じて、innerHTMLが変わる。</p>
    <p>
        <input type="text" v-model="elt" />
        <span v-html="elt"></span>
    </p>
  </section>
</template>

<script>
export default {
    name: 'VHtml',
    data: function () {
        return {
            elt: '',
        };
    },
};
</script>

<style></style>
