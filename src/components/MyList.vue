<template>
<li class="list-group-item" @dblclick="edit()">
    <input type="text" v-if="isEdit" v-model="listText" @keyup.enter="saveItem()" class="form-control">
    <span v-else>{{ listText }}</span>
</li>
    
</template>

<script>
    export default {
       name:'MyList' ,
       data() {
        return {
            listText:"",
            isEdit:true
        }
       },
       methods: {
        saveItem(){
          return  this.isEdit=false;
        },
        edit(){
            return this.isEdit=true;
        }
       },
    }
</script>

<style lang="scss" scoped>

</style>