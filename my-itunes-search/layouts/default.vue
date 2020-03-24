<template>
  <section class="container">
    <div>
      <ToolBar />
      <nuxt />
    </div>
  </section>
</template>

<script>
import ToolBar from '~/components/Toolbar'

export default {
  components: {
    ToolBar
  },
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
