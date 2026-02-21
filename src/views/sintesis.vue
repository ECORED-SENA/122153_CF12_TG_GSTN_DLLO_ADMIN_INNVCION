<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    p.mb-4 El siguiente mapa integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo.
    
    .row.justify-content-center
      .col-lg-9.mb-5
        figure
          img(src="@/assets/curso/temas/sintesis.svg", alt="A continuación, se presenta la síntesis del componente formativo: Toma de decisiones: para llegar a ella se necesita los estándares de calidad, posteriormente un diagnostico con sus acciones, contingencias, seguimientos y mejoramiento, esto lleva a la administración estratégica con informes organizacionales y finalmente la toma de decisiones de la mano de modelos gerenciales y estructuras administrativas.")
    .row.justify-content-center  
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
