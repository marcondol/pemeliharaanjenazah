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
            <p>Ta’ziyyah atau melayat adalah mengunjungi orang yang sedang tertimpa musibah kematian salah seorang keluarganya dalam rangka menghibur atau memberi semangat. Para mu’azziyin ( orang laki-laki yag ber-ta’ziyyah ) atau mu’aziyyat ( orang perempuan yang ber-ta’ziyyah ) hedaknya memberikan dorongan kekuatan mental atau menasihati agar orang yang tertimpa musibah tetap sabar dan tabah menghadapi musibah ini. Umayah ra. mengatakan ini bahwa anak perempua Rasulullah saw.menyuruh seseorang untuk memanggil dan memberi tahu beliau bahwa anaknya dalam keadaan hampir mati. Lalu beliau bersabda, kembalilah engkau kepadanya. Katakan bahwa segala yag diambil dan yang diberikan, bahkan apapun yang ada dihadapan kita kepunyaan Allah. Dialah yang menentukan ajalnya, maka suruhlah ia sabar dan tunduk kepada perintah.” (HR. Bukhari Muslim )</p>
            <p>Adab ( etika ) orang ber-ta’ziyyah antara lain seperti berikut :</p>
            <ul>
               <li>Menyampaikan do’a untuk kebaikan dan ampunan terhadap orang yang meninggal serta kesabaran bagi orang yang ditinggal.</li>
               <li>Hindarilah pembicaraan yang menambah sedih keluarga yang ditimpa musibah</li>
               <li>Hindarilah canda tawa apalagi sampai terbahak bahak</li>
               <li>Usahakan turut menyalati mayat dan turut mengantarkan ke pemakaman sampai selesai penguburan</li>
               <li>Membuatkan makanan bagi keluarga yang ditimpa musibah</li>
            </ul>
            <p>Demikian diperintahkan Rasulullah saw. kepada keluarganya sewaktu keluarga Ja’far ditimpa kematian ( HR. Lima ahli hadits kecuali Nasai )</p>

         </div>
      </v-ons-card>
   </v-ons-page>
</template>

<script>
export default {
  name: 'taziah',
  data () {
    return {
      msg: 'Taziah'
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
