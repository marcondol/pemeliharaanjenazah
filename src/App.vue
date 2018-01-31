<template>
  <v-ons-page id="app">
    <v-ons-splitter>
      <v-ons-splitter-side swipeable collapse width="250px"
        :animation="$ons.platform.isAndroid() ? 'overlay' : 'reveal'"
        :open.sync="menuIsOpen">
        <menu-page  @menuclicked="changePage" ></menu-page>
      </v-ons-splitter-side>

      <v-ons-splitter-content>
        <home-page v-if="this.page=='home'" ></home-page>
        <perawatan-page v-else-if="this.page=='perawatan'"></perawatan-page>
        <memandikan-page v-else-if="this.page=='memandikan'"></memandikan-page>
        <mengkafani-page v-else-if="this.page=='mengkafani'"></mengkafani-page>
        <menyalatkan-page v-else-if="this.page=='menyalatkan'"></menyalatkan-page>
        <menguburkan-page v-else-if="this.page=='menguburkan'"></menguburkan-page>
        <taziah-page v-else-if="this.page=='taziah'"></taziah-page>
        <ziarah-page v-else-if="this.page=='ziarah'"></ziarah-page>
        <rangkuman-page v-else-if="this.page=='rangkuman'"></rangkuman-page>
        <soal-page v-else-if="this.page=='soal'"></soal-page>
      </v-ons-splitter-content>
    </v-ons-splitter>
  </v-ons-page>
</template>

<script>
import HomePage from './components/HomePage'
import MenuPage from './components/MenuPage'
import PerawatanPage from './components/PerawatanPage'
import MemandikanPage from './components/MemandikanPage'
import MengkafaniPage from './components/MengkafaniPage'
import MenyalatkanPage from './components/MenyalatkanPage'
import MenguburkanPage from './components/MenguburkanPage'
import TaziahPage from './components/TaziahPage'
import ZiarahPage from './components/ZiarahPage'
import RangkumanPage from './components/RangkumanPage'
import SoalPage from './components/SoalPage'


export default {
  name: 'app',
  data: ()=>{
      return   {
                  page : "home"
               }
   },
   computed: {
       menuIsOpen: {
         get () {
            return this.$store.state.splitter.open
         },
         set (newValue) {
            this.$store.commit('splitter/toggle', newValue)
         }
    }
  },
   components: {
      HomePage,
      MenuPage,
      PerawatanPage,
      MemandikanPage,
      MengkafaniPage,
      MenyalatkanPage,
      MenguburkanPage,
      TaziahPage,
      ZiarahPage,
      RangkumanPage,
      SoalPage
  },
  methods: {
      changePage(page_id){
         this.page = page_id;
         console.log(page_id);
      }
   }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
ons-splitter-side[side=left][animation=overlay] {
  border-right: 1px solid #BBB;
}
</style>
