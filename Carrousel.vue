<template>
  <ol v-if="!toggle">
        <li v-for ="images in images" :key="images">
          {{images}}
        </li>
  </ol>
</template>

<script>
  export default {
    data() {
      return {
        images: [
          '../Images/joker.png',
          '../Images/Flipper.png',
          '../Images/shell.png',
        ],
      };
    },
  };
</script>

<style>
  .example-slide {
    align-items: center;
    background-color: #666;
    color: #999;
    display: flex;
    font-size: 1.5rem;
    justify-content: center;
    min-height: 10rem;
  }
</style>