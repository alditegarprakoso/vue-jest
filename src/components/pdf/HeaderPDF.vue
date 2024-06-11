<template>
    <div class="wrap-header">
        <div class="letter-head">
            <img src="@/assets/images/logo.png" alt="logo" class="logo">
            <div class="invoice-header">
                <p class="invoice-title averta-black">INVOICE</p>
                <p class="date averta">Tanggal Terbit: -</p>
                <p class="due-date averta">Jatuh Tempo: -</p>
            </div>
        </div>
        <div class="mailing-address">
            <div class="to">
                <p class="averta fs-14 text-secondary">Kepada Yth:</p>
                <p class="text-branch averta-bold">Branch Manager Alfamart Tangsel</p>
                <p class="averta fs-14 text-secondary">Alfamart BSD</p>
            </div>
            <div class="address">
                <p class="averta fs-14 text-secondary">Alamat</p>
                <p class="text-address averta">Jl. BSD Raya Utama Desa Sampora, Kecamatan Cisauk, Tangerang 15345 Indonesia</p>
            </div>
        </div>
        <div class="id-survey">
            <p><span class="averta-bold">Alfamart BSD | </span><span>IDSURVEY01</span></p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HeaderPDF'
}
</script>

<style scoped>

.letter-head {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 25px;
}

.letter-head .logo {
    height: 35px;
}

.letter-head .invoice-header {
    text-align: left;
    margin-right: 80px;
}

.invoice-header .invoice-title {
    font-size: 24px;
    color: #3185FC;
}

.invoice-header .date, .invoice-header .due-date {
    color: #868686;
    font-size: 14px;
}

.mailing-address {
    display: flex;
    justify-content: space-between;
    padding: 0px 12px;
    border-radius: 12px;
    background: #3185FC1A;
}

.mailing-address .to {
    width: 50%;
}

.mailing-address .address {
    width: 50%;
}

.to .text-branch {
    margin: -5px 0px;
}

.address .text-address {
    color: #252525;
    margin: -5px 0px;
}

.id-survey {
    background: #3185FC1A;
    border: 3px solid #3185FC;
    border-radius: 12px;
    padding: 12px;
    margin: 24px 0px;
}

.id-survey p {
    padding: 0px;
    margin: 0px;
}

</style>