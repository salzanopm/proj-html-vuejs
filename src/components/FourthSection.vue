<template>
    <!-- start section -->
    <section id="live-dates" class="fourth-section"> 
        <!-- start wrapper -->
        <div class="container65">
            <h2>
                Live dates
            </h2>
            <hr>
            <p class="common-text-medium">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aperiam, obcaecati dolor aut dolore in beatae repudiandae illo qui. Animi sed fuga autem alias explicabo eveniet vitae quia nesciunt commodi exercitationem.
            </p>
            <!-- start list containers -->
            <div class="list-container">
                <div class="single-list">
                    <i v-on:click="open1=!open1" :class="{show:!open1}" class="fas fa-plus fa-xs"></i>
                    <i v-on:click="open1=!open1" :class="{show:open1}" class="fas fa-minus minus-container"></i>
                    <p class="text-primary-color common-text-big">17/08/2020 GEM festival 2020 anakalia, georgia</p>  
                </div>
                <div :class="{show:open1}" class="opensection">
                    <div class="img-container">
                        <img src="../assets/img/fss-demo-main.jpg" alt="">
                    </div>
                    <div class="text-container">
                        <h5>Untold Stories</h5>
                        <p class="common-text-medium">Lorem ipsum dolor sit amet consectetur adipisicing elit. Distinctio amet incidunt, aliquam autem error dolore repellat quisquam! Reprehenderit voluptate accusamus, veritatis aliquam aut iusto, id sint nostrum reiciendis dolorem sunt!</p>
                        <button class="button-red">Book now</button>
                    </div>
                </div>
            </div>
            <div class="list-container">
                <div class="single-list">
                    <i v-on:click="open3=!open3" :class="{show:!open3}" class="fas fa-plus fa-xs"></i>
                    <i v-on:click="open3=!open3" :class="{show:open3}" class="fas fa-minus minus-container"></i>
                    <p class="text-primary-color common-text-big">24/09/2020 groovefest dominical republic</p>  
                </div>
                <div :class="{show:open3}" class="opensection">
                    <div class="img-container">
                        <img src="../assets/img/fss-demo-main.jpg" alt="">
                    </div>
                    <div class="text-container">
                        <h5>Untold stories</h5>
                        <p class="common-text-medium">Lorem ipsum dolor sit amet consectetur adipisicing elit. Distinctio amet incidunt, aliquam autem error dolore repellat quisquam! Reprehenderit voluptate accusamus, veritatis aliquam aut iusto, id sint nostrum reiciendis dolorem sunt!</p>
                        <button class="button-red">Book now</button>
                    </div>
                </div>
            </div>
            <div class="list-container">
                <div class="single-list">
                    <i v-on:click="open4=!open4" :class="{show:!open4}" class="fas fa-plus fa-xs"></i>
                    <i v-on:click="open4=!open4" :class="{show:open4}" class="fas fa-minus minus-container"></i>
                    <p class="text-primary-color common-text-big">31/10/2020 oasis festival 2020 marrakech, morocco</p>  
                </div>
                <div :class="{show:open4}" class="opensection">
                    <div class="img-container">
                        <img src="../assets/img/fss-demo-main.jpg" alt="">
                    </div>
                    <div class="text-container">
                        <h5>Untold stories</h5>
                        <p class="common-text-medium">Lorem ipsum dolor sit amet consectetur adipisicing elit. Distinctio amet incidunt, aliquam autem error dolore repellat quisquam! Reprehenderit voluptate accusamus, veritatis aliquam aut iusto, id sint nostrum reiciendis dolorem sunt!</p>
                        <button class="button-red">Book now</button>
                    </div>
                </div>
            </div>
            <div class="list-container">
                <div class="single-list">
                    <i v-on:click="open5=!open5" :class="{show:!open5}" class="fas fa-plus fa-xs"></i>
                    <i v-on:click="open5=!open5" :class="{show:open5}" class="fas fa-minus minus-container"></i>
                    <p class="text-primary-color common-text-big">07/11/2020 moga festival essaquria, morocco</p>  
                </div>
                <div :class="{show:open5}" class="opensection">
                    <div class="img-container">
                        <img src="../assets/img/fss-demo-main.jpg" alt="">
                    </div>
                    <div class="text-container">
                        <h5>Untold stories</h5>
                        <p class="common-text-medium">Lorem ipsum dolor sit amet consectetur adipisicing elit. Distinctio amet incidunt, aliquam autem error dolore repellat quisquam! Reprehenderit voluptate accusamus, veritatis aliquam aut iusto, id sint nostrum reiciendis dolorem sunt!</p>
                        <button class="button-red">Book now</button>
                    </div>
                </div>
            </div>
            <div class="list-container">
                <div class="single-list">
                    <i v-on:click="open2=!open2" :class="{show:!open2}" class="fas fa-plus fa-xs"></i>
                    <i v-on:click="open2=!open2" :class="{show:open2}" class="fas fa-minus minus-container"></i>
                    <p class="text-primary-color common-text-big">10/12/2021 envision festival - uvita, costa rica</p>  
                </div>
                <div :class="{show:open2}" class="opensection">
                    <div class="img-container">
                        <img src="../assets/img/fss-demo-main.jpg" alt="">
                    </div>
                    <div class="text-container">
                        <h5>Untold stories</h5>
                        <p class="common-text-medium">Lorem ipsum dolor sit amet consectetur adipisicing elit. Distinctio amet incidunt, aliquam autem error dolore repellat quisquam! Reprehenderit voluptate accusamus, veritatis aliquam aut iusto, id sint nostrum reiciendis dolorem sunt!</p>
                        <button class="button-red">Book now</button>
                    </div>
                </div>
            </div>
            <!-- end list containers -->
        </div>
        <!-- end wrapper -->
    </section>
    <!-- end section -->
</template>

<script>

export default {
    name: "FourthSection",
     data() {
        return {
            open1:true,
            open2:true,
            open3:true,
            open4:true,
            open5:true
        }
    }
};
</script>

<style scoped lang="scss">
    @import "../style/Variables.scss";
    section {
        
        background-color: $brand_tertiary_color;

        hr {
            margin: 0 15px 15px 15px;
        }

        i {
            padding: 0 10px;
            margin: 5px;
        }
    }

    h5 {
        margin: 5px 0;
        
    }

    .minus-container {
        height: 20px;
        width: 20px;
        background-color: $brand_primary_color;
        display: flex;
        justify-content: center;
        align-items: center;
        
    }
    


    .single-list {
        display: flex;
        align-items: center;
        background-color: $brand_secondary_color;
        padding: 5px;
        margin-top: 20px;
    }

    .text-primary-color {
        color: $brand_primary_color;
        text-transform: uppercase;
    }

    .opensection {
        position: relative;
        background-color: $brand_secondary_color;
        height: 100px;
    }
    .img-container {
        width: 100px;
        height: 60px;
        position: absolute;
        top: 5px;
        left: 20px;
    }
    .text-container {
        position: absolute;
        top: -10px;
        left: 150px;
        text-align: left;
        margin-bottom: 20px;
    }
    .show {
        display: none;
    }

    button {
        margin: 8px 0;
    }


</style>