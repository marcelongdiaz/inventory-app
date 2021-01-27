<template>
<div class="cstm-progress-container">

    <div class="clear-container row">
        <div class="col-sm-3 progressbar-label-cntr">
            <p class="progressbar-label">Tissue Paper</p>
        </div>
        <div class="floater col-sm-7 ">
            <div class="progress cstm-progress">
                        <div class="progress-bar bg-danger" role="progressbar" style="width: 10%" aria-valuenow="10" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
        </div>
    </div>
    <div class="clear-container row">
        <div class="col-sm-3 progressbar-label-cntr">
            <p class="progressbar-label">A4 Size Paper</p>
        </div>
        <div class="floater col-sm-7">
            <div class="progress cstm-progress">
                        <div class="progress-bar bg-warning" role="progressbar" style="width: 45%" aria-valuenow="45" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
        </div>
    </div>
    <div class="clear-container row">
        <div class="col-sm-3 progressbar-label-cntr">
            <p class="progressbar-label">Mug</p>
        </div>
        <div class="floater col-sm-7">
            <div class="progress cstm-progress">
                        <div class="progress-bar bg-success" role="progressbar" style="width: 90%" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100"></div>
            </div>
        </div>
    </div>
    
</div>
</template>

<script>
export default {
    name: 'ProgressBar',
    props: [],
    data(){
        return
    }
}
</script>

<style>
.progressbar-label{
    /* float: left; */
    margin: 0 102px 0 0;
    text-align: left;
}
.cstm-progress{
    transform: translateY(50%);
    border-radius: 9px;
    border: 1px solid #e9ecef;
}
.cstm-progress .progress-bar{
    border-radius:9px
}
.clear-container{
    /* height: 47px; */
    margin-bottom : 23px;  
    border-bottom: 1px solid rgba(0, 0, 0, 0.174);
    padding-bottom: 20px;
    margin-top :17px
}
.clear-container::after{
    content: "";
    display: table;
    clear: both;
    
}
.floater{
    float: right
}
.progressbar-label-cntr{
    padding: 0;
    white-space: nowrap;
}
</style>