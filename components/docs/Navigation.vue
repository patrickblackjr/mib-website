<template>
  <div id="docs-navigation">
    <b-nav vertical class="w-25">
      <b-nav-item v-for="item in items" v-bind:key="item.text" :href="item.link">{{ item.text }}</b-nav-item>
    </b-nav>
  </div>
</template>

<script>
export default {
  data () {
    return {
      items: [
        { text: '!invest', link: '/docs' },
        { text: '!balance', link: '/docs/balance' },
        { text: '!broke', link: '/docs/broke' },
        { text: '!active', link: '/docs/active' },
        { text: '!top', link: '/docs/top' },
      ]
    }
  }
}
</script>

<style>
#docs-navigation {
  border: 1px solid black;
}
</style>
