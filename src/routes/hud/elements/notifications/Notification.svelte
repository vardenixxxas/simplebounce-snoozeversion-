<script lang="ts">
    export let title: string;
    export let message: string;
</script>

<div class="notification">
    <div class="title">{title}</div>
    <div class="message">{message}</div>
</div>

<style lang="scss">
  .notification {
    display: grid;
    grid-template-areas:
            "a" 
            "b";
    grid-template-columns: max-content 1fr;
    border-left: 2px solid rgb(127, 0, 255);
    column-gap: 10px;
    background: rgba(24, 24, 24, 1.0);
    width: 300px;
    overflow: hidden;
    padding: 10px;
    margin-bottom: 10px;
  }

  
  .title {
    grid-area: a;
    font-size: 12px;
    color: white;
    text-shadow: rgba(128,0,255,0.9) 0px 0px 12px;
  }

  .message {
    grid-area: b;
    font-size: 12px;
    color: #cbd1e3;
  }
</style>
