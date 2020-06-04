<template>
  <section>
    <h3>v-slot</h3>
    <p>ここにApp.vueで指定したテンプレートが表示されます。</p>
    <slot name="message">Default Message</slot>
  </section>
</template>

<script>
export default {
  name: 'VSlot',
};
</script>

<style></style>
