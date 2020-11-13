<template>
  <div>
    <navbar />
    <parallax
      :img="parallaxImg"
      :title="parallaxTitle"
      :caption="parallaxCaption"
    />
    <v-container id="posts">
      <v-row>
        <v-col
          cols="12"
          sm="8"
        >
          <v-row>
            <v-col
              v-for="i in 8"
              :key="i"
              cols="12"
              sm="6"
            >
              <lazy-content-card :data="post" />
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>

export default {
  data: () => ({
    post: {
      img: 'https://1.bp.blogspot.com/-O0qfJkCQSsg/X1cQvjDaeFI/AAAAAAAAAXA/lAyCiQ19ItQ1hJv98Zp2ZHpOjLtRSku2ACLcBGAsYHQ/s400/1.jpg',
      tag: 'Banjarmasin',
      creator: 'Admin RSUDSS',
      title: 'RSUD Sultan Suriansyah resmi memiliki Laboratorium Polymerase Chain Reaction (PCR)',
      createdAt: 'September 08, 2020',
      content: 'RSUD Sultan Suriansyah resmi memiliki laboratorium Polymerase Chain Reaction (PCR) \n (Banjarmasin, 01/09/2020) Kini Rumah Sakit Sultan Suriansyah Banjarmasin telah memiliki Laboratorium Polymerase Chain Reaction (PCR) yang telah diresmikan pada tanggal tanggal 1 September 2020. Acara peresmian Laboratorium (PCR) tersebut dilakukan oleh Wali Kota Banjarmasin, Bapak H. Ibnu Sina, S.Pi., M.Si yang dihadiri oleh Kepala Dinas Kesehatan Kota Banjarmasin, Bapak Dr. Machli Riyadi, SH., MH. Serta jajaran pejabat tinggi di lingkungan Pemerintah Kota Banjarmasin.',
      link: '/aa'
    },
    parallaxImg: 'https://kanalkalimantan.com/wp-content/uploads/2020/07/WhatsApp-Image-2020-07-02-at-14.23.43.jpeg',
    parallaxTitle: 'RSUD Sultan Suriansyah',
    parallaxCaption: 'Rumah Sakit Umum Daerah Sultan Suriansyah',

  }),
  computed: {
    //
  },
  methods: {
    //
  }
}
</script>
