<template>
  <div class="block__container">
    <Block/>
    <Block/>
    <Block/>
    <Block/>
    <Block/>
    <Block/>
    <Block/>
    <Block/>
    <Block/>
  </div>
</template>

<script>
import Block from '@/components/Block';
export default {
  name: 'BlockContainer',
  components: { Block },
};
</script>

<style lang="scss" scoped>
.block__container {
  padding: 1rem;
  display: grid;
  grid-template: repeat(3, 1fr) / repeat(3, 1fr);
  height: 100vh;
  width: 100%;
  grid-gap: 1rem;
}
</style>
