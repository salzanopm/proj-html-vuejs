<template>
    <section class="second-section"> 
        <div class="container65">
            <h2 class="upperline">
                Music is life
            </h2>
            <hr>
            <p class="common-text2">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aperiam, obcaecati dolor aut dolore in beatae repudiandae illo qui. Animi sed fuga autem alias explicabo eveniet vitae quia nesciunt commodi exercitationem.
            </p>
        </div>
    </section>
</template>

<script>

export default {
    name: "FirstSection",
};
</script>

<style scoped lang="scss">
    @import "../style/Variables.scss";
    section {
        height: 225px;
        background-color: $brand_secondary_color;

       
        h2.upperline {
          border-top: solid 10px $brand_primary_color;
          padding-top: 30px;
          margin: 0 200px;
        }

        hr {
            margin: 0 15px 15px 15px;
        }

        p {
            margin: 10px;
        }
        .container65 {
        padding-top: 0;
        }
    }
    
</style>