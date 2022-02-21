<template>

  <header>
    <div class="container">

      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      
      <nav>
        <ul>
          <li><a href="#">CHARACTERS</a></li>
          <li><a href="#" class="active">COMICS</a></li>
          <li><a href="#">MOVIES</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">GAMES</a></li>
          <li><a href="#">COLLECTIBLES</a></li>
          <li><a href="#">VIDEOS</a></li>
          <li><a href="#">FANS</a></li>
          <li><a href="#">NEWS</a></li>
          <li><a href="#">SHOP</a></li>
        </ul>  
      </nav>     

    </div>
  </header>

</template>

<script>
export default {
  name: 'HeaderComponent'
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
