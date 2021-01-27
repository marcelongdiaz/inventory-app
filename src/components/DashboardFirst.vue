<template>
  <div class="table cstm-container cstm-container-req">
      <div class="table-header cstm-dashboard-table">
        <h3 class="text-left">{{ title }}</h3>
        <p class="text-right cstm-text-right">
            <button class="btn btn-outline-primary">See all</button>
        </p>
      </div>
      <table class="cstm-table">
          <thead class="cstm-table-thead">
              <tr>
                  <th class="border-top-0" v-for="(title, index) in (Object.keys(requisitions[0]))" v-bind:key="index">{{ title | TitleCase }}</th>
                  <th class="border-top-0"></th>
              </tr>
          </thead>
          <tbody>
              <tr v-for="(order, index) in requisitions" :key="index">
                  <td  class="border-0" v-for="(value, name, index) in order" :key="index">{{ value }}</td>
                  <td class="border-0"><button class="btn btn-primary">Order Details</button></td>
              </tr>
          </tbody>
      </table>
  </div>
</template>

<script>
export default {
    name: 'DashboardFirst',
    props: {
        requisitions: Array
    },
    data(){
        return{
            title: 'Requisitions'
        }
    },
    filters: {
        TitleCase : function(title){
            title = title.charAt(0).toUpperCase() + title.slice(1)
            return title.replace("_", " ");
        }
    }
}
</script>

<style>

.cstm-table{
    width: 100%
}
.cstm-table-thead tr th{
    font-weight: normal;
}
.cstm-container-req{
    max-height:578px;
    height: 100%;
    min-height: 578px;
    padding: 21px 23px;
    box-sizing: border-box

}
.cstm-text-right{
    position: relative;
    top: -20px;
}
</style>