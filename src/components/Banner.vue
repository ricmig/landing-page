<template>
<div class="banner-container__uol">
    <div class="banner-content__uol d-flex justify-content-center align-items-center flex-column pt-4">
        <img width="250" src="../assets/logos.png" alt="logos da NFL e do Espm Play">
        <div class="d-flex justify-content-center align-items-center flex-column py-2 pt-2 pb-4 jumbotron-fluid">
            <p class="font-weight-bold text-white text-uppercase m-0 h2">assita ao vivo</p>
            <p class="h4 text-white text-uppercase m-0">aos jogos da nfl</p>
        </div>
    </div>
</div>
</template>

<style>

.banner-container__uol{
    background: linear-gradient(0deg, rgb(54, 169, 319), rgba(49, 141, 255, 0.88)), url(/static/img/bg-top.fe6f12e.jpg);
    background-position: calc(50% - 15rem);
    min-height: 65vh;
}

.banner-content__uol{
    width: 100%;
}

@media only screen and (min-width: 992px) {
    .banner-container__uol{
        background: url(/static/img/bg-top.fe6f12e.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        min-height: 420px;
    }
    .banner-content__uol {
        width: 30rem;
        margin-left: 15%;
    }
}

</style>