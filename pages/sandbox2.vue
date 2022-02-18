<template>
  <div>
    <div class="card">
      <div class="card-body">
        <h3 class="text-center mb-5">Sandbox II Frontend Basic</h3>
        <div class="row">
          <div class="col-md-4">
            <SandboxAdd @get="(newValue) => this.listBuku.push(newValue)" />
            <br />
            <SandboxListItem :items="listBuku" @get="(newValue) => (this.listBuku = newValue)" />
          </div>
          <div class="col-md-4">
            <SandboxAdd @get="getPembaca" />
            <br />
            <SandboxListItem :items="listPembaca" @get="(newValue) => (this.listPembaca = newValue)" />
          </div>
          <div class="col-md-4">
            <SandboxOption
              :listPembaca="listPembaca"
              :listBuku="listBuku"
              @get="(newValue) => this.listBacaan.push(newValue)"
            />
            <br />
            <SandboxListItem :items="listBacaan" @get="(newValue) => (this.listBacaan = newValue)" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  
  auth: false,
  data() {
    return {
      listBuku: [],
      listPembaca: [],
      listBacaan: [],
    };
  },
  methods: {
    getPembaca(newValue) {
      this.listPembaca.push(newValue);
    },
  },
};
</script>
