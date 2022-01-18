<template>
    <section class="second-section"> 
        <div class="container65">
            <h2 class="upperline">
                Latest band news
            </h2>
            <hr>
            <p class="common-text2">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aperiam, obcaecati dolor aut dolore in beatae repudiandae illo qui. Animi sed fuga autem alias explicabo eveniet vitae quia nesciunt commodi exercitationem.
            </p>
            <div class="picture-section">
                <div class="row">
                    <div class="left-column">
                        <div class="box">
                            <div class="top-box">

                            </div>
                            <div class="middle-box">
                                <div class="case">
                                    <div class="left-case">

                                    </div>
                                    <div class="right-case">

                                    </div>
                                </div>
                            </div>
                            <div class="bottom-box">

                            </div>
                        </div>
                    </div>
                    <div class="right-column">
                        <div class="row">
                            <div class="up-row">

                            </div>
                            <div class="down-row">

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
        border: solid 1px black;
        margin: 30px 0;

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
        height: 50%;
    }

    div[class$="-case"] {
        float: left;
        height: 100%;
    }

    div[class$="-box"] {
        float: left;
        width: 100%;
    }

    .top-box {
        height: 25%;
        border: solid 1px white;
    }

    .bottom-box {
        height: 25%;
        border: solid 1px white;
    }

    .middle-box {
        height: 50%;
        border: solid 1px white;
    }

    .left-case {
        width: 50%;
        border: solid 1px white;
    }

    .right-case {
        width: 50%;
        border: solid 1px white;
    }



    .up-row {
        width: 100%;
        border: solid 1px white;
    }

    .down-row {
        width: 100%;
        border: solid 1px white;
    }


    .left-column {
        width: 65%;
        border: solid 1px white;
    }

    .right-column {
        width: 35%;
        border: solid 1px green;
    }





</style>