<template>
  <h1 style="color:crimson">Jobs</h1>
  <div v-for="job in jobs" :key="job.id">
    <router-link :to="{name:'jobdetail',params:{id:job.id}}">
    <h1>{{job.title}}</h1>
    </router-link>

  </div>
</template>

<script>
export default {
    data(){
        return{
            jobs:[
                {id:"1",title:"project manager",detail:"apple manager"},
                {id:"2",title:"project designer",detail:"apple designer"},
                {id:"3",title:"project developer",detail:"apple developer"}

            ]
        }
    }
}
</script>

<style>

</style>