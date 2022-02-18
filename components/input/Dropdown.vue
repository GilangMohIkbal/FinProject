<template>
    <div>
    <select class="custom-select" id="inputGroupSelect04" aria-label="Example select with button addon">
    <option selected>{{name}}</option>
    <option value="1">One</option>
    <option value="2">Two</option>
    <option value="3">Three</option>
  </select>
    </div>
</template>

<style>
  select{
    padding:10px;
    border:1px solid gray;
    border-radius:15px;
    margin-top: 10px;
    width: 200px;
  }
</style>

<script>
export default {
  
    props : {
        name: {
            type: String,
            default: "Input Name",
        },
    },
   
}
</script>