<template>
  <div>
    <footer class="footer">
      <p>DailyTask - 2022</p>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>


<style scoped>

.footer{
  position: fixed;
  bottom: 0;
  width: 100%;
  height: 10vh;
  background: #35A852;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: row;
}

.footer p{
  font-size: 1rem;
  font-weight: bold;
}


</style>