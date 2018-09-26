<template>
    <div class="drawer-toggle" role="button" @click="$emit('toggle')">
        <div class="bar"></div>
        <div class="bar"></div>
        <div class="bar"></div>
    </div>
</template>

<script>
import TheSideNavToggle from '@/components/Navigation/TheSideNavToggle';
    export default {
        name: 'TheHeader',
        components:{
            TheSideNavToggle
        }
    }
</script>

<style scoped>
    .drawer-toggle{
        display: flex;
        flex-direction: column;
        justify-content: space-around;

    }
</style>