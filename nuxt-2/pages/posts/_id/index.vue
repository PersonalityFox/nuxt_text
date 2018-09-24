<template>
    <div class="single-post-page">
        <section class="post">
            <h1 class="post-title">Title post</h1>
            <div class="post-details">
                <div class="post-detail">Last update in XXX</div>
                <div class="post-detail">Written by Name</div>
            </div>
            <p class="post-content">Content of the post</p>
        </section>
        <section class="post-feedback">
            <p>Let me know what you thing about the post, send a mail to <a href="mailto:feedbacl@myemail.com">feedbacl@myemail.com</a></p>
        </section>
    </div>
</template>

<style>
.single-post-page{
     padding: 30px;
      text-align: center;
      box-sizing: border-box;
}
.post{
    width:100%;
}
    .post-title{
        margin:0;
    }
    .post-details{
        padding: 10px;
        box-sizing: border-box;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }
    
</style>