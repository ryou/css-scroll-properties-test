<template>
  <div class="PhotoList">
    <div v-for="image in images" :key="image.id" class="PhotoList_item"><img :src="image.src"></div>
  </div>
</template>

<script>
import HelloWorld from '../components/HelloWorld.vue';

export default {
  data() {
    return {
      images: [
        {
          id: 0,
          src: 'https://picsum.photos/400/300/?image=0',
        },
        {
          id: 1,
          src: 'https://picsum.photos/400/300/?image=10',
        },
        {
          id: 2,
          src: 'https://picsum.photos/400/300/?image=20',
        },
        {
          id: 3,
          src: 'https://picsum.photos/400/300/?image=30',
        },
        {
          id: 4,
          src: 'https://picsum.photos/400/300/?image=40',
        },
      ],
    };
  },
  components: {
    HelloWorld,
  },
};
</script>

<style lang="scss" scoped>
.PhotoList {
  display: flex;
  overflow-x: scroll;

  scroll-snap-type: x mandatory;
}
.PhotoList_item {
  flex-shrink: 0;
  flex-grow: 0;
  flex-basis: 100%;

  scroll-snap-align: center;

  img {
    vertical-align: top;
    width: 100%;
  }
}
</style>

