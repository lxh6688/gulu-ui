<template>
  <div class="tabs-item" @click="xxx">
    <slot></slot>
  </div>
</template>
<script>
  export default {
    name: 'GuluTabsItem',
    props: {
      disabled: {
        type: Boolean,
        default: false
      },
      name: {
        type: String|Number,
        requierd: true
      }
    },
    inject: ['eventBus'],
    created(){
      this.eventBus.$on('update:selected', (name) => {
        console.log(name)
      })
    },
    methods:{
      xxx(){
        this.eventBus.$emit('update:selected', this.name)
      }
    }
  }
</script>
<style>
  .tabs-item {
  }
</style> 