<template>
    <div>
        <button type="button" @click="click" class="btn btn-outline-success">{{name}}</button>
    </div>
</template>

<style>
.btn {
    border-radius: 50%;
    margin: 5px;
}
    
</style>

<script>
export default {
    props: {
        name: {
            type: String,
            default: "+",
        },
    },
    click : {
        type: Function,
        default: function() {
            alert("Button Clicked");
        }
    }
}
</script>