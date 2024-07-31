<script setup>
import { ref } from 'vue';
const news = ref([]);
const getNews = async () => {
    const response = await fetch('https://api.rss2json.com/v1/api.json?rss_url=https://www.pcchile.cl/feed/');
    const data = await response.json();
    news.value = data.items;
}
getNews();
</script>
<template>
    <v-container>
        <v-row>
            <v-col cols="12">
                <h2 class="text-h2 text-center">Noticias</h2>
            </v-col>
        </v-row>
    </v-container>
    <v-container>
        <v-row>
            <v-col cols="12" md="6" v-for="item in news" :key="item.guid">
                <v-card>
                    <v-card-title><span class="font-weight-black">{{ item.title }}</span></v-card-title>
                    <v-card-subtitle>{{ item.pubDate }}</v-card-subtitle>
                    <v-card-text><span v-html="item.description"></span></v-card-text>
                    <v-card-actions>
                        <v-btn variant="outlined" :href=item.link target="_blank">Ver más</v-btn>
                    </v-card-actions>
                </v-card>
            </v-col>
        </v-row>
    </v-container>
</template>
