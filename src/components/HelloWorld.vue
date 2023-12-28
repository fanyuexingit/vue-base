<template>
  <div v-bind:class="dynamicClass" :id="dynamicId">test</div>

  <button :disabled="isButtonisabled">button</button>

  <div v-bind="objectOfAttrs"></div>
</template>



<script>
export default{
  data(){
    return{
      dynamicClass:"appClass",
      dynamicId:"appId",
      dynamicTitle:null,
      isButtonisabled:false,
      objectOfAttrs: {
        class:"appClass",
        id:"appId",
      }
    }
  }
}
</script>


<style>
.appClass{
  color: red;
  font-size: 20px;
}

</style>