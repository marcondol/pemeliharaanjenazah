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
               <li>Syarat-syarat wajib memandikan jenazah
                  <ul>
                     <li>Jenazah itu orang islam. Apa pun alirannya, madzhab, ras, suku dan profesinya.</li>
                     <li>Didapati tubuhnya walaupun sedikit</li>
                     <li>Bukan mati syahid ( mati dalam peperangan untuk membela agama islam seperti yang terjadi pada masa Nabi Muhammad saw. ) </li>
                  </ul>
               </li>
               <li>Yang berhak memandikan jenazah
                  <ul>
                     <li>Apabila jenazahnya laki-laki, yang memandikannya hendaknya laki-laki. Perempuan tidak boleh memandikan jenazah laki-laki, kecuali istri dan mahramnya.</li>
                     <li>Apabila jenazah itu perempuan, hendaklah dimandikan oleh perempuan. Laki-laki tidak boleh memandikan kecuali suami atau mahramnya.</li>
                     <li>Apabila jenazah itu seorang istri, sementara suami dan mahramnya ada semua, suami lebih berhak untuk memandikan istrinya.</li>
                     <li>Apabila jenazah itu seorang suami, sementara istri dan mahramnya ada semua, istri lebih berhak untuk memandikan suaminya.</li>
                     <li>Kalau jenazah anak laki-laki masih kecil, perempuan boleh memandikannya. Begitu juga kalau jenazah perempuan masih kecil, laki-laki boleh memandikannya.</li>
                  </ul>
               </li>
               <li>
                  Tata cara memandikan jenazah :
                  <ul>
                     <li>Di tempat tertutup agar yang melihatnya hanya orang-orang yang memandikan dan yang mengurusnya saja.</li>
                     <li>Jenazah diletakkan di tempat yang tinggi seperti dipan.</li>
                     <li>Dipakaikan kain basahan seperti sarung agar auratnya tidak terbuka</li>
                     <li>Jenazah disandarkan pada sesuatu, lantas disapu perutnya sambil ditekan pelan-pelan agar semua kotorannya keluar, lantas dibersihkan dengan tangan kirinya. Dianjurkan mengenakan sarung tangan. Dalam hal ini boleh memakai wangi-wangian agar tidak terganggu bau kotoran si mayyit/jenazah.</li>
                     <li>Setelah itu hendaklah mengganti sarung tangan untuk membersihkan mulut dan gigi jenazah</li>
                     <li>Membersihkan semua kotoran dan najis</li>
                     <li>Mewudhukan, setelah itu membasuh seluruh badannya</li>
                     <li>Disunnahkan membasuh 3 sampai 5 kali.</li>
                  </ul>
               </li>
                  Air untuk memandikan jenazah sebaiknya dingin. Kecuali udara sangat dingin atau ada kotoran yang sulit dihilangkan, boleh menggunakan air hangat.
            </ol>
         </div>
      </v-ons-card>
      <v-ons-card>
         <video width="320" height="240" controls>
           <source src="../assets/vid/mandi_pria.mp4" type="video/mp4">
         </video>
         <video width="320" height="240" controls>
           <source src="../assets/vid/mandi_wanita.mp4" type="video/mp4">
         </video>
      </v-ons-card>
   </v-ons-page>
</template>

<script>
export default {
  name: 'memandikan',
  data () {
    return {
      msg: 'Memandikan Jenazah'
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
