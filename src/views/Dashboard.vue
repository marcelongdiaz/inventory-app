<template>
    <div class="border-1">
        <dashboard-first :requisitions="requisitions"></dashboard-first>
        <dashboard-second></dashboard-second>
    </div>
</template>

<script>

import DashboardFirst from '@/components/DashboardFirst';
import DashboardSecond from '@/components/DashboardSecond';
export default {
    name: 'Dashboard',
    components: {
        DashboardFirst,
        DashboardSecond
    },
    data(){
        return{
            requisitions: [
                {
                    name: "Grant Marshall",
                    position: "Junior Software Engineer", 
                    department: "IT",
                    mobile_number: "01718332233",
                },
                {
                    name: "Pena Valdez",
                    position: "Executive", 
                    department: "Marketing",
                    mobile_number: "09112312343",
                },
                {
                    name: "Jessica Miles",
                    position: "Intern", 
                    department: "Marketing",
                    mobile_number: "01812223123",
                },
                {
                    name: "Kerri Barber",
                    position: "Junior Analyst", 
                    department: "IT",
                    mobile_number: "01900001123",
                },
                {
                    name: "Natasha Gamble",
                    position: "Software Engineer", 
                    department: "IT",
                    mobile_number: "01982122222",
                }
            ]
        }
    }
}
</script>

<style>

</style>