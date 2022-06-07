<template>
<HelloWorld />
</template>

<script>
import { defineComponent } from 'vue'

// Components
import HelloWorld from '../components/HelloWorld.vue'
import DashboardLayout from '../layouts/DashboardLayout.vue'

export default defineComponent({
  name: 'HomeView',

  components: {
    HelloWorld
  },
  created () {
    this.$emit('update:layout', DashboardLayout)
  }
})
</script>
