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
      <v-ons-list-title><h3>Membuka Relung Hati</h3></v-ons-list-title>
      <v-ons-card>
         <div>
            <p>Hidup di dunia ini tidaklah selamanya. Akan datang masanya kita berpisah dengan dunia berikut isinya. Perpisahan itu terjadi saat kematian menjemput. Kematian adalah pintu dan setiap manusia akan memasuki pintu itu, tanpa ada seorang pun yang dapat menghindar darinya.</p>
            <p>كل نفس ذائقة الموت.....</p>
            <p>Artinya : Tiap-tiap yang bernyawa akan merasakan mati. ( QS. Ali Imran/3:185 )</p>
            <p>Ayat di atas menjelaskan bahwa setiap yang bernyawa pasti akan mati. Kita juga akan mati sebab kita ini manusia yang memiliki nyawa. Kematian datang tidak pernah pilih-pilih. Apabila ajal datang, tidak ada satu kekuatan pun yang mempercepat atau memperlambat. Ada kalanya kematian itu mejemput saat masih bayi, kanak-kanak, remaja, dewasa bahkan orang yang sudah tua renta.</p>
            <p>Kadang ia menjemputnya saat manusia sedang tidur, terjaga, sedang sedih, sednag bahagia, sedang sendiri dan sedang bersama. Kematian datang tidak pernah ada yang tahu. Oleh karena itu, mengigat mati harus sering dilakukan agar manusia menyadari bahwa dirinya tidak akan hidup kekal. Salah satu cara untuk mengigat mati adalah sering-sering ber-ta’ziyyah, mengurus jenazah, mulai dari memandikan, mengafani, menyalati sampai menguburnya.</p>
            <p>Seorang putra dari sahabat yang mulia Abdullah bin Umar ra. mengabarkan, aku sedang duduk bersama Rasulullah saw. Tatkala datang seorang laki-laki dari kalangan Anshar. Ia mengucapkan salam kepada Rasulullah saw. lalu berkata, “ Ya Rasulullah, mu’min manakah yang paling utama ?” Beliau menjawab, yag paling baik akhlaknya di antara mereka.”, ”mu’min manakah yang paling cerdas ?” tanya lelaki itu lagi. Beliau mejawab : “ orag yang paling banyak mengingat mati dan paling baik persiapannya untuk kehidupan setelah mati. Mereka itulah orang-orang yang cerdas.” ( HR. Ibnu Majah )</p>
         </div>
      </v-ons-card>
   </v-ons-page>
</template>

<script>
export default {
  name: 'home',
  data () {
    return {
      msg: 'Selamat Datang'
    }
  },
  methods: {
    goTo (url) {
      window.open(url, '_blank')
    }
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
