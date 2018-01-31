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
      <v-ons-list-title><h3>Soal-soal</h3></v-ons-list-title>
      <v-ons-card>
         <div>
            <p>A.	Berilah tanda silang ( X) pada huruf a, b, c, d, atau e yang dianggap sebagai jawaban yang palig tepat !</p>
            <p>1.	Perhatikan pernyataan-pernyataan berikut !</p>
               <p>&nbsp &nbsp a)	Jenazah laki-laki sebaiknya dibungkus dengan tiga helai kain kafan, dan wanita dengan lima helai</p>
               <p>&nbsp &nbsp b)	Jika jenazahnya laki-laki hedaknya orang yang mengafaninya juga laki-laki</p>
               <p>&nbsp &nbsp c)	Tiap helai kain kafan dihamparkan di atas tikar dan diberi harum-haruman</p>
               <p>&nbsp &nbsp d)	Jenazah diletakkan di atas kain kafan dengan posisi tangan diangkat seperti sedang takbir ihram</p>
               <p>&nbsp &nbsp e)	Seluruh tubuh jenazah dibalut dengan kain kafan kecuali muka dibiarkan terbuka</p>
            <p>Dari pernyataan tersebut, mana pernyataan yang termasuk ketentuan syari’at dalam mengafani jenazah ?</p>
               <p>&nbsp &nbsp a.	( a,b dan d )</p>
               <p>&nbsp &nbsp b.	( b,c dan e )</p>
               <p>&nbsp &nbsp c.	( a,b,d dan e )</p>
               <p>&nbsp &nbsp d.	( a,b dan c )</p>
               <p>&nbsp &nbsp e.	( c,d dan e )</p>
            <p>2.	Perhatikan pernyataan berikut.</p>
               <p>&nbsp &nbsp 1)	Yang shalat jenazah harus orang muslim</p>
               <p>&nbsp &nbsp 2)	Merendahkan suara bacaan ketika shalat</p>
               <p>&nbsp &nbsp 3)	Shalat jenazah dilakukan setelah jenazah dimandikan</p>
               <p>&nbsp &nbsp 4)	Membaca surah setelah al fatihah</p>
               <p>&nbsp &nbsp 5)	Letak jenazah di sebelah qiblat dari yang menyalatkan</p>
            <p>Dari pernyataan-pernyataan tersebut, pernyataan yang termasuk syarat-syarat sah shalat jenazah adalah…</p>
               <p>&nbsp &nbsp a.	1,2, dan 3</p>
               <p>&nbsp &nbsp b.	1,3, dan 5</p>
               <p>&nbsp &nbsp c.	3,4, dan 5</p>
               <p>&nbsp &nbsp d.	1,2, dan 4</p>
               <p>&nbsp &nbsp e.	2,3, dan 4</p>
            <p>3.	Salah satu ucapan doa dalam shalat jenazah berbunyi :</p>
            <p>  اللهم اغفرله ( ها ) وارحمه ( ها ) وعافه ( ها ) واعف عنه ( ها )</p>
            <p>Artinya…..</p>
               <p>&nbsp &nbsp a.	Gantikanlah rumahnya, dengan yang lebih baik dari rumahnya ketika di dunia</p>
               <p>&nbsp &nbsp b.	Gantikanlah kaum keluarganya dari kaum keluarganya dahulu</p>
               <p>&nbsp &nbsp c.	Ampunilah segala dosanya yang telah lalu</p>
               <p>&nbsp &nbsp d.	Ya Allah, ampunilah ia, kasihinilah ia, sejahterakanlah ia, maafkanlah kesalahannya.</p>
               <p>&nbsp &nbsp e.	Periharalah dia dari siksa kubur dan azab neraka</p>
            <p>4.	Perhatikan pernyataan-pernyataan berikut :</p>
               <p>&nbsp &nbsp 1)	Seorang muslimah tidak boleh menyalatkan jenazah laki-laki muslim</p>
               <p>&nbsp &nbsp 2)	Bila jenazahnya laki-laki, letak imam shalat jenazah sejajar dengan kepala jenazah</p>
               <p>&nbsp &nbsp 3)	Laki-laki muslim tidak boleh menyalatkan jenazah wanita muslimah</p>
               <p>&nbsp &nbsp 4)	Bila jenazahnya wanita, letak imam salat jenazah sejajar dengan dengan bagian tengah badan jenazah</p>
               <p>&nbsp &nbsp 5)	Salat jenazah gaib harus meghadap dimana jenazah itu dimakamkan</p>
            <p>Dari pernyataan-pernyataan tersebut, pernyataan yang termasuk ke dalam ketentuan syari’at tentang salat jenazah adalah…</p>
               <p>&nbsp &nbsp a.	1 dan 2</p>
               <p>&nbsp &nbsp b.	2 dan 3</p>
               <p>&nbsp &nbsp c.	3 dan 4</p>
               <p>&nbsp &nbsp d.	2 dan 4</p>
               <p>&nbsp &nbsp e.	1, 3 dan 5</p>
            <p>5.	Berikut ini termasuk perbuatan-perbuatan sunah pada waktu pemakaman, kecuali…</p>
               <p>&nbsp &nbsp a.	Meninggikan kubur sekadarnya</p>
               <p>&nbsp &nbsp b.	Menandai kubur dengan batu atau kayu</p>
               <p>&nbsp &nbsp c.	Menaruh kerikil di atas kubur</p>
               <p>&nbsp &nbsp d.	Menyiram kubur dengan air</p>
               <p>&nbsp &nbsp e.	Penguburan jenazah sebaiknya jangan disegerakan</p>
            <p>B.	Jawablah soal-soal berikut dengan benar dan tepat !</p>
               <p>&nbsp &nbsp 1.	Mengapa Rasulullah saw. Menyebutkan bahwa, “ mu’min yang paling banyak mengingat mati dan yang paling baik persediaannya untuk hidup setelah mati adalah mu’min yang paling cerdik ? Jelaskan !</p>
               <p>&nbsp &nbsp 2.	Sebutkan hal-hal yang sebaiknya segera dilaksanakan terhadap jenazah yang baru saja meinggal sebelum jenazahnya dimandikan !</p>
               <p>&nbsp &nbsp 3.	Apa yang dimaksud dengan ta’ziyyah ? kemukakan pula hukumnya, alasan hukumnya, dan adab-adabnya !</p>
               <p>&nbsp &nbsp 4.	Jika orang yang meninggal dunia meninggalkan hutang, bagaimana hukum melunasinya dan harta siapa yang digunakan untuk melunasi hutangnya ?</p>
               <p>&nbsp &nbsp 5.	Memandikan, mengafani, menyalatkan, dan menguburkan jenazah seorang muslim hukumnya adalah fardlu kifayah. Jelaskan maksudnya !</p>
         </div>
      </v-ons-card>
   </v-ons-page>
</template>

<script>
export default {
  name: 'soal',
  data () {
    return {
      msg: 'Soal - Soal'
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
