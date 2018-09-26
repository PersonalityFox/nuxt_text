<template>
    <div class="sidenav-container">
        <div v-if="show"
            class="sidenav-backdrop"
            @click="$emit('close')">
        </div>
        <transition name="slide-side">
            <div v-if="show"
            class="sidenav">
                <ul class="nav-list">
                        <li class="nav-item">
                            <nuxt-link to="/posts">Blog</nuxt-link>
                        </li>
                        <li class="nav-item">
                            <nuxt-link to="about">About</nuxt-link>
                        </li>
                        <li class="nav-item">
                            <nuxt-link to="/admin">Admin</nuxt-link>
                        </li>
                    </ul>
                </div>
        </transition>
    </div>
</template>

<script>
    export default {
        name: 'TheSlidenav',
        props:{
            show:{
                type: Boolean,
                default: false
            }
        }
    }
</script>

<style scoped>
    .sidenav-container{
        height: 100%;
        width: 100%;
        background-color: rgba(0, 0, 0, 0.7);
        position: fixed;
        top:0;
        left:0;

    }
    .sidenav{
        height: 100%;
        width: 300px;
        background-color: white;
        z-index: 4;
         position: fixed;
        top:0;
        left:0;
        box-sizing: border-box;
        padding: 30px;
    }
    .nav-item{
        list-style:none;
        padding: 0;
        margin: 0;
    }
    .nav-item{
        margin: 20px 0;
    }
    .nav-item a{
        text-decoration: none;
        color: black;
    }
</style>