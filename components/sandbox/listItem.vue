<template>
  <ul class="list-group list-group-flush">
    <li v-for="(item, i) in items" :key="i" class="list-group-item d-flex justify-content-between">
      <span>{{ item }}</span>
      <button type="button" @click="clickDelete(i)" class="btn btn-danger">
        -
      </button>
    </li>
  </ul>
</template>
<script>
export default {
  props: {
    items: {
      type: Array,
      default: () => [],
    },
  },
  methods: {
    clickDelete(index) {
      const newValue = this.items.filter((item, i) => i !== index);
      this.$emit("get", newValue);
    },
  },
};
</script>
