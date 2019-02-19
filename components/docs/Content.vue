<template>
  <div id="docs-content">
    <h2 class="title">{{ command }}</h2>
    <h5 class="subtitle">{{ explanation }}</h5>
    <p>{{ text }}</p>
  </div>
</template>

<script>
export default {
  props: [
    'command',
    'explanation',
    'text'
  ]
}
</script>