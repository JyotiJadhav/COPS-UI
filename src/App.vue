<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-md-12">
        <Header></Header>
      </div>
    </div>
    <div class="row" v-if="type == 'Daily'">
      <div class="col-md-4">
        <TaskList></TaskList>
      </div>
      <div class="col-md-8">
        <TaskLayout type="Daily" ></TaskLayout>
        <TaskProgress></TaskProgress>
        <DailyTasks></DailyTasks>
      </div>
    </div>
     <div class="row" v-if="type=='Weekly'">
      <div class="col-md-12" >
        <TaskLayout type="Weekly" ></TaskLayout>
        <TaskProgress v-if="false"></TaskProgress>
        <Weekly></Weekly>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <Footer></Footer>
      </div>
    </div>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" yourName = "JYOTI"/> -->
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import TaskList from "./components/TaskLayout/TaskList";
import Header from "./components/Layout/Header";
import DailyTasks from "./components/TaskLayout/DailyTasks";
import TaskLayout from "./components/TaskLayout/TaskLayout";
import TaskProgress from "./components/TaskLayout/TaskProgress";
import Footer from "./components/Layout/Footer";
import Weekly from "./components//Template/TemplateGrid";

export default {
  name: "App",
  components: {
    TaskList,
    Header,
    DailyTasks,
    TaskLayout,
    TaskProgress,
    Footer,
    Weekly,
  },
  data(){
    return{
      type: 'Weekly'
    }
  }
};
</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
