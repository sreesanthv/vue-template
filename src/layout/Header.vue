<template>
  <div class="header wrapper">
    
    <div class="menu-wrapper">
      <ul class="menu">
        <li>
          <router-link to="/" exact>Home</router-link>
        </li>
      </ul>
    </div>

  </div>

</template>

<script>


export default {
  name: 'Header',
  methods: {
  }
}
</script>

<style scoped>
.header {
  z-index: 1;
  padding: 20px 0;
  position: relative;

  .is-active {
    color: #e01b3c;
  }

  a {
    color: #000;
    text-decoration: none;
  }

  .menu-wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .menu {
    font-size: 25px;
    text-transform: uppercase;
    display: flex;
    justify-content: center;
    align-items: center;

    li {
      padding: 15px;

    }

    &.side {
      font-size: 15px;

      .logout-button {
        cursor: pointer;
      }
    }
  }
}
</style>
