<template>
  <v-app>
    <ToolBar></ToolBar>
    <MenuDrawer></MenuDrawer>
    
    <v-content>
      <v-container>
        <!-- this is where content are rendered -->
        <nuxt />
      </v-container>
    </v-content>
  <Footer></Footer>
  </v-app>
</template>

<script>
  import MenuDrawer from '~/components/MenuDrawer'
  import ToolBar from '~/components/ToolBar'
  import Footer from '~/components/Footer'

  export default {
    components: {
      MenuDrawer,
      ToolBar,
      Footer
    }
  }
</script>
