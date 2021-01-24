<template>
  <div id="app">
    <main-header></main-header>
    <div class="row">
      <div class="col-md-2 cstm-nav">
        <ul class="cstm-nav-list">
          <li><span class="icon-cstm-dashboard cstm-icon"></span> Dashboard</li>
          <li><span class="icon-cstm-requisition cstm-icon"></span> Requisitions</li>
          <li><span class="icon-cstm-store cstm-icon"></span> Stocks</li>
          <li><span class="icon-cstm-employees cstm-icon"></span> Employees</li>
          <!-- <li><span class="icon-cstm-invoice"></span> Report</li> -->
        </ul>
      </div>
      <div class="col-md-10 cstm-view">
        <router-view/>
      </div>
    </div>
    
  </div>
</template>

<script>
import MainHeader from '@/components/MainHeader'
export default {
  name: 'App',
  components: {
    MainHeader
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
.cstm-nav{
  padding: 41px 21px
}
.cstm-nav-list{
  list-style-type: none;
  padding: 0
} 
.cstm-nav-list li{
  margin-bottom: 35px;
  text-align: left;
  padding-left: 21px
}
.cstm-icon{
  margin-right: 16px
}
.cstm-view{
  padding: 30px;
  box-sizing: border-box;
}

.app{
  background-color: #F7F9FB
}
</style>
