<template>
  <div id="app">
    <BlockContainer/>
  </div>
</template>

<script>

import BlockContainer from '@/components/BlockContainer';

export default {
  name: 'App',
  components: { BlockContainer },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: monospace;
}
</style>
