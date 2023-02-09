<template>
    <div>
        
        <h2>This is a About page</h2>
        <div class="info">
        <img src='../assets/guy.png' alt="A avatar of Guy_Z">
        
        <ol>
            <li>His Full name is:</li>
            <li>He had a starnge taste over mate.</li>
            <li>Of course he have a unhuman brian.</li>
        </ol>
        </div>
        
        
    </div>
</template>


<script setup>
import { ref, computed } from 'vue';


const img = '../assets/guy.png'// What's the problem here? Why can't I bind this img to the template?

// const img = computed({
//     get(){
//         console.log('Test')
//         return 'Slay-Vue\src\assets\guy.png';
//     }
// })

//button logic
const counter = ref(0)
function changeNum(){
    counter.value++
}




</script>

<style scoped>

ol{
    width: max-content;
    height: auto;
    margin-top: auto;
    margin-bottom: 30px;
    padding: 20px 10px 20px 20px;
    border: 2px solid blueviolet;
}

li{
    font-size: 1.2em;
    font-weight: bold;
    list-style: none;
}
.info{
    border-top: 5px dashed grey;
    border-bottom: 5px dashed grey;
    padding: 20px 0 20px ;
    width: 600px;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
}

img{
    width: 100px;
    display: inline;
    mix-blend-mode:color-burn;
}






img{
    width: 200px;
}

</style>