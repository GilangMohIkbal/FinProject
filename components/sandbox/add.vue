<template>
  <div class="row">
    <div class="col-md-9">
      <input type="text" v-model="inputan" class="form-control rounded-pill px-3" />
    </div>
    <div class="col-md-3">
      <button type="button" class="btn btn-outline-primary rounded-circle" @click="clickAdd">
        <i class="fas fa-plus"></i>
      </button>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      inputan: "",
    };
  },
  methods: {
    clickAdd() {
      this.$emit("get", this.inputan);
      this.inputan = "";
    },
  },
};
</script>
