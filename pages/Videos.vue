<template>
<div style="margin:10%">
    <p style="text-align:center;font-size:40px;margin:3%">Videos</p>
  <b-container>
    <b-row class="justify-content-md-center">
        <b-col cols="4">
<b-table-simple hover small responsive bordered fixed >
                <b-thead head-variant="dark">
                <b-tr>
                    <b-th colspan="1">Matapelajaran</b-th>
                </b-tr>
                </b-thead>
                <b-tbody>
                <b-tr>
                    <b-th colspan="1"><b-button pill variant="outline-secondary" @click="Matpel = 'Matematika' " >Matematika</b-button></b-th>
                </b-tr>
                <b-tr>
                    <b-th colspan="1"><b-button pill variant="outline-secondary" @click="Matpel = 'BahasaIndonesia' " >Bahasa Indonesia</b-button></b-th>
                </b-tr>
                <b-tr>
                    <b-th colspan="1"><b-button pill variant="outline-secondary" @click="Matpel = 'Biologi' " >Biologi</b-button></b-th>
                </b-tr>
                </b-tbody>
            </b-table-simple>
        </b-col>
        <b-col cols="8" v-if="Matpel === 'Matematika'">
<b-table-simple hover small responsive fixed bordered>
        <b-thead head-variant="dark">
                <b-tr>
                    <b-th colspan="1">Title</b-th>
                </b-tr>
                </b-thead>
                <b-tbody>
                <b-tr>
                    <b-th colspan="1"><nuxt-link to="/vid">Matematika 1</nuxt-link></b-th>
                </b-tr>
                <b-tr>
                    <b-th colspan="1">Matematika 2</b-th>
                </b-tr>
                </b-tbody>
            </b-table-simple>
        </b-col>
        <b-col cols="8" v-else-if="Matpel === 'BahasaIndonesia'">
<b-table-simple hover small responsive fixed bordered>
        <b-thead head-variant="dark">
                <b-tr>
                    <b-th colspan="1">Title</b-th>
                </b-tr>
                </b-thead>
                <b-tbody>
                <b-tr>
                    <b-th colspan="1"><nuxt-link to="/vid">Bahasa Indonesia</nuxt-link></b-th>
                </b-tr>
                <b-tr>
                    <b-th colspan="1">Bahasa Indo</b-th>
                </b-tr>
                </b-tbody>
            </b-table-simple>
        </b-col>
        <b-col cols="8" v-else-if="Matpel === 'Biologi'">
<b-table-simple hover small responsive fixed bordered>
        <b-thead head-variant="dark">
                <b-tr>
                    <b-th colspan="1">Title</b-th>
                </b-tr>
                </b-thead>
                <b-tbody>
                <b-tr>
                    <b-th colspan="1"><nuxt-link to="/vid">Biologi 1</nuxt-link></b-th>
                </b-tr>
                <b-tr>
                    <b-th colspan="1">Biologi 2</b-th>
                </b-tr>
                </b-tbody>
            </b-table-simple>
        </b-col>
        <b-col cols="8" v-else>
<b-table-simple hover small responsive fixed bordered>
        <b-thead head-variant="dark">
                <b-tr>
                    <b-th colspan="1">Title</b-th>
                </b-tr>
                </b-thead>
                <b-tbody>
                <b-tr>
                    <b-th colspan="1">Pilih Matepelajaran</b-th>
                </b-tr>
                </b-tbody>
            </b-table-simple>
        </b-col>
    </b-row>
  </b-container>
  </div>
</template>

<script>
  export default {
      data() {
      return {
        Matpel: true
      }
      }
  }
</script>
