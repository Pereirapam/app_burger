<template>
    <div class="message-container">
        <p>{{ msg }}</p>
    </div>
</template>

<script>
export default {
  name: "Message",
  props: {
    msg: String
  }
}
</script>

<style scoped>
    .message-container {
        color: #004085;
        background-color: #cce5ff;
        border-color: #b8daff;
        padding: 10px;
        border-radius: 5px;
        margin: 30px;
        max-width: 400px;
        align-items: center;
    }
</style>