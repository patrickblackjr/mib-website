<template>
  <div id="docs">
    <b-container>
      <page-header :title="pageTitle" />
      <b-row align-h="center" class="text-center">
        <!-- <b-col cols="12" md="2" class="text-right">
          <Navigation />
        </b-col> -->
        <b-col cols="12" md="8">
          <p class="mb-4">
            To invoke a command, reply to either the top-level u/MemeInvestor_bot comment 
            in the comment section of any r/MemeEconomy post or to one of its subsequent 
            replies to your command comment.
          </p>
          <Content command="!invest [amount]" explanation="Invests the amount you enter in the meme." text="4 hours after the investment, the meme growth will be evaluated and your investment can profit you or make you bankrupt. Minimum possible investment is 100 MemeCoins. Example: !invest 1500" />
          <Content command="!balance" explanation="Returns your current balance" />
          <Content command="!broke" explanation="Invoke this command when your balance will become 100 Memecoins." text="You must have no active investements and balance below 100 Memecoins." />
          <Content command="!active" explanation="Returns a number of active investments." />
          <Content command="!top" explanation="Returns the top 5 meme investors." />
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import PageHeader from '@/components/PageHeader.vue';
// import Navigation from '@/components/docs/Navigation.vue';
import Content from '@/components/docs/Content.vue';

export default {
  components: {
    PageHeader,
    // Navigation,
    Content
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