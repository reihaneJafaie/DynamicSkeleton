<script setup>
import DynamicSkeleton from "./components/DynamicSkeleton.vue";
</script>

<template>
 <section>
  <div class="card">
  <img src="../src/assets/reihaneJafaie.png" alt="Avatar" style="width:100%">
  <div class="textBox">
    <h4 class="title"><b>Rei CodeBanu</b></h4> 
    <p>
      As a professional code witch,I conjure elegant spells in the form of code.
    </p>
    <div>
      github: https://github.com/reihaneJafaie
      instagram : rei_codebanu
    </div> 
  </div>
</div>

<div class="card">
  <DynamicSkeleton class="DynamicSkeleton" :height="'310px'" :width="'100%'" :borderRadius="'15px'" />
  <div class="textBox">
    <DynamicSkeleton class="DynamicSkeleton" :height="'30px'" :width="'70%'" :borderRadius="'5px'" />
    <p>
      <DynamicSkeleton class="DynamicSkeleton" :height="'20px'" :width="'100%'" :borderRadius="'5px'" />
      <DynamicSkeleton class="DynamicSkeleton" :height="'20px'" :width="'100%'" :borderRadius="'5px'" />
      <DynamicSkeleton class="DynamicSkeleton" :height="'20px'" :width="'100%'" :borderRadius="'5px'" />
    </p>
    <div>
      <DynamicSkeleton class="DynamicSkeleton" :height="'20px'" :width="'100%'" :borderRadius="'5px'" />
      <DynamicSkeleton class="DynamicSkeleton" :height="'20px'" :width="'100%'" :borderRadius="'5px'" />
    </div> 
  </div>
</div>
 </section>
</template>

<style scoped>
.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  width: 310px;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  background-color: palevioletred;
  border-radius: 18px;
  padding: 20px;
  margin: 0;
}

.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}
.title{
  font-size: 32px;
  color: aliceblue;
  margin:10px 0;
}
.textBox{
  font-size: 20px;
  margin: 0;
}

img{
  width: 100%;
  border-radius: 15px;
}
.DynamicSkeleton{

  margin: 10px auto;
}
section{
  display: flex ;
  justify-content: space-around;
  gap: 20px;
}
</style>
