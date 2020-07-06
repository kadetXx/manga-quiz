<template>
  <div>
    <div class="question-heading">
      <h2>
        Question 1<span class="question-number">/10</span>
      </h2>
    </div>

    <div class="question-container">
      <div class="question-box">
        <p class="question">
          What is the name of the fastest programmer in the middle east who won a guiness world record last year
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Questions',
  props: {
    
  }
}
</script>

<style scoped>

  .question-heading {
    margin: 1% 20%;
    color: #ced2e4;
    border-bottom: 1px dashed rgba(150, 141, 141, 0.3);
    padding: 2% 0%;
  }

  .question-number {
    font-size: 13px;
    font-weight: 100;
    letter-spacing: 2px;
    margin-left: 2px;
  }

  .question-box {
    margin: 2% 20%;
  }

  .question {
    color: #eeeff7;
    font-size: 21px;
    font-weight: 400;
  }

  @media (max-width: 900px) {

  .scoreboard {
    margin-bottom: 2rem;
  }

  .question-heading, .question-box {
    margin: 4% 7%;
  }

  .question-box {
    margin-bottom: 3rem;
    margin-top: 2rem
  }

  .question-heading {
    padding-bottom: 0.6rem;
  }
}

</style>