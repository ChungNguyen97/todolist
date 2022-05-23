<template>
  <div class="product">
    <h3>{{ title }}</h3>
    <ul>
      <li v-for="{id,title} in listProduct" :key="id">
        {{id}} - {{title}}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "ProductPage",
  data() {
    return {
      title: "Product Page",
      listProduct: [],
    };
  },
  methods: {
    async callData() {
      const res = await fetch(
        "https://jsonplaceholder.typicode.com/todos?_limit=10"
      );
      const data = res.json();
      return (this.listProduct = await data);
    },
  },
  created() {
    this.callData();
  },
};
</script>

<style>
</style>