<template>
  <div class="entry-title d-flex justify-content-between p-2"> 
    <div>
        <span class="text-success fs-3 fw-bold">15</span>
        <span class="fs-3 mx-1">Julio</span>
        <span class="mx-2 fs-4 fw-light">2022,Miercoles</span>
    </div>
    <div>
        <button class="btn btn-danger mx-2">
            Borrar
            <i class="fa fa-trash-alt"></i>
        </button>
        <button class="btn btn-primary">
            Subir Foto
            <i class="fa fa-upload"></i>
        </button>
    </div>
  </div>
  <hr>
  <div class="d-flex flex-column px-3 h-75">
    <textarea>Que sucedio hoy?</textarea>
  </div>
  
  <Fab
    icon = "fa-save"
  />
    <img src="https://images.contentstack.io/v3/assets/blt731acb42bb3d1659/bltb41437253cd58d82/5f4d4d504a7bbc279b8448fa/Morgana_Coven_Final.jpg" alt="entry-picture" width="750" class="img-thumbnail">
</template>

<script>
import { defineAsyncComponent } from "vue";
export default {
  components:{
    Fab: defineAsyncComponent(() => import('../components/fab.vue'))
  }
}
</script>

<style lang="scss" scoped>
textarea {
  font-size: 20px;
  border: none;
  height: 100%;
    &:focus{
      outline: none;
    }
}
img{
  width: 200px;
  position: fixed;
  bottom: 150px;
  right: 25px;
  box-shadow: 0px 5px 10px rgba($color: #000000, $alpha: 0.2);
}
</style>