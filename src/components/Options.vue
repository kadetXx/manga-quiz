<template>
  <div class="Optioncomponent">
    <div class="option-box">
      <div class="option">
        <p>Ahmed Musa</p> 
        <div class="check"></div>
      </div>
       <div class="option">
        <p>Mohammed Salah</p> 
        <div class="check"></div>
      </div>
       <div class="option">
        <p>Argen Robben</p> 
        <div class="check"></div>
      </div>
       <div class="option">
        <p>Kelechi Iheanacho</p>
        <div class="check"></div>
      </div>
    </div>
    
    <div class="button-container">
      <button>Next</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Options',
  props: {

  },
}
</script>

<style scoped>
 
  body {
    color: #eeeff7;
  }

  .option-box {
    margin: 0 20%;
  }

  .option {
    margin: 2% 0;
    padding: 2%;
    border-radius: 10px;
    display: flex;
    justify-content: space-between;
    box-shadow: 0px 0px 2px 1px #435996;
    background-color: rgba(0, 0, 0, 0.3);
  }

  .option:hover {
    box-shadow: 0px 0px 2px 3px #435996;
    background-color: #252C4A;
  }

  .check {
    width: 20px;
    height: auto;
    border-radius: 100%;
    background-color: rgba(0, 0, 0, 0.3);
  }

  .button-container {
    display: flex;
    width: 100%;
    justify-content: center;
    align-items: center;
  }

  button {
    padding: 1rem 3rem;
    background-color: #117EEB;
    border: none;
    border-radius: 20px;
    color: #fff;
  }

  button:hover {
    background-color: #083e74;
  }

  button:focus {
    outline: none;
  }

  @media (max-width: 900px) {
  .option-box {
    margin: 5% 7%;
  }

  .option {
    padding: 0.8rem;
    box-shadow: 0px 0px 3px 2px #435996;
    background-color: #252C4A;
    margin: 1rem 0;
  }

  .option:hover {
    box-shadow: 0px 0px 2px 1px #435996;
    background-color: rgba(0, 0, 0, 0.3);
  }

}
  

</style>