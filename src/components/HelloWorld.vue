<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button @click="increasecountvalue">increase</button><br><br>
    <button type="button"> count is {{ count }} </button ><br><br>
    <button @click="decreasecountvalue">decrease</button>
    <p>Name: {{misnomer}}</p>
    <p>date: {{date}}</p>
    <p>session: {{session}}</p>
    
  </div>
  <div id="footer-msg">
    <p>
      This is the hello world project to see how vue-js works <br> and twist its approach to my whims
    </p>
  </div>
</template>

<script>
export default{
  //props option
  props:['msg'],
  //data options
  data(){
    return{
      count:0,
      misnomer:"run the world",
      date: "11/06/2023",
      session:"session 50",
    }
  },
  methods:{
    //this method focuses on increasing the value of count
    increasecountvalue()
    {
      //get the count variable and increment it by one
      this.count++;
    }, 
    //this methos focuses on decreasing the value of count
    decreasecountvalue()
    {
      //get the value of count and decrease the value by one
      if(this.count === 0 )
        this.count = 0;
      else
        this.count--;
    }
  }
}
// const count = ref(0)
</script>



<style scoped>
.read-the-docs {
  color: #888;
}

.card{
  font-weight:400;
  color: #9da2fd;
}
#footer-msg{
  font-weight:100;
  font-size: 70%;
}


h1{
  font-family: 'Kablammo', cursive;
}

</style>
