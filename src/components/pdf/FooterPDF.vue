<template>
  <div class="wrap-footer">
    <div class="wrap-instruksi">
      <p class="averta-bold fs-16">Instruksi Pembayaran</p>
      <ul class="fs-14 dot-list">
        <li>
          Pembayaran maksimal dilaksanakan 14 hari terhitung dari tanggal
          penerimaan tagihan.
        </li>
        <li>Pembayaran dapat ditransfer ke rekening:</li>
      </ul>
      <div class="rekening-wrapper">
        <p class="averta-bold fs-16">PT. Tenaga Kanggo Indonesia</p>
        <p>BCA KCU Serpong</p>
        <p>No Rekening: <span class="averta-bold">4978888397</span></p>
      </div>
    </div>
    <div>
        <p class="averta fs-14 mb-ttd">Dibuat Oleh,</p>
        <p class="averta fs-14">
            <u class="averta-bold">Nita</u>
            <br>
            <span>(Finance)</span>
        </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterPDF",
};
</script>

<style scoped>

.dot-list {
  list-style-type: disc;
}

.wrap-instruksi {
  margin-bottom: 50px;
}

.rekening-wrapper {
  padding: 4px 12px;
  background: #fafafa;
  border-radius: 12px;
  margin: auto;
  width: 95%;
}

.mb-ttd {
  margin-bottom: 120px;
}

</style>
