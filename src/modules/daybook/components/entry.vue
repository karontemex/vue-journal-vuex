<template>
  <div class="entry-container mb-3 pointer p-2"
  @click="$router.push({name:'entry', params:{id:10}})">
      <div class="entry-title d-flex">
            <span class="text-success fs-5 fw-bold">15</span>
            <span class="mx-1 fs-5">jULIO</span>
            <span class="mx-2 fw-light">2022,jueves</span>
        </div>
        <div class="entry-description">
            Ipsum ex elit nisi sunt ex aliqua aliquip irure. Labore magna consequat commodo aliqua. Excepteur ullamco laboris mollit proident exercitation eu aliqua aute fugiat occaecat magna. Enim laboris occaecat voluptate magna aliqua occaecat consectetur nisi est elit elit incididunt. Occaecat eiusmod proident adipisicing dolore magna officia enim mollit nulla cupidatat cupidatat do. Eu aliquip anim aliqua cillum dolor culpa irure eu occaecat.
        </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .entry-container{
        border-bottom: 1px solid #2c3e50;
        transition:  0.2s all ease-in;
    
        &:hover{
            background-color: lighten($color:grey, $amount: 45);
            transition:  0.2s all ease-in;
        }

        .entry-descrciption{
            font-size: 12px;
        }
    }
    .entry-title{

    }
</style>