<template>
    <section id="latest-news" class="second-section"> 
        <div class="container65">
            <h2 class="upperline">
                Latest band news
            </h2>
            <hr>
            <p class="common-text-medium">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aperiam, obcaecati dolor aut dolore in beatae repudiandae illo qui. Animi sed fuga autem alias explicabo eveniet vitae quia nesciunt commodi exercitationem.
            </p>
            <div class="picture-section">
                <div class="row">
                    <div class="left-column">
                        <div class="box">
                            <div class="single-card-top-box">
                                <div class="overlay"></div>
                                <div class="text-card">
                                    <h5>weweewewe</h5>
                                    <p class="common-text-medium">efffeef</p>
                                </div>
                            </div>
                            <div class="middle-box">
                                <div class="case">
                                    <div class="single-card-left-case">
                                        <div class="overlay"></div>
                                        <div class="text-card">
                                        <h5>weweewewe</h5>
                                        <p class="common-text-medium">efffeef</p>
                                    </div>  
                                    </div>
                                    <div class="single-card-right-case">
                                        <div class="overlay"></div>
                                        <div class="text-card">
                                            <h5>weweewewe</h5>
                                            <p class="common-text-medium">efffeef</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="single-card-bottom-box">
                                <div class="overlay"></div>
                                <div class="text-card">
                                    <h5>weweewewe</h5>
                                    <p class="common-text-medium">efffeef</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="right-column">
                        <div class="row">
                            <div class="single-card-up-row">
                                <div class="overlay"></div>
                                <div class="text-card">
                                    <h5>weweewewe</h5>
                                    <p class="common-text-medium">efffeef</p>
                                </div>
                            </div>
                            <div class="single-card-down-row">
                                <div class="overlay"></div>
                                <div class="text-card">
                                    <h5>weweewewe</h5>
                                    <p class="common-text-medium">efffeef</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "SecondSection",
};
</script>

<style scoped lang="scss">
    @import "../style/Variables.scss";
    section {
        
        background-color: $brand_tertiary_color;

        hr {
            margin: 0 15px 15px 15px;
        }

        p {
            margin: 10px;
        }
    }  

    .picture-section {
        height: 850px;
        margin: 30px 0;
        text-align: left;
    }

    .row {
        height: inherit;
    }

    .box {
        height: 100%;
    }

    .case {
        height: 100%;
    }

    .box:after {
        content: '';
        display: table;
        clear: both;
    }

    .row:after {
        content: '';
        display: table;
        clear: both;
    }

    .case:after {
        content: '';
        display: table;
        clear: both;
    }


    div[class$="-column"] {
        float: left;
        height: 100%;
    }

    div[class$="-row"] {
        float: left;
        height: calc(50% - 5px);
    }

    div[class$="-case"] {
        float: left;
        height: 100%;
    }

    div[class$="-box"] {
        float: left;
        width: 100%;
    }

    .single-card-top-box {
        height: calc(25% - 5px);
        background-image: url('../assets/img/blog_music_techo.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        position: relative;
        margin-bottom: 5px;
        

    }

    .single-card-bottom-box {
        height: calc(25% - 5px);
        background-image: url('../assets/img/blog_flavor_rock.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        position: relative;
        margin-top: 5px;
    }

    .middle-box {
        height: calc(50% - 10px);
        margin: 5px 0;
    }

    .single-card-left-case {
        width: calc(50% - 5px);
        background-image: url('../assets/img/blog-post3.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        position: relative;
        margin-right: 5px;
    }

    .single-card-right-case {
        width: calc(50% - 5px);
        background-image: url('../assets/img/blog-post4.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        position: relative;
        margin-left: 5px;
    }



    .single-card-up-row {
        width: 100%;
        height: calc(100% - 5px);
        background-image: url('../assets/img/blog-post1.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        position: relative;
        margin-bottom: 5px;
    }

    .single-card-down-row {
        width: 100%;
        height: calc(100% - 5px);
        background-image: url('../assets/img/blog-post2.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        position: relative;
        margin-top: 5px;
    }


    .left-column {
        width: calc(65% - 5px);
        margin-right: 5px;
    }

    .right-column {
        width: calc(35% - 5px);
        margin-left: 5px;
    }

    .text-card {
        position: absolute;
        bottom: 0;
        width: 100%;
        height: 60px;
        display: flex;
        flex-direction: column;
        background-color: $brand_secondary_color;
    }

    .overlay {
        display: none;
        background-color: rgba(230, 100, 100, .5);
        width: 100%;
        height: 100%;        
    }
    div[class^="single-card"]:hover .overlay {
        display: block;
    }

    h5 {
        height: 50%;
        padding: 10px;
        color: $brand_primary_color;
    }

   





</style>