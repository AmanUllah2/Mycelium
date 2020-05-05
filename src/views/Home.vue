<template>
  <div class="home">
    <mission/>
  </div>
</template>

<script>
// @ is an alias to /src
import mission from '../components/mission'
//import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    mission
  }
}
</script>
