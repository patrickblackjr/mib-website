<template>
  <div id="main">
    <b-container>
      <Header/>
      <Donate/>
    </b-container>
  </div>
</template>

<script>
import Header from '@/components/home/Header.vue';
import Donate from '@/components/home/Donate.vue';

export default {
  components: {
    Header,
    Donate
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
      pageTitle: 'Home',
    }
  }
}
</script>