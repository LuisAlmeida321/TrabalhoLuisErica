<template>
  <vue-horizontal-timeline :items="lista" />
</template>

<script>
  export default {
    data() {
      const example1 = {
        title: "Title example 1",
        content:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut ex dolor, malesuada luctus scelerisque ac, auctor vitae risus. Vivamus risus dolor, faucibus a bibendum quis, facilisis eget odio."
      };
      const example2 = {
        title: "Title example 2",
        content:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut ex dolor, malesuada luctus scelerisque ac, auctor vitae risus. Vivamus risus dolor, faucibus a bibendum quis, facilisis eget odio."
      };
      const example3 = {
        title: "Title example 3",
        content:
          "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut ex dolor, malesuada luctus scelerisque ac, auctor vitae risus. Vivamus risus dolor, faucibus a bibendum quis, facilisis eget odio."
      };
      const lista = [example1, example2, example3, example3, example3, example1, example2, example3, example3, example3];

      return { lista };
    }
  };
</script>