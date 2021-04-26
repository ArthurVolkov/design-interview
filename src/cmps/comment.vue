
<template>
  <div class="flex flex flex-col justify-center align-center comment">
    <p>{{ comment.txt }}</p>
    <div class="flex justify-center align-center">
      <img :src="getImgUrl(comment.imgUrl)" alt="" />
      <div class="flex flex-col">
          <h4>{{comment.name}}</h4>
          <p>{{comment.position}}</p>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: "comment",
  props: {
    comment: Object
  },
  data() {
    return {

    }

  },
  methods: {
    getImgUrl(pic) {
      return require('../assets/' + pic)
    },
  }


};
</script>
