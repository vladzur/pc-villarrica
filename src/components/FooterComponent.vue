<script setup>
const goToInstagram = () => {
    window.open('https://www.instagram.com/partido.comunista.villarrica/', '_blank');
}
const goToFacebook = () => {
    window.open('https://www.facebook.com/people/PC-Villarrica/61552411023948/', '_blank');
}
const goToYoutube = () => {
    window.open('https://www.youtube.com/@PCVillarrica', '_blank');
}

</script>
<template>
    <v-footer padless height="auto" color="red-darken-4" class="text-center">
        <v-row class="align-center justify-center">
            <v-col cols="12" class="py-4">
                <v-icon color="white" class="mx-2" @click="goToInstagram">
                    <v-icon icon="mdi-instagram" />
                </v-icon>
                <v-icon color="white" class="mx-2" @click="goToFacebook">
                    <v-icon icon="mdi-facebook" />
                </v-icon>
                <v-icon color="white" class="mx-2" @click="goToYoutube">
                    <v-icon icon="mdi-youtube" />
                </v-icon>
            </v-col>
            <v-col cols="12" class="py-4">
                <span class="white--text">&copy; {{ new Date().getFullYear() }} - PC Villarrica</span>
            </v-col>
            <v-col cols="12" class="py-4">
                <v-icon color="white" class="mx-2">
                    <v-icon icon="mdi-hammer-sickle" />
                </v-icon>
            </v-col>
        </v-row>
    </v-footer>
</template>
