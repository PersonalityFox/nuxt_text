<template>
    <nuxt-link :to="'/posts/' + id">
        <article class="post-preview">
        <div class="post-thumbnail" :style="{backgroundImage: 'url('+thumbnail+')'}"></div>
        <div class="post-content">
            <h1>{{title}}</h1>
            <p>{{previewText}}</p>
        </div>
        </article>
    </nuxt-link>
</template>

<script>
export default{
    name: 'PostPreview',
    props: {
        id: {
            type: String,
            required: true
        },
        title: {
            type: String,
            required: true
        },
        previewText: {
            type: String,
            required: true
        },
        thumbnail: {
            type: String,
            required: true
        }
    }
}
</script>

<style scroped>
.post-preview{
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #ccc;
  width:90%;
  background-color: white;
}
.home-page{

}
.intro{

}
a{
  text-decoration: none;
  color:black;
}
.post-thumbnail{
  width:100%;
  height: 200px;
  background-position: center;
  background-size: cover;
}
.post-content{
  padding: 10px;
  text-align:center
}
</style>
