<template>
  <div class="hello container mt-5">
    <div class="input-group mb-5">
  <input type="text" class="form-control" v-model="message" placeholder="請輸入訊息">
  <span class="input-group-addon">
  <button class="btn btn-primary" @click="submitMessage()">Go</button>
  </span>
</div>
    <div class="media" v-for="item in messages">
      <img v-if="item.username == username" class="align-self-start mr-3" src="https://www.dramafever.com/st/news/images/72eb3876-4148-4370-8911-570f5dd18178.jpg" width="100px" height="100px" alt="Generic placeholder image">
      <div class="media-body">
        <h5 class="mt-0">{{item.username}}</h5>
        <p>{{item.message}}</p>
      </div>
      <img v-if="item.username != username" class="align-self-start mr-3" src="http://www.chinapress.com.my/wp-content/uploads/2017/06/20170626fb35.jpg" width="100px" height="100px" alt="Generic placeholder image">
    </div>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      username:'Winni',
      message: '',
      messages: [
        {
          username:'Ricahrd',
          message :'Hello Winni'
        },
        {
          username:'Winni',
          message :'安安'
        }
      ]
    }
  },
  methods:{
    submitMessage(){
      let vm = this
      vm.messages.unshift({
          username:vm.username,
          message :vm.message
        })
        vm.message = ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
