<template>
    <div class="single-post-page">
        <section class="post">
            <h1 class="post-title">Title of Post</h1>
            <div class="post-details">
                <div class="post-detail">Last updated on XXXX</div>
                <div class="post-detail">Written by NAME</div>
            </div>
            <p class="post-content">
                Content of post
            </p>
        </section>
        <section class="post-feedback">
            <p> 
                Feedback text 
            </p>
            <a href="mailto:s.ozturk999@gmail.com">Mail me everything</a>
        </section>
    </div>
</template>
<style scoped lang="scss">
.single-post-page {
  padding: 30px;
  text-align: center;
  box-sizing: border-box;
}

.post {
  width: 100%;
}

@media (min-width: 768px) {
  .post {
    width: 600px;
    margin: auto;
  }
}

.post-title {
  margin: 0;
}

.post-details {
  padding: 10px;
  box-sizing: border-box;
  border-bottom: 3px solid #ccc;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

@media (min-width: 768px) {
  .post-details {
    flex-direction: row;
  }
}

.post-detail {
  color: rgb(88, 88, 88);
  margin: 0 10px;
}

.post-feedback a {
  color: $secondaryColor;
  text-decoration: none;
}

.post-feedback a:hover,
.post-feedback a:active {
  color: $secondaryColorLight;
}
</style>