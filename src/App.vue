<template>
  <div id="app">
    <api-news></api-news>
    <section id="team" class="pb-5">
      
      <div class="container">
        
        <div class="row">
          <div class="col-xs-12 col-sm-6 col-md-3" v-for="(item, index) of team" :key="index">
            <team-card :member="item"></team-card>
          </div>
        </div>

      </div>
    </section>
  </div>
</template>

<script>

import ApiNews from './components/ApiNews.vue'
import TeamCard from './components/TeamCard.vue'

export default {
  name: 'App',
  components: {
    TeamCard,
    ApiNews,
  },




  data(){
    return{
      team: [
        {
        codigo: 1,
        nombre: 'Alexander Angulo',
        descripcion: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris condimentum ac elit et accumsan.',
        rol: 'Desarrollador full stack',
        image: 'images/alex.jpg'
      
      },
      {
        codigo: 2,
        nombre: 'Gustavo Rojas',
        descripcion: 'Lorem ipsum dolor sit amet, consetur adipiscing elit. Mauris condimentum ac elit et accumsan.',
        rol: 'Desarrollador backend',
        image: 'images/Gustavo.JPG'
      },
      {
      codigo: 3,
nombre: 'Lucas Mera',
descripcion: 'Lorem ipsum dolor sit amet, consectetur adipiscing lit. Mauris condimentulit et accumsan.',
rol: 'Desarrollador backend',
image: 'https://sunlimetech.com/portfolio/boot4menu/assets/imgs/team/img_01.png'
    },
    {
      codigo: 4,
nombre: 'Lucas Mer',
descripcion: 'Lorem  dolor sit amet, consectetur adipiscing elit. Mauris condimentum ac elit et acmsan.',
rol: 'Desarrollador backend',
image: 'https://sunlimetech.com/portfolio/boot4menu/assets/imgs/team/img_01.png'

    },


      ]
    }
  } 
}
</script>

