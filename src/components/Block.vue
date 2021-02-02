<template>
  <div @click="hit" class="block__item" :class="{killed}">
    {{ hp }}
  </div>
</template>

<script>
export default {
  name: 'Block',
  data() {
    return {
      hp: Math.floor(Math.random() * 10) + 1,
    };
  },
  computed: {
    killed() {
      return !this.hp;
    },
  },
  methods: {
    hit() {
      if (this.hp) this.hp--;
    },
  },
};
</script>

<style lang="scss" scoped>
.block__item {
  background-color: cornflowerblue;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  font-size: 3rem;
  user-select: none;
  cursor: pointer;

  &.killed {
    background-color: lightgrey;
  }
}
</style>
