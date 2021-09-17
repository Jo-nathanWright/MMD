<template>
  <div class="container-fluid home border-top border-secondary">
    <div class="row">
      <div class="col-4 bg-info">
        <h2>Active Upgrdes :</h2>
      </div>
      <div class="col-8 d-flex flex-column justify-content-center align-items-center bg-dark text-light">
        <img class="image" src="../assets/img/moon.png" alt="clickable Moon" title="Clickable Moon" @click="click">
        <h5>Click Multiplier : </h5>
        <h5>Auto Clickers : </h5>
      </div>
    </div>
  </div>
</template>
<script>
import Pop from '../utils/Pop'
export default {
  name: 'Main',
  setup() {
    return {
      click() {
        Pop.toast('Clicked', 'success', 'top-end', 1000, false)
      }
    }
  }
}
</script>

<style scoped>
.image{
  max-width: 250px;
}
.home{
  display: grid;
  height: 90.5vh;
}
</style>
