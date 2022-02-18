<template>
  <div class="row">
    <div class="col-md-9">
      <select id="pembaca" v-model="selectPembaca" class="form-control rounded-pill px-3">
        <option v-for="(pembaca, i) in listPembaca" :key="i">{{ pembaca }}</option>
      </select>
      <select id="buku" v-model="selectBuku" class="form-control rounded-pill px-3 mt-3">
        <option v-for="(buku, i) in listBuku" :key="i">{{ buku }}</option>
      </select>
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
  props: {
    listPembaca: {
      type: Array,
      default: () => [],
    },
    listBuku: {
      type: Array,
      default: () => [],
    },
  },
  data() {
    return {
      selectPembaca: "",
      selectBuku: "",
    };
  },
  methods: {
    clickAdd() {
      this.$emit("get", this.selectPembaca + " - " + this.selectBuku);
      this.selectPembaca = "";
      this.selectBuku = "";
    },
  },
};
</script>
