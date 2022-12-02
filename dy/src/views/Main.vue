<template>
  <div id="wrap">
    <div class="contents">
      <div class="spring">
        <p></p><p></p>
      </div>
      <LeftContents/>
      <RightContents/>
      <MenuContents/>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import LeftContents from '@/components/LeftContents.vue'
import RightContents from '@/components/RightContents.vue'
import MenuContents from '@/components/MenuContents.vue'

export default {
  name: 'App',
  components: {
    LeftContents,
    RightContents,
    MenuContents
  }
}
</script>
