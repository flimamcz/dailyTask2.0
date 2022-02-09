<template>
   <div id="app">
      <Header />
      <main class="mainContainer">
        <div class="intro-text">
          <h1>Tarefa do dia <span></span></h1>
          <p>Adicione suas tarefas diárias, mantendo seu foco e disciplina diariamente!</p>
          <p>Recupere a clareza e a tranquilidade, tirando todas essas tarefas da sua cabeça e colocando na sua lista de tarefas.</p>
        </div>

        <div class="img-people">
          <img src="/peoples-intro.svg" alt="peoples in task">
        </div>
      </main>

      <Footer/>
   </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,400;0,500;0,700;1,400;1,500;1,700&display=swap');

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  list-style-type: none;
  color: #FFFFFF;
  font-family: 'Roboto', sans-serif;
}

body{
  background: #232625;
}

img{
  display: block;
  max-width: 100%;
}

.mainContainer{
  width: min(90%, 1200px);
  margin: 20px auto;
  display: flex;
  align-items: center;
  flex-direction: row;
  height: 70vh;
  justify-content: space-between;
  padding: 0 60px;
}

.intro-text h1{
  font-style: italic;
  font-size: 2.4rem;

}

.intro-text p{
  max-width: 320px;
  margin-top: 20px;
  font-style: italic;
}

@media screen and (max-width: 1130px){
  .mainContainer{
    padding: 0;
  }
}

@media screen and (max-width: 900px){
  .img-people{
    max-width: 350px;
  }

  .intro-text{
    margin-right: 40px;

  }

  .intro-text h1{
    font-style: italic;
    font-size: 2rem;

  }

  .intro-text p{
    font-size: 0.875rem;
    max-width: 300px;
    margin-top: 15px;
  }


}

@media screen and (max-width: 600px){
  .img-people{
    display: block;
    max-width: 250px;
    margin: 40px auto;
  }

  .intro-text{
    margin-right: 0;
  }
  
  .intro-text h1{
    font-style: italic;
    font-size: 1.8rem;
    text-align: center;
  }

  .intro-text p{
    font-size: 0.875rem;
    text-align: center;
    max-width: 300px;
    margin: 15px 0;
  }

  .mainContainer{
    width: min(90%, 300px);
    flex-direction: column;
    justify-content: center;
    padding: 0 20px;
  }

}

</style>
