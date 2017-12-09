<template>
  <div class="hello container mt-5">
    <div class="input-group mb-5">
  <input type="text" class="form-control" placeholder="請輸入訊息">
  <span class="input-group-addon">
  <button class="btn btn-primary">Go</button>
  </span>
</div>
    <div class="media">
      <img class="align-self-start mr-3" src="http://lorempixel.com/100/100/food/1/" alt="Generic placeholder image">
      <div class="media-body">
        <h5 class="mt-0">Top-aligned media</h5>
        <p>Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis. Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia congue felis in faucibus.</p>
        <p>Donec sed odio dui. Nullam quis risus eget urna mollis ornare vel eu leo. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.</p>
      </div>
    </div>
    <div class="media">
      <div class="media-body">
        <h5 class="mt-0 mb-1">Media object</h5>
        Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis. Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia congue felis in faucibus.
      </div>
      <img class="ml-3" src="http://lorempixel.com/100/100/food/3/" alt="Generic placeholder image">
      </div>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
