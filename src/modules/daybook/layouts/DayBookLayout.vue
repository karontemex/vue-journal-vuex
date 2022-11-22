<template>
    <navbar></navbar>
    <div class="d-flex">
        <div class="col-4">
                <entrylist></entrylist>
        </div>
        <div class="col">
            <router-view/>
        </div>
    </div>
</template>

<script>
import {defineAsyncComponent} from 'vue';
export default {
    components:{
        navbar: defineAsyncComponent(()=>import('../components/navbar.vue')),
        entrylist: defineAsyncComponent(()=>import('../components/entrylist.vue'))
        
    }
}
</script>
