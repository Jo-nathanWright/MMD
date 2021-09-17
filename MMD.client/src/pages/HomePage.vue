<template>
  <div class="home flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-5 bg-white rounded elevation-1 bg-dark">
      <img src="../assets/img/moon.png" alt="Moon Miner Logo" class="rounded-circle elevation-2 bg-light">
      <h1 class="my-5 bg-secondary text-white p-3 rounded text-center">
        Moon Miner
      </h1>
      <router-link :to="{ name: 'Main' }">
        <button type="button" class="btn btn-large btn-outline-light">
          Start Mining
        </button>
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
  setup() {
    return {

    }
  }
}
</script>

<style scoped lang="scss">
.home{
  display: grid;
  height: 80vh;
  place-content: center;
  text-align: center;
  user-select: none;
  .home-card{
    width: 50vw;
    > img{
      height: 200px;
      width: 200px;
    }
  }
}
</style>
