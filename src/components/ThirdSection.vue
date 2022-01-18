<template>
    <section id="meet-the-band">
        <div class="content">
            <p class="quote">
                "I just listened to it and said to myself,"Man I really love this
                album."Stil, today, it just sound so fresh. It sounds full of ideas"
                these guys knew what they were doing. They're good. And they're 
                inventive. I haven't heard anything this year that as inventive I really don't expect to"
            </p>
            <div class="img-container">
                <img src="../assets/img/band_interview_play_icon.png" alt="play image">
            </div>
        </div>
    </section>
</template>

<script>

export default {
    name: "ThirdSection",
};
</script>

<style scoped lang="scss">
    @import "../style/Variables.scss";
    section {
        height: 450px;
        background-image: url('../assets/img/home-testimonial-parallax.jpg');
        text-align: center;
        display: flex;
        align-items: center;
    }
    .quote {
        font-style: oblique;
        width: 35%;
        margin: auto;
    }

    .img-container {
        height: 50px;
        width: 50px;
        display: inline-block;
        margin: 20px
    }
    
</style>