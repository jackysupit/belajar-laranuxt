<template>
  <div class="row">
      List Pegawai:
        {{listPegawai}}

      <p class="kotak-pink" v-for="(pegawai, index) in listPegawai">
        <div>No: {{index+1}}</div>
        <div>Nama: {{pegawai.nama}}</div>
        <div>Jenis Kelamin: {{pegawai.jenisKelamin}}</div>
      </p>
  </div>
</template>

<script setup lang="ts">
  const listPegawai = [
    {
      "nama": "Andi",
      "jenisKelamin": 1,
    },
    {
      "nama": "Budi",
      "jenisKelamin": 1,
    },
    {
      "nama": "Chintya",
      "jenisKelamin": 2,
    },
    {
      "nama": "Diana",
      "jenisKelamin": 4,
    },
  ]
</script>
<style scoped>
.kotak-pink {
  width: 340px;
  height: 120px;
  padding: 20px;
  margin: 5px;
  float:left;
  color: black;
  background: pink;
  display: block;
}
</style>
