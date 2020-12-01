<template>
  <b-container style="" >
      <p style="text-align:center;font-size:40px;margin:3%">Videos</p>
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
                    <b-th colspan="1">Matematika</b-th>
                </b-tr>
                <b-tr>
                    <b-th colspan="1">Bahasa Indonesia</b-th>
                </b-tr>
                </b-tbody>
            </b-table-simple>
        </b-col>
        <b-col cols="8">
<b-table-simple hover small responsive fixed bordered>
                <b-thead head-variant="dark">
                <b-tr>
                    <b-th colspan="1">Title</b-th>
                </b-tr>
                </b-thead>
                <b-tbody>
                <b-tr>
                    <b-th colspan="1"><nuxt-link to="/vid">Lorem, ipsum dolor.</nuxt-link></b-th>
                </b-tr>
                <b-tr>
                    <b-th colspan="1">Lorem ipsum dolor sit.</b-th>
                </b-tr>
                </b-tbody>
            </b-table-simple>
        </b-col>
    </b-row>
  </b-container>
</template>

<script>
  export default {
  }
</script>
