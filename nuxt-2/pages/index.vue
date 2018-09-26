<template>
  <div class="home-page">
      <section class="intro">
        <h1>Get the latest tech news!</h1>
      </section>
      <section class="featured-posts">
        <PostPreview 
        id="1"
        thumbnail="https://via.placeholder.com/950x150"
        title="Hello there!"
        previewText="This my first post!"/>
        <PostPreview 
        id="2"
        thumbnail="https://via.placeholder.com/950x150"
        title="Hello there! 2"
        previewText="This my first post! 2"/>
         <PostPreview 
        id="3"
        thumbnail="https://via.placeholder.com/950x150"
        title="Hello there! 3"
        previewText="This my first post! 3"/>
      </section>
  </div>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview';
export default{
  components:{
    PostPreview
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
