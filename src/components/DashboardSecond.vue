<template>
  <div class="row">
      <div class="col-md-6 cstm-ss-container-l">
        <div class="cstm-container cstm-second-stock ">
            <div class="cstm-req-header">
                <h4 class="d-inline float-left">{{ title1 }}</h4>
                <button class="btn btn-outline-primary float-right">See all</button>
            </div>
            <div class="progressbar-container">
                <progress-bar></progress-bar>
            </div>
        </div>
          
      </div>    
      <div class="col-md-6 cstm-ss-container-r">
        <div class="cstm-container cstm-second-stock ">
            <div class="cstm-req-header">
                <h4 class="d-inline float-left">{{ title2 }}</h4>
                <!-- <custom-dropdown></custom-dropdown> -->
            </div>
        </div>
          
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
    /* padding: 31px */
    padding: 0px;
    height: 100%;
}
.cstm-req-header{
    overflow: hidden;
    padding: 20px 31px 20px 31px;
    position: relative;
    border-bottom: 0.5px solid gray
}
.cstm-req-header h3{
    transform: translateY(50%)
}

.progressbar-container{
    padding: 33px 30px 29px 30px
}
.cstm-ss-container-l{
    padding: 0px 15px 0px 0px;
}
.cstm-ss-container-r{
    padding: 0px 0px 0px 15px;
}
</style>