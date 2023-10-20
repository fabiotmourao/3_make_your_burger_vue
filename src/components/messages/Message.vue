<template>
  <div class="message" :class="msgType">{{ msg }}</div>
</template>

<script>
export default {
  props: {
    msg: String,
    msgType: String,
  },
};
</script>

<style scoped>
.message {
  padding: 10px;
  border-radius: 5px;
  max-width: 400px;
  margin: 30px auto;
  font-weight: bold;
}

.success {
  background-color: #4CAF50;
  color: white;
}

.danger {
  background-color: #f44336;
  color: white;
}
</style>
