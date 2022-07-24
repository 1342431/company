<script setup>
function Home_Button(){
    document.getElementById('Description').style.display = "block";
    document.getElementById('ContactForm').style.display = "none";
}
</script>
<template>
    <div>
        <h1 class="email_css"> info@1342431.com</h1>
    </div>
    <div class="home_button_css">
        <button class="button-86" role="button" @click="Home_Button()">Home</button>
    </div>
</template>
<style scoped>

.email_css{
    left: 35%;
    bottom: 50px;
    top: 200px;
}

.home_button_css{
  margin: 0;
  position: relative;
  top: 300px;
  left: 46%;
}

.button-86 {
  all: unset;
  width: 100px;
  height: 30px;
  font-size: 16px;
  background: transparent;
  border: none;
  position: relative;
  color: #f0f0f0;
  cursor: pointer;
  z-index: 1;
  padding: 10px 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  white-space: nowrap;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  top: 50%
}

.button-86::after,
.button-86::before {
  content: '';
  position: absolute;
  bottom: 0;
  right: 0;
  z-index: -99999;
  transition: all .4s;
}

.button-86::before {
  transform: translate(0%, 0%);
  width: 100%;
  height: 100%;
  background: #051e28;
  border-radius: 10px;
}

.button-86::after {
  transform: translate(10px, 10px);
  width: 35px;
  height: 35px;
  background: #c18d71;
  backdrop-filter: blur(5px);
  -webkit-backdrop-filter: blur(5px);
  border-radius: 50px;
}

.button-86:hover::before {
  transform: translate(5%, 20%);
  width: 110%;
  height: 110%;
}

.button-86:hover::after {
  border-radius: 10px;
  transform: translate(0, 0);
  width: 100%;
  height: 100%;
}

.button-86:active::after {
  transition: 0s;
  transform: translate(0, 5%);
}
</style>