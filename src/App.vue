<script setup>
import Footer from '@/components/FooterComponent.vue';
import NavBar from '@/components/NavBarComponent.vue';
</script>
<template>
    <v-app>
        <NavBar />
        <v-main>
            <router-view />
        </v-main>
        <Footer />
    </v-app>
</template>
