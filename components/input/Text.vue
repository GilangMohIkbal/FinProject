<template>
   
  <input type="text" class="form-control"  :placeholder="name" >

</template>


<style>
.input-group input {
    padding:10px;
    border:1px solid gray;
    border-radius:15px;
    margin-top: 10px;
}
    
</style>
<script>
export default {
    data() {
        return {

        }
    },
    props: {
        name: {
                type: String,
                default: "Input Name",
            },
         model: {
                type: String,
        },
       
    }

    
}
</script>