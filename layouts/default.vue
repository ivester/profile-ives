<!-- TODO refactor to use script setup -->
<script >
export default {
  setup () {
    useMeta({
      title: '🐶 Ivester\'s Profile Page',
      bodyAttrs: {
        class: 'bg-grey-100 font-sans leading-normal tracking-normal'
      }
    })
  }
}
</script>

<template>
  <div>
    <!-- <MainNav /> -->
    <!-- <slot name="header" class="bg">Default header</slot> -->
    <slot name="default"/>
    <!-- <slot name="footer">
      <footer>Copyright {{new Date().getFullYear()}}</footer>
    </slot> -->
  </div>
</template>