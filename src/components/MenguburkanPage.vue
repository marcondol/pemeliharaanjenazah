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
            <ul>
               <li>Perihal mengubur jenazah ada beberapa penjelasan sebagai berikut :
                     Rasulullah saw. Menganjurkan agar jenazah segera dikuburkan, sesuai sabdanya :
                     عن أبي هريرة رضي الله عنه عن النبي صلى الله عليه وسلم قال أسرعوا بالجنازة ( روه البخاري ومسلم )
                  Artinya : “ dari abu hurairoh ra. Dari Nabi Muhammad saw. bersabda : segerakanlah menguburkan jenazah… “ (H.R. Bukhari dan Muslim )
               </li>
               <li>Sebaiknya mennguburkan jenazah pada siang hari. Megubur jenazah pada malam hari diperbolehkan apabila dalam keadaan terpaksa seperti bau yang sangat menyengat meskipun sudah diberi wangi-wangian atau karena sesuatu hal lain yang harus disegerakan untuk dikubur.</li>
               <li>Anjuran meluaskan lubag kubur. Rasulullah saw. pernah mengantar jenazah sampai di kuburnya. Lalu beliau duduk di tepi lubang kubur, dan bersabda, Luaskanlah pada bagian kepala, dan luaskanlah pula pada bagian kaki, ada beberapa kurma baginya di surge( HR. Ahmad dan Abu Dawud ).</li>
               <li>Boleh meguburkan dua/tiga jenazah dalam satu liang kubur. Hal itu dilakukan sewaktu selesai perang uhud.  Rasulullah saw. bersabda : “ galilah dan dalamkanlah. Baguskanlah dan masukkanlah dua atau tiga orang di dalam satu liang kubur. Dahulukalah orang yang paling banyak hafal al qur’an ( H.R. Nasai dan Tirmidzi dan Hisyam bin Amir ra ).</li>
               <li>Bacaan meletakkan mayit dalam kubur. Apabila meletakkan mayyit dalam kubur, Rasulullah saw. membaca :
               بسم الله وعلى ملة رسول الله
               Artinya : Dengan nama Allah dan agama Rasulullah.

               بسم الله وعلى ملة رسول الله وعلى سنة رسول الله
               Artinya : Dengan nama Allah dan agama Rasulullah dan atas nama sunnah Rasulullah”. ( HR. Lima ahli hadits kecuali Nasai dan Ibu Umar ra ).
               </li>
               <li> Larangan memperindah kuburan. Jabir ra. menerangkan, “ Rasulullah saw. melarang mengecat kuburan, duduk, dan membuat bangunan di atasnya. “ ( HR. Muslim )</li>
               <li>Sebelum dikubur, ahli waris atau keluarga hendaklah bersedia menjadi penjamin atau menyelesaikan atas hutang hutang si mayat jika ada, baik dari harta yang ditinggalkannya atau dari sumbangan keluarganya. Nabi Muhammad saw. bersabda : “  diri orang mu’min itu tergantung ( tidak sampai ke hadirat Tuhan ) karena hutangnya, sampai dibayar dulu hutangnya itu ( oleh keluarganya ).” ( HR. Ahmad dan Tirmidzi dari Abu Hurairah ra. )  </li>
            </ul>
         </div>
      </v-ons-card>
      <v-ons-card>
         <video width="320" height="240" controls>
           <source src="../assets/vid/menguburkan.mp4" type="video/mp4">
         </video>
      </v-ons-card>
   </v-ons-page>
</template>

<script>
export default {
  name: 'menguburkan',
  data () {
    return {
      msg: 'Menguburkan Jenazah'
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
