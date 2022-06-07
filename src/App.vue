<template>
  <v-app>
    <component :is="layout">
      <router-view v-model:layout="layout"></router-view>
    </component>
    </v-app>
</template>

<script>

export default {
  name: 'App',
  data () {
    return {
      layout: 'div'
    }
  }
}
</script>
