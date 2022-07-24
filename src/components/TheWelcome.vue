<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
function button_contact(){
  alert("☠️☠️☣️☣️☠️☠️ You have been hacked!!!! ☠️☠️☣️☣️☠️☠️")
}
</script>

<template>
  <div>
    <WelcomeItem  class='logo_color_secondary'>
      <template #icon>
        <DocumentationIcon />
      </template>
      <template #heading>Banking & Payments</template>
        With vast experience in the technology used in banks and other financial institutions, we provide hassle free IT consulting in the finance sector.
    </WelcomeItem>

    <WelcomeItem class='logo_color_secondary'>
      <template #icon>
        <ToolingIcon />
      </template>
      <template #heading>Internet of Things</template>
      We extend seamless integration of sensors and other hardware using IoT for commercial clients.
    </WelcomeItem>

    <WelcomeItem class='logo_color_secondary'>
      <template #icon>
        <EcosystemIcon />
      </template>
      <template #heading>Machine Learning</template>
      Our data science & ML experts propel your business forward by delivering crucial insights.
    </WelcomeItem>

      <WelcomeItem class='logo_color_secondary'>
      <template #icon>
        <CommunityIcon />
      </template>
      <template #heading>Data Analytics</template>
      We help you understand your data through superior data analysis techniques.
    </WelcomeItem>
  </div>
  <div class="contact_button_css">
    <button class="button-86" role="button" v-on:click="button_contact()">Contact</button>
  </div>
</template>

<style scoped>
main .contact_button_css{
  margin: 0;
  position: relative;
  top: 0%;
  left: 45%;
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