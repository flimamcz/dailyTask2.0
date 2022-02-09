<template>
  <div>
    <header class="header">
      <div class="container">
        <div class="logo">
          <img src="logo-todolist.svg" alt="logo DailyTask">
        </div>
        <div>
          <NuxtLink to="/" class="button">Adicionar Task</NuxtLink>
        </div>
      </div>
    </header>
    <div class="sep"></div>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>


<style scoped>

*{
  font-size: 62.5%;
}

.container{
  display: flex;
  width: min(90%, 1200px);
  padding: 25px 0;
  align-items: center;
  justify-content: space-between;
  margin: 0 auto;
}



.sep{
  width: 100%;
  height: 1.4px;
  display: block;
  background: rgba(255, 255, 255, 0.4);
}

.button{
  width: 160px;
  height: 45px;
  border-radius: 3px;
  font-size: 1rem;
  font-weight:  700;
  background: #35A852;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 12px;
  transition: .3s ease-in;
}

.button:hover{
  background: #4ad46d;
  color: #232625;
}

@media screen and (max-width: 600px){
  .logo{
    max-width: 120px;
  }

  .button{
  width: 140px;
  height: 40px;
  border-radius: 2px;
  font-size: 0.875rem;
  padding: 8px;
}
}

</style>