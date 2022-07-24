<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
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
      <EcosystemIcon />
    </template>
    <template #heading>Data Analytics</template>
    We help you understand your data through superior data analysis techniques.
  </WelcomeItem>

</template>
