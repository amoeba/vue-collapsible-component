<template>
  <div class="collapsible-pane">
    <slot name="title" v-on:click="handleClick">
      default title
    </slot>
    <slot v-if="collapsed" name="content">
      default content
    </slot>
  </div>
</template>

<script>
export default {
  name: 'CollapsiblePane',
  data: () => {
    return {
      collapsed: true
    }
  },
  methods: {
    handleClick() {
      this.collapsed = !this.collapsed;
    }
  }
}
</script>
