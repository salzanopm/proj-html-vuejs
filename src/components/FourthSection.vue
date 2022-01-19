<template>
    <section id="live-dates" class="fourth-section"> 
        <div class="container65">
            <h2>
                Live dates
            </h2>
            <hr>
            <p class="common-text-medium">
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aperiam, obcaecati dolor aut dolore in beatae repudiandae illo qui. Animi sed fuga autem alias explicabo eveniet vitae quia nesciunt commodi exercitationem.
            </p>
            <div class="list-container">
                <div class="single-list">
                    <i v-on:click="open1=!open1" class="fas fa-plus fa-xs"></i>
                    <p class="text-primary-color">nffoiefofoeof</p>  
                </div>
                <div :class="{show:open1}" class="opensection">
                    <div class="img-container">
                        <img src="../assets/img/fss-demo-main.jpg" alt="">
                    </div>
                    <div class="text-container">
                        <h5>dnfknifief</h5>
                        <p>dnifbifv</p>
                    </div>
                </div>
            </div>
            <div class="list-container">
                <div class="single-list">
                    <i v-on:click="open2=!open2" class="fas fa-plus fa-xs"></i>
                    <p class="text-primary-color">nffoiefofoeof</p>  
                </div>
                <div :class="{show:open2}" class="opensection">
                    <div class="img-container">
                        <img src="../assets/img/fss-demo-main.jpg" alt="">
                    </div>
                    <div class="text-container">
                        <h5>dnfknifief</h5>
                        <p>dnifbifv</p>
                    </div>
                </div>
            </div>
            <div class="list-container">
                <div class="single-list">
                    <i v-on:click="open3=!open3" class="fas fa-plus fa-xs"></i>
                    <p class="text-primary-color">nffoiefofoeof</p>  
                </div>
                <div :class="{show:open3}" class="opensection">
                    <div class="img-container">
                        <img src="../assets/img/fss-demo-main.jpg" alt="">
                    </div>
                    <div class="text-container">
                        <h5>dnfknifief</h5>
                        <p>dnifbifv</p>
                    </div>
                </div>
            </div>
            <div class="list-container">
                <div class="single-list">
                    <i v-on:click="open4=!open4" class="fas fa-plus fa-xs"></i>
                    <p class="text-primary-color">nffoiefofoeof</p>  
                </div>
                <div :class="{show:open4}" class="opensection">
                    <div class="img-container">
                        <img src="../assets/img/fss-demo-main.jpg" alt="">
                    </div>
                    <div class="text-container">
                        <h5>dnfknifief</h5>
                        <p>dnifbifv</p>
                    </div>
                </div>
            </div>
            <div class="list-container">
                <div class="single-list">
                    <i v-on:click="open5=!open5" class="fas fa-plus fa-xs"></i>
                    <p class="text-primary-color">nffoiefofoeof</p>  
                </div>
                <div :class="{show:open5}" class="opensection">
                    <div class="img-container">
                        <img src="../assets/img/fss-demo-main.jpg" alt="">
                    </div>
                    <div class="text-container">
                        <h5>dnfknifief</h5>
                        <p>dnifbifv</p>
                    </div>
                </div>
            </div>
            <div class="list-container">
                <div class="single-list">
                    <i v-on:click="open6=!open6" class="fas fa-plus fa-xs"></i>
                    <p class="text-primary-color">nffoiefofoeof</p>  
                </div>
                <div :class="{show:open6}" class="opensection">
                    <div class="img-container">
                        <img src="../assets/img/fss-demo-main.jpg" alt="">
                    </div>
                    <div class="text-container">
                        <h5>dnfknifief</h5>
                        <p>dnifbifv</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>

export default {
    name: "FourthSection",
     data() {
        return {
            open1:false,
            open2:false,
            open3:false,
            open4:false,
            open5:false
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
        }
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
        bottom: 20px;
        left: 20px;
    }
    .text-container {
        position: absolute;
        top: 20px;
        left: 150px;
        text-align: left;
    }
    .show {
        display: none;
    }


</style>