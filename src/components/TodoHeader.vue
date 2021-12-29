<template>
    <header>
        <span class="hamberger">
            <i class="fas fa-bars"></i>
        </span>
        <h1>최혜진의 <em>First</em> <span>To-do-list</span>!</h1>
    </header>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    header{}
    span.hamberger{display: block; color: green; height: 2.5rem; line-height: 2.5rem; float: left; margin-left: 1.5rem; }
    span.hamberger i{font-size: 2rem; }
    h1{text-align: center; font-weight: 700; color: #2f3b52; margin: 2.5rem 0 1.5rem;}
    em{font-weight: bold; text-decoration: underline 1px #444; color:seashell;}
    h1 span{color: seagreen;}
</style>