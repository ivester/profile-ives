<template>
  <div>
    <MainNav />
    <slot name="header" class="bg">Default header</slot>
    <slot name="default"/>
    <slot name="footer">
      <footer>Copyright {{new Date().getFullYear()}}</footer>
    </slot>
  </div>
</template>