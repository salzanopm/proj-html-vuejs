<template>
    <section id="live-dates" class="fourth-section"> 
        <div class="container65">
            <h2>
                Live dates
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
    name: "FourthSection",
};
</script>

<style scoped lang="scss">
    @import "../style/Variables.scss";
    section {
        height: 225px;
        background-color: $brand_secondary_color;

        hr {
            margin: 0 15px 15px 15px;
        }

        p {
            margin: 10px;
        }
    }
    
</style>