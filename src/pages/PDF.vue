<template>
  <div>
    <div id="wrap-pdf">
      <HeaderPDF />
      <BodyPDF />
      <FooterPDF />
    </div>
  </div>
</template>

<script>
import HeaderPDF from "@/components/pdf/HeaderPDF.vue";
import BodyPDF from "@/components/pdf/BodyPDF.vue";
import FooterPDF from "@/components/pdf/FooterPDF.vue";

export default {
  name: "PDF",
  components: {
    HeaderPDF,
    BodyPDF,
    FooterPDF,
  },
  mounted() {
    window.document.title = "PDF";
  }
};
</script>

<style scoped>

#wrap-pdf {
  width: 210mm;
  margin: auto;
  padding: 30px;
  background: white;
}

</style>
