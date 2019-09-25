<template>
<div>
    <NavDrawer></NavDrawer>
  <v-toolbar>
              <v-btn
          color="pink"
          dark
          @click.stop="drawer = !drawer"
        >
          Toggle
        </v-btn>
    <v-btn>
      <v-icon>home</v-icon>
      <v-toolbar-title>YouTube</v-toolbar-title>
    </v-btn>
  </v-toolbar>
</div>

</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue';
import NavDrawer from '@/components/NavDrawer.vue';

export default {
  name: "menubar",
  components: {
      NavDrawer,
  },
    data () {
        return {
            drawer = 0,
        }
    },
    
};
</script>

<style scoped>
</style>
