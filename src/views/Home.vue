<template>
  <div class="home">
  <Questions />
    <Options />
  </div>
</template>

<script>
// @ is an alias to /src
import Questions from '../components/Questions'
import Options from '../components/Options'
import axios from 'axios'

export default {
  name: 'Home',
  components: {
    Questions,
    Options
  },

  data() {
    return {
      apiQuiz: []
    }
  },

  mounted: () => {
    axios.get('https://opentdb.com/api.php?amount=10&category=31&type=multiple')
    .then(res => {
      this.apiQuiz = res.data.results
      console.log(this.apiQuiz)
    })
    .catch(err => console.log(err))
  }
}
</script>
