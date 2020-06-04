<template>
  <article id="app">
    <h1>Vue.jsのディレクティブ</h1>
    <section>
      <VText />
      <VHtml />
      <VShow />
      <VClass />
      <VAttr />
      <VIf />
      <VSlot>
        <template v-slot:message>
          <p>Hello, World!!</p>
        </template>
      </VSlot>
      <VPre />
      <VOnce />
    </section>
  </article>
</template>

<script>
import VText from './components/reactive/VText';
import VHtml from './components/reactive/VHtml';
import VShow from './components/reactive/VShow';
import VClass from './components/reactive/VClass';
import VAttr from './components/reactive/VAttr';
import VIf from './components/reactive/VIf';
import VSlot from './components/reactive/VSlot';
import VPre from './components/reactive/VPre';
import VOnce from './components/reactive/VOnce';

export default {
  name: 'App',
  components: {
    VText,
    VHtml,
    VShow,
    VClass,
    VAttr,
    VIf,
    VSlot,
    VPre,
    VOnce,
  },
};
</script>

<style></style>
