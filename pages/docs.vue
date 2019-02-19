<template>
  <div id="docs">
    <b-container>
      <page-header :title="pageTitle" />
      <Navigation />
    </b-container>
  </div>
</template>

<script>
import PageHeader from '@/components/PageHeader.vue';
import Navigation from '@/components/docs/Navigation.vue';

export default {
  components: {
    PageHeader,
    Navigation
  },
  head () {
    let title = this.pageTitle;
    return {
      title: title,
      meta: [{
          hid: `description`,
          name: 'description',
          content: `Start investing in memes with the best broker in /r/MemeEconomy today!`
        }
      ]
    }
  },
  data () {
    return {
      pageTitle: 'Documentation',
    }
  }
}
</script>