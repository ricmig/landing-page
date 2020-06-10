<template>
    <div>
        <div>
            <div class="bg-light w-100 h-100 px-5 py-2 div-container__uol">
                <div v-for="(card, index) in contentInfo" :key="index" :id="id" class="div-content__uol">
                    <a class="text-black d-flex justify-content-around align-items-center" :href="card.link.url">
                        <div class="d-flex" style="max-width:270px; line-height: 2.2rem;">
                            <img class="h-100" :src="card.src" :alt='`imagem sobre ${card.id}`'>
                            <span class="pl-4 d-flex align-items-center position-relative">
                                <div class="border-content__uol position-absolute"></div>
                                <p class="m-0 h6 text-black">{{card.text}}</p>
                            </span>
                        </div>
                    </a>
                </div>
            </div>
            <div class="square-content__uol bg-light"></div>
        </div>
        <div class="d-flex justify-content-around align-items-center flex-column p-4">
            <p class="h5 text-center mb-3">No UOL Esporte Clube você tem:</p>
            <div class="w-100 d-flex card-content__uol pb-5">
                <div class="bg-light m-4 d-flex flex-column justify-content-around align-items-center">
                    <span class="bg-darkgray-100 w-100 h-100 d-flex align-items-center justify-content-center">
                        <img src="../assets/ico2.png" alt="logo time 1" width="50">
                    </span>
                    <img class="py-3" src="../assets/logos.png" width="200" >
                    <span class="bg-darkgray-100 w-100 h-100 d-flex align-items-center justify-content-center">
                        <img src="../assets/espnlogo.png" alt="logo time 1" width="100">
                    </span>
                </div>
                <div class="bg-light m-4 d-flex flex-column justify-content-around align-items-center">
                    <span class="bg-darkgray-100 w-100 h-100 d-flex align-items-center justify-content-center">
                        <img src="../assets/ico2.png" alt="logo time 1" width="50">
                    </span>                    
                    <img class="py-3" src="../assets/logos.png" width="200">
                    <span class="bg-darkgray-100 w-100 h-100 d-flex align-items-center justify-content-center">
                        <img src="../assets/espnlogo.png" alt="logo time 1" width="100">
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props:{
        contentInfo:{
            type:Object,
            required:true
        }
    }
}
</script>

<style>
    .square-content__uol{
        width: 30px;
        height: 30px;
        margin: auto;
        -webkit-transform: rotate(45deg);
        transform: rotate(45deg);
        position: relative;
        bottom: 15px;
    }

    .div-content__uol{
        width:100%;
        margin: 20px 10px 10px;
    }

    .card-content__uol{
        flex-direction: column;
    }

    .card-content__uol div{
        height: 200px;
    }

    @media only screen and (min-width: 992px) {
    .div-content__uol{
        width:30%;
    }

    .div-container__uol{
        display: flex;
        padding:4rem !important;
    }

    .card-content__uol{
        flex-direction: row;
        justify-content: center;
    }

    .card-content__uol div{
        width: 33%;
    }
    
}

    .border-content__uol {
        height: 30px;
        width: 3px;
        left: 6px;
        background-color: #a51c1c;
    }

    .bg-darkgray-100{
        background-color: #eaeeef;
    }

</style>