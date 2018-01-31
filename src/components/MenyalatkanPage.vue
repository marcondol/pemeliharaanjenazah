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
            <p>Orang yang meninggal dunia dalam keadaan islam berhak untuk di-shalatkan. </p>
            <p>Sabda Rasulullah saw. “ Shalatkanlah orang-orang yang telah mati.” ( HR. Ibnu Majah ). Shalatkanlah olehmu orang-orang yang mengucapkan : “ Lailaaha Illallah “ ( HR. Daruqutni ). Dengan demikian,  jelaslah bahwa orang yang berhak dishalati ialah orang yang meninggal dunia dalam keadaan beriman kepada Allah swt. </p>
            <p>Adapun orang yang telah murtad dilarang untuk dishalati.</p>
            <p>Untuk bisa dishalati, keadaan si mayat haruslah :</p>
            <ul>
               <li>Suci, baik badan, tempat dan pakaian</li>
               <li>Sudah dimandikan dan dikafani</li>
               <li>Jenazah sudah berada di depan orang yang menyalatkan atau sebelah kiblat.  </li>
            </ul>
            <p>Tata cara pelaksanaan shalat jenazah adalah sebagai berikut :</p>
            <ul>
               <li>Jenazah diletakkan paling muka. Apabila mayat laki-laki, hendaknya imam berdiri menghadap dekat kepala mayat. Jika mayat wanita, imam menghadap dekat perutnya.<li>
               <li>Letak imam paling muka diikuti oleh para makmum. Jika yang menyalati sedikit, usahakan dibuat 3 baris/saf.</li>
               <li>Mula-mula semua jamaah berdiri dengan berniat melakukan shalat jenazah dengan empat takbir.
               Niat tersebut jika dilafalkan sebagai berikut :
               أصلي على هذا الميت ( هذه الميتة ) اربع تكبيرات فرض كفاية مأموما لله تعالى
               Artinya : “ Aku berniat salat atas jenazah ini empat takbir fardlu kifayah sebagai makmum karena Allah ta’ala”.</li>
               <li>Kemudian takbirotul ihram yang pertama, dan setelah takbir pertama itu selanjutnya membaca surat al-fatihah.</li>
               <li>Takbir yang kedua, dan setelah itu, membaca shalawat atas Nabi Muhammad saw.

                  اللهم صل على سيدنا محمد وعلى ال سيدنا محمد
               </li>
               <li>Takbir yang ketiga kemudian membaca doa untuk jenazah. Bacaan doa bagi jenazah adalah sebagai berikut :

                  اللهم اغفرله ( ها ) وارحمه ( ها ) وعافه ( ها ) واعف عنه ( ها )

                  Artinya : “ ya Allah, ampunilah ia, kasihanilah ia, sejahterakanlah ia, maafkanlah kesalahannya. “
               </li>
               <li>Takbir keempat, dilanjutkan dengan membaca doa sebagai berikut :
                  اللهم لاتحرمنا أجره ( ها ) ولاتفتنا بعده ( ها ) واغفر له ( ها )
                  Artinya : “ ya Allah, janganlah engkau menjadikan kami penghalang dari mendapatkan pahalanya dan janganlah engkau beri kami fitnah sepeninggalnya, dan ampunilah kami dan dia.” ( HR. Hakim )
               </li>
               <li>Membaca salam sambil menoleh ke kanan dan ke kiri.</li>
            </ul>
         </div>
      </v-ons-card>
      <v-ons-card>
         <video width="320" height="240" controls>
           <source src="../assets/vid/menshalatkan.mp4" type="video/mp4">
         </video>
      </v-ons-card>
   </v-ons-page>
</template>

<script>
export default {
  name: 'menyalatkan',
  data () {
    return {
      msg: 'Menyalatkan Jenazah'
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
