<template>

  <header>
    <div class="container">

      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      
      <nav>
        <ul>
          <li v-for="(link, index) in links" :key="index">
            <a :href="link.url" :class="link.current? 'active': ''">{{link.text}}</a>
          </li>
        </ul>  
      </nav>     

    </div>
  </header>

</template>

<script>
export default {
  name: 'HeaderComponent',
  data() {
    return {
      links: [
        {
          text: "CHARACTERS",
          url: "#",
          current: false
        },
        {
          text: "COMICS",
          url: "#",
          current: true
        },
        {
          text: "MOVIES",
          url: "#",
          current: false
        },
        {
          text: "TV",
          url: "#",
          current: false
        },
        {
          text: "GAMES",
          url: "#",
          current: false
        },
        {
          text: "COLLECTIBLES",
          url: "#",
          current: false
        },
        {
          text: "VIDEOS",
          url: "#",
          current: false
        },
        {
          text: "FANS",
          url: "#",
          current: false
        },
        {
          text: "NEWS",
          url: "#",
          current: false
        },
        {
          text: "SHOP",
          url: "#",
          current: false
        }
      ]
    }
  }
}
</script>


<style scoped lang="scss">
  @import "../assets/style/general.scss";
  @import "../assets/style/colors.scss";

  header {
    
    .container {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
  }

  nav {
    font-family: 'Roboto Condensed', sans-serif;
    font-weight: 700;
    
    ul {
      display: flex;

      li {
        padding: 0 1rem;

        a {
          color: $primary;
          padding: 4rem 0;
          display: inline-block;


          &.active,
          &:hover {
            color: $secondary;
            border-bottom: 5px solid $secondary;
          }
        }
      }
    }
  }
</style>
