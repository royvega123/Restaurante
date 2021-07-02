<template id="home-page">
<v-content>
    <v-toolbar
        color="purple"
        dark
      >
        <v-toolbar-title>BIENVENIDO A  </v-toolbar-title>

        <v-divider
          class="mx-4"
          vertical
        ></v-divider>

        <span class="subheading">Gusteau's</span>

        <v-spacer></v-spacer>

        <v-toolbar-items class="hidden-sm-and-down">
          <v-btn text >
          <v-list-item link href="/login" :ripple="true">
                      <v-list-item-icon>
                          <v-icon>mdi-view-dashboard</v-icon>
                      </v-list-item-icon>
                      <v-list-item-title>  Iniciar Sesion</v-list-item-title>
                  </v-list-item>

          </v-btn>

          <v-divider vertical></v-divider>

          <v-btn text>
            Registrate
          </v-btn>

          <v-divider vertical></v-divider>

          <v-btn text>
           Hacerca de
          </v-btn>

          <v-divider vertical></v-divider>

        </v-toolbar-items>



        <v-app-bar-nav-icon></v-app-bar-nav-icon>


      </v-toolbar>
      <v-carousel>
               <v-carousel-item
                 v-for="(item,i) in items"
                 :key="i"
                 :src="item.src"
                 reverse-transition="fade-transition"
                 transition="fade-transition"
               ></v-carousel-item>
             </v-carousel>
</v-content>
</template>
<script>
    Vue.component("home-page", {
        template: "#home-page",
      data () {
          return {
            items: [
              {
                src: 'https://www.peru.travel/Contenido/Noticia/Imagen/pe/174/1.1/Principal/88.jpg',
              },
              {
                src: 'https://cnnespanol.cnn.com/wp-content/uploads/2019/01/Galerias-nuevos-restaurantes-2019-CNN-1.jpg?quality=100&strip=info',
              },
              {
                src: 'https://gestion.pe/resizer/h6Zig3yPGvhlUSwmFYYROlq2I7o=/580x330/smart/filters:format(jpeg):quality(75)/cloudfront-us-east-1.images.arcpublishing.com/elcomercio/2YSGG6JP3NGRVPYV3NY5VT7VYU.jpg',
              },
              {
                src: 'https://www.peru.travel/Contenido/Noticia/Imagen/pe/174/1.1/Principal/88.jpg',
              },
            ],
          }
        },
    })
</script>

