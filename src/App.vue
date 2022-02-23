<template>
  <div id="app">
    <main>
      <div class="search-box">
        <input type="text" class="search-bar" placeholder="Pesquise..." />
      </div>
    </main>
  </div>
</template>

<script>
  export default {
    name: 'app',
    data () {
      return {
        api_key: 'bcb97876df3b9d375ba54203c848c15b'
      }
    }
  }
</script>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  }

  #app {
    background-image: url('./assets/cold-bg.jpg');
    background-size: cover;
    background-position: bottom;
    transition: .4s;
  }

  main {
    min-height: 100vh;
    padding: 25px;

    background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.25), rgba(0, 0, 0, 0.75));
  }

  .search-box .search-bar{
    display: block;
    width: 100%;
    padding: 15px;

    color: #313131;
    font-size: 20px;

    appearance: none;
    border: none;
    outline: none;
    
    background: rgba(255, 255, 255, 0.5);
    border-radius: 0 16px 0 16px;
    transition: .4s;
  }

  .search-box .search-bar:focus {
    background: rgba(255, 255, 255, 0.75);
    box-shadow: 0 0 16px rgba(0, 0, 0, 0.25);
    border-radius: 16px 0 16px 0;
  }
</style>
