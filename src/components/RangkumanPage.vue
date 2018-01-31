<template>
   <v-ons-page>
      <v-ons-toolbar class="home-toolbar">
         <div class="left">
            <v-ons-toolbar-button @click="$store.commit('splitter/toggle')">
               <v-ons-icon icon="ion-navicon, material:md-menu"></v-ons-icon>
            </v-ons-toolbar-button>
         </div>
         <div class="center">{{ msg }}</div>
      </v-ons-toolbar>
      <v-ons-card>
         <div>
            <ol>
               <li>Kewajiban kita terhadap jenazah antara lain : memandikan, mengafani, menyalati, dan meguburnya</li>
               <li>Yang berhak memandikan jenazah adalah keluarga terdekat, bapak, ibu, suami, istri dan anak</li>
               <li>Bagi laki-laki disunnahkan tiga helai kain kafan, bagi perempuan lima helai kain kafan</li>
               <li>Tata cara shalat jenazah berbeda dengan shalat biasa. Pada shalat jenazah, tidak ada ruku dan sujud, hanya empat kali takbir dan diselingi doa</li>
               <li>Cara mengingat mati adalah dengan menjeguk atau ber-ta’ziyyah dan berziarah kubur</li>
               <li>Mengurus jenazah hukumnya fardlu kifayah, yaitu kewajiban secara bersama-sama atau gotong royong.</li>
            </ol>
         </div>
      </v-ons-card>

   </v-ons-page>
</template>

<script>
export default {
  name: 'rangkuman',
  data () {
    return {
      msg: 'Rangkuman'
    }
  },
  methods: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header {
  text-align: center;
}

img {
  max-width: 300px;
}

ons-list-title {
  text-transform: none;
}

ons-list-title:not(:first-of-type) {
  margin-top: 30px;
}

ons-card {
  text-align: left;
}

ons-list-item, ons-card {
  cursor: pointer;
}
</style>
