<template>
  <h6>With only Custom Component and Imports</h6>

  <div>
    <custom-component />
  </div>
</template>

<script lang="ts">
import { QBtn, Notify } from 'quasar'
import { defineComponent } from 'vue'
import CustomComponent from './custom-component.ts'

console.log(QBtn)
console.log('Notify', Notify)

export default defineComponent({
  name: 'RSOnlyCustomWithImports',
  components: {
    CustomComponent
  }
})
</script>
