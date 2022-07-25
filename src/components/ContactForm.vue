<script setup>
function Send_Button(){
  alert("message sent");
}
</script>
<template>
  <div class="form">
    <form action="https://formsubmit.co/973cd4c2571691fedf98728fcac72687" method="POST">
      <h3>Get in touch !!</h3>
      <input type="text" id="name" name="name" placeholder="Your Name" required>
      <input type="email" id="email" name="email" placeholder="Your Email" required>
      <input type="text" id="phone" name="phone" placeholder="Your Phone No." required>
      <input type="text" id="message" name="message" placeholder="How can I help you?" required>
      <input type="hidden" name="_next" value="https://1342431.com/thanks.html">
      <button class="button-86" type="submit">Send</button>
    </form>
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
  margin: 20px 0;
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