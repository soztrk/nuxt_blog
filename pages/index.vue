<template>
  <!-- <Tutorial/> -->
  <div class="home-page">
    <section class="intro">
      <h1>Catch All News Now</h1>
    </section>
    <section class="featured-posts">
      <PostPreview
      id="1"
      thumbnail="https://images.unsplash.com/photo-1667956896405-de7027b24219?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1025&q=80"
      title="Hello Mello"
      previewText="This is the first post"
      />
    </section>
  </div>
</template>

<script>
import PostPreview from "~/components/posts/PostPreview"
export default{
components:{
  PostPreview
}
}
</script>

<style scoped lang="scss">
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
