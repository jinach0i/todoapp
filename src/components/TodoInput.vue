<template>
    <div class="input-box">
        <input type="text" v-model="newTodoItem" placeholder="Type you can do here" v-on:keyup.enter="addItem">
        <span class="add-icon" v-on:click="addItem">
            <i class="fas fa-plus-square"></i>
        </span>
    </div>
</template>
<script>
export default {
    data() {
        return {
            newTodoItem: ''
        }
    },
    methods: {
        addItem(){
            if (this.newTodoItem !== "") {
                localStorage.setItem(this.newTodoItem && this.newTodoItem.trim(), this.newTodoItem && this.newTodoItem.trim());
                this.clearInput();
            }
            // document.write('<p>내가방금인풋에뭐라썼게?</p>')
        },
        clearInput(){
                this.newTodoItem = '';
            },
    }
}
</script>
<style>
    div.input-box{ height: 50px; line-height: 50px; border-radius: 5px;}
    input{border: 1px solid lightgreen; width: 55%; height: 3rem; font-size: 1rem;}
    input:focus{outline: 1px solid seagreen;}
    span.add-icon{ display: inline-block;}
    span.add-icon i{color:#39be61; vertical-align: middle; font-size: 3rem;}
</style>