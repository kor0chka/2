<template>
  <div class="wrapper">

    <header>
      <div class="navbar">
        <div class="container">
          <div class="navbar-content">
            <div class="logo"> Users CRM </div>
            <ul class="navbar-list">
              <li class="navbar-item" v-for="link in links" :key="link.title">
                <router-link class="mavbar-link" :title="link.title" :to="link.url">{{}}</router-link>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  data () {
    return {
      links: [
        { title: 'Home', url: '/'},
        { title: 'Users', url: '/users'}
      ]
    }
  }
}
</script>
