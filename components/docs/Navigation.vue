<template>
  <div id="docs-navigation">
    <b-row>
      <b-col cols="12" md="4">
        <b-nav vertical class="w-25">
          <b-nav-item v-for="item in items" v-bind:key="item.text" :href="item.link">{{ item.text }}</b-nav-item>
        </b-nav>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  data () {
    return {
      items: [
        { text: '!invest', link: '#invest' },
        { text: '!balance', link: '#balance' },
        { text: '!broke', link: '#broke' },
        { text: '!active', link: '#active' },
        { text: '!top', link: '#top' },
      ]
    }
  }
}
</script>