<template>
  <SidebarView />
  
  <div>
    <HeaderView />

  </div>

</template>

<script>
import SidebarView from '@/components/sidebar/SidebarView.vue'
import HeaderView from '@/components/HeaderView.vue'
import { sidebarWidth } from '@/components/state'
import { useSidebarResponsive } from '@/components/state.js'


export default {
  components: { SidebarView, HeaderView },
  setup() {
    useSidebarResponsive()
    return { sidebarWidth }


  }
}
</script>
