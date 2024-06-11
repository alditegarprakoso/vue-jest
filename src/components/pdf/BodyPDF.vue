<template>
  <div class="wrap-body">
    <table class="table-custom">
      <tr>
        <td class="text-left">No.</td>
        <td class="text-left">Detail Pekerjaan</td>
        <td class="text-right">Volume Pekerjaan</td>
        <td class="text-right">Satuan</td>
        <td class="text-right">Harga Satuan</td>
        <td class="text-right">Total Harga</td>
      </tr>
      <template v-for="item in 15">
        <tr :key="item">
          <td class="text-left">
            <p>{{ item }}</p>
          </td>
          <td class="text-left">
            <p>Area Perbaikan 1</p>
            <p>Sub Area 1</p>
            <p>Item Pekerjaan 1</p>
          </td>
          <td class="text-right">
            <p>1</p>
          </td>
          <td class="text-right">
            <p>Unit</p>
          </td>
          <td class="text-right">
            <p>Rp 1.000.000</p>
          </td>
          <td class="text-right">
            <p>Rp 1.000.000</p>
          </td>
        </tr>
        <tr v-if="item % 5 === 0" :key="item" class="wrap-total-item">
          <td class="text-left">
            <p>#</p>
          </td>
          <td>
            <p>Area Perbaikan 1</p>
            <p class="averta-bold">Total</p>
          </td>
          <td colspan="4" class="text-right">
            <p class="averta-bold">Rp 1.000.000</p>
          </td>
        </tr>
      </template>
    </table>
    <div class="wrap-total">
      <div class="wrap-price">
        <div class="wrap-sub-total">
          <p class="averta-bold text-title text-left">DPP</p>
          <p class="averta-bold">Rp 1.000.000</p>
        </div>
      </div>
      <div class="wrap-price">
        <div class="wrap-sub-total">
          <p class="averta-bold text-title text-left">PPN</p>
          <p class="averta-bold">Rp 1.000.000</p>
        </div>
      </div>
      <div class="wrap-price">
        <div class="wrap-sub-total">
          <p class="averta-bold text-title text-left">
            PPH FINAL 4 AYAT 2 <br />
            (1,75%)
          </p>
          <p class="averta-bold">Rp 1.000.000</p>
        </div>
      </div>
      <div class="wrap-price grand-total">
        <div class="wrap-sub-total">
          <p class="averta-bold text-title text-left">Grand Total</p>
          <p class="averta-black text-grand-total">Rp 1.000.000</p>
        </div>
      </div>
    </div>
    <div class="spelled-out">
      <p><i>(Terbilang: Seratus Lima Puluh Tujuh Ribu Empat Ratus Lima Puluh Rupiah)</i></p>
    </div>
  </div>
</template>

<script>
export default {
  name: "BodyPDF",
};
</script>

<style scoped>
.wrap-body {
  margin: 20px 0px 50px 0px;
  border: 1px solid #ddd;
  border-radius: 12px;
}

.text-left {
  text-align: left;
}

.text-right {
  text-align: right;
}

.table-custom {
  width: 100%;
  border-spacing: 0;
  font-size: 14px;
  padding: 0px 12px;
}

.table-custom tr:first-child td {
  padding: 30px 12px 30px 12px;
  border-bottom: 1px solid #ddd;
}

.table-custom td:not(:first-child) {
  padding: 5px 12px;
}

.wrap-total-item {
  background: #fafafa;
  border-radius: 12px;
}

.wrap-total-item td {
  padding: 0px 12px;
}

.wrap-total-item td:first-child {
  border-top-left-radius: 12px;
  border-bottom-left-radius: 12px;
}

.wrap-total-item td:last-child {
  border-top-right-radius: 12px;
  border-bottom-right-radius: 12px;
}

.wrap-price {
  display: flex;
  justify-content: end;
  align-items: center;
}

.wrap-sub-total {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0px 24px;
  width: 45%;
}

.wrap-sub-total p {
  margin: 6px 0px;
  padding: 0;
}

.grand-total {
  background: linear-gradient(90deg, #FFFFF7 100%, #FFF5EA 100%);
}

.text-grand-total {
  color: #D9272D;
}

.spelled-out {
  color:#252525;
  font-size: 12px;
  text-align: right;
  margin-right: 20px;
  padding-bottom: 20px;
}

</style>
