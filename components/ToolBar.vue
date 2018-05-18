<template>
    <div>
        <v-toolbar dark fix app class="teal darken-4" :clipped="$vuetify.breakpoint.lgAndup">
        <v-toolbar-side-icon @click="drawer = !drawer"></v-toolbar-side-icon>
        <v-btn
            icon
            @click.stop="miniVariant = !miniVariant"
        >
            <v-icon v-html="miniVariant ? 'chevron_right' : 'chevron_left'"></v-icon>
        </v-btn>
        <v-btn
            icon
            @click.stop="clipped = !clipped"
        >
            <v-icon>web</v-icon>
        </v-btn>
        <v-btn
            icon
            @click.stop="fixed = !fixed"
        >
            <v-icon>remove</v-icon>
        </v-btn>
        <v-toolbar-title v-text="title"></v-toolbar-title>
        <v-spacer></v-spacer>
        </v-toolbar>
    </div>
</template>

<script>
  export default {
    data () {
      return {
        clipped: false,
        drawer: true,
        fixed: false,
        items: [
          { icon: 'apps', title: 'Welcome', to: '/' },
          { icon: 'bubble_chart', title: 'Inspire', to: '/inspire' }
        ],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: 'Vuetify.js'
      }
    }
  }
</script>
