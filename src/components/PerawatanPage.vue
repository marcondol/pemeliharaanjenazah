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
            <p>Apabila seseorang telah dinyatakan positif meninggal dunia, ada beberapa hal yang harus disegerakan dalam pengurusan jenazah oleh keluarganya. Yaitu memandikan, mengafani, menyalati dan menguburkannya. Namun sebelum mayat itu dimandikan, ada beberapa hal yang harus diperhatikan terhadap kondisi jenazah, yaitu seperti berikut :</p>
            <ul>
               <li>Pejamkanlah matanya dan mohonkanlah ampun kepada Allah SWT atas segala dosanya.</li>
               <li>Tutuplah seluruh badannya dengan kain sebagai penghormatan dan agar tidak kelihatan auratnya.</li>
               <li>Ditempatkan di tempat yang aman dari jangkauan binatang.</li>
            </ul>
         </div>
      </v-ons-card>
   </v-ons-page>
</template>

<script>
export default {
  name: 'perawatan',
  data () {
    return {
      msg: 'Perawatan Jenazah'
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
