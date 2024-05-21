<template>
  <div>
    <button @click="sendDataToParent">tekan untuk kirim data ke parent</button>
  </div>
</template>

<script>
export default {
  name: 'ChildComponent',
  methods: {
    sendDataToParent() {
      this.$emit('dataSent', 'jika kamu melihat tulisan ini,maka proses kirim data ke parent berhasil :)');
    }
  }
}
</script>

<style scoped>
button {
  padding: 10px 20px;
  font-size: 16px;
  background-color: #42b983;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #369a6e;
}
</style>
