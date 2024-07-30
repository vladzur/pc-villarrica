<script setup>
import Footer from './components/FooterComponent.vue';
</script>
<template>
    <v-app>
        <v-main>
            <v-parallax src="/img/villarrica_parallax.jpg" height="800">
                <div class="d-flex flex-column fill-height justify-center align-center text-white">
                    <img src="@/assets/logo.svg" alt="Partido Comunista de Chile" class="logo">
                    <h1 class="text-h1">
                        Partido Comunista de Chile
                    </h1>
                    <h2 class="text-h2">
                        Villarrica
                    </h2>
                </div>
            </v-parallax>
            <v-container fluid>
                <v-container>
                    <v-row>
                        <v-col>
                            <v-card>
                                <v-card-title>
                                    Bienvenidos al Partido Comunista de Chile en Villarrica
                                </v-card-title>
                                <v-card-subtitle>
                                    Célula “Hermanos Velásquez Mardones”
                                </v-card-subtitle>
                                <v-card-text>
                                    <p>
                                        Estamos trabajando arduamente en la construcción de nuestro sitio web. Pronto,
                                        ofreceremos contenido relevante y de interés para todos los habitantes de
                                        Villarrica.

                                        ¡Mantente atento! Muy pronto estaremos listos para compartir nuestras ideas,
                                        noticias y actividades.

                                        ¡Hasta pronto!
                                    </p>
                                </v-card-text>
                            </v-card>
                        </v-col>
                    </v-row>
                </v-container>

            </v-container>
        </v-main>
        <Footer />
    </v-app>
</template>
