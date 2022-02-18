<template>
<div class="mt-5" style="display:flex;justify-content:center;" >
   <div class="text-center mt-5">
   <input type="text" class="form-control text-center mb-3" v-model="todo" placeholder="ketikan sesuatu"/>
    <button type="button" class="bt" @click="tambahTodo"> Tambah</button>

    <!-- todolist -->
    <p>todolist :</p>
    <div v-if="isNoTodolist">
      <small>tambahkan data</small>
    </div>
    <ul class="list-group list-group-flush">
    <li v-for="(datalist,i) in todolist" :key="i" class="list-group-item subjectName" >

    <div >
        <div class="form-check tim">
        <input class="list" type="checkbox" id="checkbox">
        <label class="form-check-label" for="checkbox">
          {{datalist}}
        </label>
        <button type="button" class="btn btn-danger" @click="deleteTodo">
        <i class="fas fa-trash"></i>
        </button>
        </div>
        
        </div>

    </li>
    </ul>

    <!-- listdone -->
    <div class="list-done">
        <p>list done :</p>

        <li v-for="(datadone,i) in listdone" :key="i">
    <div style="display:flex; align-item:center; justify-content:flex-between;">
        
        <div class="form-check" @click="changeListDone" >
        <input class="form-check-input" type="checkbox" value="" id="defaultCheck1">
        <label class="form-check-label" for="defaultCheck1">
        </label>
        </div>
        {{datadone}} 
        <div>
        <button type="button" @click="deleteListDone" class="btn btn-danger">
        <i class="fas fa-trash"></i>
        </button>
        </div>
        </div>

    </li>
    </div>
  </div>
  </div>
</template>

<script>
export default {
    
    

  data() {
    return {
      todo:"",
      todolist: [],
    listdone: [],  
    }
  },


  computed: {
    isNoTodolist() {
      return this.todolist.length == 0 || this.todolist == "";
    },
    
  },


  methods : {
    tambahTodo() {
    this.todolist.push(this.todo);
    this.todo = "";
    console.log(this.todolist)
  },
  checklist () {
    var check = document.querySelectorAll(".subjectName");
    
     for (var i = 0; i <check.length; i++){
      
      
      check[i].classList.toggle("checked");
 

  }
  },
    deleteTodo(index) {
      // this.todolist.splice((todolist, i) => i !== index);
      this.todolist.splice(index, 1);
    },
    deleteListDone(datalist) {
      this.listdone.splice(datalist.target.parentNode.parentNode.dataset.index, 1);
    },
    changeListDone(listdone) {
      this.todolist.push(this.listdone[listdone.target.parentNode.parentNode.dataset.index]);
      this.listdone.splice(listdone.target.parentNode.parentNode.dataset.index, 1);
      console.log(listdone);
    }
  },
  
}
</script>

<style>
.bt {
  background-color: rgb(68, 105, 206);
  padding: 10px 15px;
  border: none;
  border-radius: 10px;
  color: white;
  transition: 0.5s;
}

.bt:hover {
  padding: 13px 25px rgb(68, 105, 206);
  border: 1px solid ;
  background-color: white;
  color: rgb(68, 105, 206);
}

.tim {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>