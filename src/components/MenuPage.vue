<template>
  <v-ons-page>
    <v-ons-toolbar modifier="transparent"></v-ons-toolbar>
    <div class="header">
      <img src="../assets/logo.jpg">
    </div>

    <v-ons-list-title>Menu </v-ons-list-title>
    <v-ons-list>
      <v-ons-list-item modifier="chevron" v-for="item in essentialLinks" @click="itemClicked(item.page)" :key="item.link">
        <div class="left"><v-ons-icon fixed-width :icon="item.icon"></v-ons-icon></div>
        <div class="center">{{ item.label }}</div>
      </v-ons-list-item>
    </v-ons-list>
  </v-ons-page>
</template>

<script>
export default {
  name: 'menu',
  data () {
    return {
      essentialLinks: [
        {
            label: 'Membuka Relung Hati',
            icon: 'fa-graduation-cap',
            page:"home"
        },
        {
            label: 'Perawatan Jenazah',
            icon: 'fa-graduation-cap',
            page: "perawatan"
        },
        {
            label: 'Memandikan Jenazah',
            icon: 'fa-graduation-cap',
            page: "memandikan"
        },
        {
            label: 'Mengkafani Jenazah',
            icon: 'fa-graduation-cap',
            page: "mengkafani"
        },
        {
            label: 'Menyalati Jenazah',
            icon: 'fa-graduation-cap',
            page: "menyalatkan"
        },
        {
            label: 'Menguburkan Jenazah',
            icon: 'fa-graduation-cap',
            page: "menguburkan"
        },
        {
            label: 'Taziah',
            icon: 'fa-graduation-cap',
            page: "taziah"
        },
        {
            label: 'Ziarah Kubur',
            icon: 'fa-graduation-cap',
            page: "ziarah"
        },
        {
            label: 'Rangkuman',
            icon: 'fa-graduation-cap',
            page: "rangkuman"
        },
        {
            label: 'Soal-soal',
            icon: 'fa-graduation-cap',
            page: "soal"
        }

      ]
    }
  },
  methods: {
    itemClicked(page_id){
       console.log('dalam', page_id);
       this.$emit('menuclicked', page_id);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header {
  text-align: center;
  margin-bottom: 20px;
}

img {
  max-width: 150px;
}

ons-list-title {
  text-transform: none;
}

ons-list-item {
  cursor: pointer;
}
</style>
