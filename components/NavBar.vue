<template>
  <div id="navbar" class="bg-primary">
    <b-container>
      <b-navbar variant="primary" type="dark">
        <b-navbar-brand class="mx-auto" to="/"><img width="50px" src="/logo.png" alt="MemeInvestor Bot"></b-navbar-brand>
        <b-collapse is-nav id="nav_collapse">
        <b-navbar-nav class="ml-auto">
          <b-nav-item exact to="/">Home</b-nav-item>
          <b-nav-item exact to="/docs">Docs</b-nav-item>
          <b-nav-item exact target="new" href="https://www.patreon.com/memeinvestor_bot">Donate</b-nav-item>
          <b-nav-item exact target="new" href="https://reddit.com/r/memeinvestor_bot">Subreddit</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
      </b-navbar>
    </b-container>
  </div>
</template>

<script>
export default {
  
}
</script>