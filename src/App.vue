<script setup lang="ts">
import Card from './components/Card.vue'
import qrCode from '/image-qr-code.png'
</script>

<template>
  <Card title="Improve your front-end skills by building projects"
    description="Scan the QR code to visit Frontend Mentor and take your coding skills to the next level"
    :image-url="qrCode" />
</template>

<style scoped></style>
