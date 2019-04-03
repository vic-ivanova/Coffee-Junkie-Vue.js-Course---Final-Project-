<template>
    <header class="masthead">
      <div class="container">
        <div class="intro-text">
          <div class="intro-heading text-uppercase">{{ SiteName }}</div>
          <div class="intro-lead-in">{{ SiteSlogan }}</div>
          <a class="btn btn-primary btn-menu btn-xl text-uppercase js-scroll-trigger" href="#menu">{{ BtnText }}</a>
        </div>
      </div>
    </header>
</template>

<script>
export default {
  data(){
    return {
      SiteName: 'Coffee Junkie',
      SiteSlogan: 'because nothing makes sense before coffee',
      BtnText: 'View Our Menu',
    }
  }
}
</script>

<style scoped>

</style>


