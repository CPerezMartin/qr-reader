<template>
  <div>
    <qrcode-stream @decode="handleDecode" />
  </div>
</template>

<script lang="ts">
  export default {}
</script>

<script setup lang="ts">
import { QrcodeStream } from "vue-qrcode-reader";



const handleDecode = (result: string | null) => {
  if (result) {
    console.log(result);
    // Realiza alguna acción con el resultado del escaneo del código QR
  }
};
</script>

<style scoped>
/* Estilos opcionales para el componente */
</style>
