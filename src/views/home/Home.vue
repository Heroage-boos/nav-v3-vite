<template>
    <div class="home-container">
        <div class="con-search">
            <Search />
        </div>
        <div class="con-nav-detail">
            <NavContent />
        </div>
    </div>
</template>
  
<script lang="ts">
import { defineComponent } from 'vue';
import Search from "@/components/Search.vue";
import NavContent from "@/views/home/NavContent.vue";
// import Search from "@/components/Search.vue";


export default defineComponent({
    name: 'HomeView',
    components: {
        Search,
        NavContent
    }
});
</script>
<style lang="scss" scoped>
.home-container {
    border: solid 1px red;
    display: flex;
    flex-direction: column;
    height: 100%;

    .con-search {
        height: 80px;
        border: solid 1px green;
    }

    .con-nav-dateil {
        flex: 1;
        border: solid 1px pink;
    }
}
</style>
