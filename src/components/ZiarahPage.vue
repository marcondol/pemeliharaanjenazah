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
            <p>Ziarah artinya berkunjung, kubur artinya kuburan. </p>
            <p>Ziarah kubur artinya berkunjung ke kuburan. </p>
            <p>Awalnya Rasulullah saw. melarang umat islam untuk berziarah kubur karena dihawatirkan akan melakukan sesuatu hal yang tidak baik, misalnya menangis diatas kuburan, bersedih, meratapi, bahkan yang lebih berbahaya adalah mengultuskan mayat yang ada di kuburan. Aka tetapi, karena mengingat mati itu penting, dan diantara mengingat mati adalah ziarah kubur, Rasulullah saw. menganjurkan berziarah dengan tujuan megingat mati. Rasulullah saw. bersabda :
            عن أبي بريدة قال قال رسول الله صلى الله عليه وسلم إني كنت نهيتكم عن زيارة القبورفزورها ( رواه النسائ )
            Artinya : Dari Abdullah bin buraidah berkata, Rasulullah saw. bersabda : “ aku pernah melarang kalian berziarah kubur, maka sekarang berziarahlah kalian ke kubur.” ( HR. Nasa’i )
            </p>
            <p>Diantara hikmah dari ziarah kubur ini antara lain sebagai berikut :</p>
            <ul>
               <li>Mengingat kematian</li>
               <li>Dapat bersikap zuhud ( menjauhkan diri dari sifat keduniawian )</li>
               <li>Selalu ingin berbuat baik sebagai bekal kelak di alam kubur dan hari akhir</li>
               <li>Medoakan si mayat yang muslim agar diampuni dan diberi kesejahteraan di akhirat</li>
            </ul>
            <p>Apabila kita mau berziarah kubur, sebaiknya perhatikan adab atau etika berziarah kubur, yaitu sebagai berikut.</p>
            <ul>
               <li>Ketika mau berziarah, niatkan dengan ikhlas karena Allah swt, tunduk hati dan merasa diawasi oleh Allah.</li>
               <li>Sesampai di pintu kuburan, ucapkan salam sebagaimana yang diajarkan oleh Rasulullah saw.
                 السلام عليكم يا أهل القبور فإنا ان شاء الله بكم لاحقون ( رواه الترميذي )
               </li>
               <li>Artinya : “ keselamatan semoga tetap bagimu wahai ahli kubur dan insya Allah kami akan bertemu dengan kamu semua. ( HR. Tarmidzi )  </li>
               <li>Tidak banyak bicara mengenai urusan dunia diatas kuburan</li>
               <li>Berdoa untuk ampunan dan kesejahteraan si mayat di alam barzah dan akhirat kelak</li>
               <li>Diusahakan tidak berjalan melangkahi kuburan atau menduduki nisan ( tanda kuburan )</li>
            </ul>
            <p>Menerapkam perilaku mulia
               Kita sebagai muslim harus peduli dengan orang lain, terutama yag berada di sekitar kita. Ketika ada orang yang meninggal atau musibah lainnya, selayaknya kita harus memperlihatkan perilaku-perilaku mulia. Perilaku mulia yang dimaksud antara lain seperti berikut :
            </p>
            <ul>
               <li>Segera mengunjungi keluarga yag terkena musibah, mendoakan mayat, mengucapkan turut berduka kepada keluarga yang ditinggalkan.</li>
               <li>Membantu persiapan pengurusan jenazah seperti memandikan, mengafani, menyalati dan meguburkan.</li>
               <li>Memberikan bantuhan kepada keluarga korban untuk memperingan bebannya sesuai kemampuan kita.</li>
               <li>Menghibur keluarga korban dengan ungkapan-ungkapan optimistis dan nasihat tentang kesabaran dan ketabahan.</li>
            </ul>
         </div>
      </v-ons-card>
   </v-ons-page>
</template>

<script>
export default {
  name: 'ziarah',
  data () {
    return {
      msg: 'Ziarah'
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
