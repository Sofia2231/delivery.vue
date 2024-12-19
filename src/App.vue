<script setup>
import { ref } from 'vue';
import Footer from './components/footer.vue';
import Header from './components/header.vue';
import Modal from './components/modal.vue';

import { store } from './store/index';
</script>

<template>
   <div class="page-wrapper">
     <Header  @toggleModal="store.toggleModal(true)"/>
         <main class="main">
            <router-view></router-view>
         </main>
         <Modal :isOpen="store.isOpen" @toggleModal="store.toggleModal(false)"/>
        <Footer />
     
    </div>
   
</template>

<style scoped>

</style>
