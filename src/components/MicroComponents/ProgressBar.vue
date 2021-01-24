<template>
    <div>
    <p class="progressbar-label">Tissue Paper</p>
    <div class="progress">
                <div class="progress-bar" role="progressbar" style="width: 25%" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100"></div>
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
    float: left;
    margin: 0;
}
</style>