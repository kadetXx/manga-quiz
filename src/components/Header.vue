<template>
  <div>
    <header>
      <div class="top-container">
      <div class="scoreboard">
        <h2 class="score-head">MangaQuiz</h2> <!--<span class="question-number">1 of 10</span>-->
      </div>
    </div>
    </header>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {

  },
  data() {
    return {
      nav: [
        {name: 'Home', route: '/'},
        {name: 'Help', route: '/help'}
      ]
    }
  }
}
</script>

<style>

  .top-container {
    display: flex;
    align-items: center;
  }

  .scoreboard {
    padding: 2%;
    box-shadow: inset 0px 0px 2px 1px rgba(0, 0, 0, 0.3);
    border-radius: 0;
    width: 100%;
    display: flex;
    justify-content: center;
    color: #ced2e4;
  }

  @media (max-width: 900px) {

    .scoreboard {
      margin-bottom: 2rem;
    }

  }
</style>