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
            <p>Pembelian kain kafan diambilkan dari uang si mayat sendiri, apabila tidak ada, orang yang selama ini yang menghidupinya yang membelikan kain kafan. Bila ia tidak mampu boleh diambilkan dari uang kas masjid, atau kas RT/RW, atau yang lainnya secara sah. Apabila tidak ada sama sekali, maka wajib atas orang muslim lain yang mampu untuk membiayainya.</p>
            <p>Kain kafan paling tidak satu lapis. Sebaiknya 3 lapis bagi mayat laki-laki dan lima lapis bagi mayat perempuan. Setiap satu lapis diantaranya merupakan kain basahan. Abu Salamah ra. Menceritakan, bahwa ia pernah bertanya kepada ‘Aisyah ra. “ Berapa lapiskah kain kafan Rosululloh saw. “ tiga lapis kain putih “ jawab ‘Aisyah. ( HR. Muslim ).</p>
            <p>Cara membungkusnya adalah hamparkan kain kafan helai demi helai dengan menaburkan kapur barus pada tiap lapisnya. Kemudian si mayat diletakkan di atasnya. Kedua tangannya dilipat di atas dada dengan tangan kanan di atas tangan kiri. Mengafaninya pun tidak boleh asal-asalan. “ Apabila kalian mengafani mayat saudara kalian, kafanilah sebaik-baiknya. “ ( HR. Muslim dari Jabir Abdullah ra. ) </p>
         </div>
      </v-ons-card>
      <v-ons-card>
         <video width="320" height="240" controls>
           <source src="../assets/vid/mengkafani.mp4" type="video/mp4">
         </video>
      </v-ons-card>
   </v-ons-page>
</template>

<script>
export default {
  name: 'mengkafani',
  data () {
    return {
      msg: 'Mengkafani Jenazah'
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
