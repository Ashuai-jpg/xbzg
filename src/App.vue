<script setup>
import { RouterLink, RouterView } from 'vue-router'


</script >

<template>

  <header>
    <h1>This is Nav Bar</h1>


  </header>

  <body>
    <div class="container">
      <nav>

        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>

      </nav>
      <div class="item">
        <RouterView></RouterView>
      </div>

    </div>



  </body>



</template>


<style scoped>
header {
  display: flex;
  flex-direction: column;

}

body {
  display: flex;
  justify-content: center;
  border: 20px solid red;

}
.container{
  border: 5px solid yellow;
  display: inherit;
  flex-direction: column;
  width: 800px;
}
h1 {
  display: inherit;
  align-self: center;
}

nav {
  display: inherit;
  align-items: center;
  justify-content: space-around;

}

.item {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-items: center;

}




/* @media (max-width: 480px){
    .item{
      display:flex;
      flex-direction: column;
      justify-content: flex-start;
    }
} */
</style>

















