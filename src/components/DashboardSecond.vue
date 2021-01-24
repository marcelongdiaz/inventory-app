<template>
  <div class="row">
      <div class="col-md-6 cstm-second-stock">
          <h3 class="d-inline float-left">{{ title1 }}</h3>
          <button class="btn btn-outline-primary">See all</button>
          <progress-bar></progress-bar>
      </div>
      <div class="col-md-6">
          <h3>{{ title2 }}</h3>
      </div>
  </div>
</template>

<script>
import ProgressBar from './MicroComponents/ProgressBar'
export default {
    name: 'DashboardSecond',
    components: {
        ProgressBar
    },
    data(){
        return{
            title1: 'Stock',
            title2: 'Usage',
            stockData:[
                {
                    item: 'Tissue Paper',
                    percentage: 5,
                    capacity: 80,
                    color: "red"
                }, 
                {
                    item: 'A4 Size Paper',
                    percentage: 20,
                    capacity: 50,
                    color: "yellow"
                }, 
                {
                    item: 'Mug',
                    percentage: 30,
                    capacity: 35,
                    color: "green"
                }, 
            ]
        }
    }
}
</script>

<style>
.cstm-second-stock{
    padding: 31px
}
</style>