<template>
<!-- start section -->
    <section id="latest-news" class="second-section"> 
        <!-- start wrap container -->
        <div class="container65">
            <!-- start title part -->
            <h2 class="upperline">
                Latest band news
            </h2>
            <hr>
            <p class="common-text-medium">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aperiam, obcaecati dolor aut dolore in beatae repudiandae illo qui. Animi sed fuga autem alias explicabo eveniet vitae quia nesciunt commodi exercitationem.
            </p>
            <!-- end title part -->
            <!-- start picture part -->
            <div class="picture-section">
                <div class="row">
                    <div class="left-column">
                        <div class="box">
                            <!-- start first card top left -->
                            <div class="single-card-top-box">
                                <div class="overlay"></div>
                                <div class="text-card">
                                    <h5>Tecnology and music</h5>
                                    <p class="common-text-medium">sed sit amet sent turpis curabitur cursur lacinia est at interdum risus id condimentum</p>
                                </div>
                            </div>
                            <!-- end first card top left -->
                            <div class="middle-box">
                                <div class="case">
                                    <!-- start second card middle left -->
                                    <div class="single-card-left-case">
                                        <div class="overlay"></div>
                                        <div class="text-card">
                                            <h5>Taking it back to the old school</h5>
                                            <p class="common-text-medium">sed sit amet sent turpis curabitur cursur lacinia est at interdum risus id condimentum</p>
                                        </div>  
                                    </div>
                                    <!-- end second card middle left -->
                                    <!-- start third card middle right -->
                                    <div class="single-card-right-case">
                                        <div class="overlay"></div>
                                        <div class="text-card">
                                            <h5>While my guitar gently weeps</h5>
                                            <p class="common-text-medium">sed sit amet sent turpis curabitur cursur lacinia est at interdum risus id condimentum</p>
                                        </div>
                                    </div>
                                    <!-- end third card middle right -->
                                </div>
                            </div>
                            <!-- start fourth card bottom left -->
                            <div class="single-card-bottom-box">
                                <div class="overlay"></div>
                                <div class="text-card">
                                    <h5>It just sounds better</h5>
                                    <p class="common-text-medium">sed sit amet sent turpis curabitur cursur lacinia est at interdum risus id condimentum</p>
                                </div>
                            </div>
                            <!-- end third card middle right -->
                        </div>
                    </div>
                    <div class="right-column">
                        <div class="row">
                            <!-- start fifth card top right -->
                            <div class="single-card-up-row">
                                <div class="overlay"></div>
                                <div class="text-card">
                                    <h5>The flavor of rock</h5>
                                    <p class="common-text-medium">sed sit amet sent turpis curabitur cursur lacinia est at interdum risus id condimentum</p>
                                </div>
                            </div>
                            <!-- end fifth card top right -->
                            <!-- start sixth card bottom right -->
                            <div class="single-card-down-row">
                                <div class="overlay"></div>
                                <div class="text-card">
                                    <h5>Sharing the stage with a legend</h5>
                                    <p class="common-text-medium">sed sit amet sent turpis curabitur cursur lacinia est at interdum risus id condimentum</p>
                                </div>
                            </div>
                            <!-- end sixth card bottom right -->
                        </div>
                    </div>
                </div>
            </div>
            <!-- end picture part -->
        </div>
        <!-- end wrap container -->
    </section>
    <!-- end section -->
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
            margin-top: 5px;
            margin-left: 5px;
        }
    }  

    .picture-section {
        height: 850px;
        margin: 30px 0;
        text-align: left;
    }

    // wrap containers
    .row {
        height: inherit;
    }

    .box {
        height: 100%;
    }

    .case {
        height: 100%;
    }

    // clearfix
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

    // common style wrap containers child
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

    // box cards
    .single-card-top-box {
        height: calc(25% - 5px);
        background-image: url('../assets/img/blog_music_techo.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        position: relative;
        margin-bottom: 5px;
    }

    .middle-box {
        height: calc(50% - 10px);
        margin: 5px 0;
    }

    .single-card-bottom-box {
        height: calc(25% - 5px);
        background-image: url('../assets/img/blog_flavor_rock.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        position: relative;
        margin-top: 5px;
    }

    // case cards
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

    // row cards
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

    // columns
    .left-column {
        width: calc(65% - 5px);
        margin-right: 5px;
    }

    .right-column {
        width: calc(35% - 5px);
        margin-left: 5px;
    }

    // overlay
    .overlay {
        display: none;
        background-color: rgba(230, 100, 100, .5);
        width: 100%;
        height: 100%;        
    }

    // common
    .text-card {
        position: absolute;
        bottom: 0;
        width: 100%;
        height: 60px;
        display: flex;
        flex-direction: column;
        background-color: $brand_secondary_color;
    }

    div[class^="single-card"]:hover .overlay {
        display: block;
    }

    // overwrite
    h5 {
        height: 50%;
        margin-top: 5px;
        margin-left: 5px;
        color: $brand_primary_color;
    }
</style>