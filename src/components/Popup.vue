<template>
    <div>
        <h2>PopUp Component</h2>
        <button @click="$emit('close')">Close Popup</button>
    </div>
</template>

<script>
    export default {
        name:'Popup',
        emit:['close']
        
    }
</script>

<style scoped>
 button{background-color: tomato;width: 140px;height: 40px;border: 2px solid teal;border-radius: 5px;}
</style>