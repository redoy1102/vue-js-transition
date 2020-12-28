<template>
  <div class="container">
    <transition name="appear"
    enter-active-class="animated slideInDown"
    leave-active-class="animated slideInUp">

      <div class="p-3 mb-2 bg-success text-white" v-if="display" >Hello World</div>

    </transition>

    <button @click="display=!display" class="btn btn-primary" >Toggle</button>
  </div>
</template>


<script>
export default  {
  data(){
    return{
      display: false
    }
  }
}
</script>>