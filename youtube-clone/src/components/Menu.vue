<template>
  <v-toolbar flat dark>
    <v-card class="mx-auto" height="400" width="256">
      <v-navigation-drawer class="deep-purple accent-4" permanent>
        <v-list>
          <v-list-item v-for="item in items" :key="item.title" link>
            <v-list-item-icon>
              <v-icon>{{ item.icon }}</v-icon>
            </v-list-item-icon>

            <v-list-item-content>
              <v-list-item-title>{{ item.title }}</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>

        <template v-slot:append>
          <div class="pa-2">
            <v-btn block>Logout</v-btn>
          </div>
        </template>
      </v-navigation-drawer>
    </v-card>
    <v-btn>
      <v-icon>ICON</v-icon>
      <v-toolbar-title>YouTube</v-toolbar-title>
    </v-btn>
  </v-toolbar>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue';

export default {
  name: "menubar",
  components: {},
    data () {
        return {
            items: [
            { title: 'Dashboard', icon: 'dashboard' },
            { title: 'Account', icon: 'account_box' },
            { title: 'Admin', icon: 'gavel' },
            ],
        }
    },
    
};
</script>

<style scoped>
</style>
