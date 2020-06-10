<template>
<div class="banner-container__uol">
    <div class="banner-content__uol w-100 d-flex justify-content-center align-items-center flex-column p-5">
        <img width="250" src="../assets/logos.png" alt="logos da NFL e do Espm Play">
        <div class="d-flex justify-content-center align-items-center flex-column py-2 pt-2 pb-4 jumbotron-fluid">
            <p class="font-weight-bold text-white text-uppercase m-0 h2 py-2">assita ao vivo</p>
            <p class="h4 text-white text-uppercase m-0">aos jogos da nfl</p>
            <p class="h5 max-w-150 text-white text-center m-0 py-3" style="max-width:500px; line-height:2.5rem;">Com o <span class="font-weight-bold">Com o UOL Esporte Clube</span>, você assiste aos principais jogos do Monday Night Football da NFL no <span class="font-weight-bold">ESPM Play</span></p>
            <div class="max-w-50 d-flex justify-content-around align-items-end">
                <div class="d-flex flex-column align-items-center">
                    <img class="w-75" src="../assets/ico.png" alt="logo time 1">
                    <p class="w-100 h6 text-white text-center font-weight-bold" style="min-width:96px;">New England Patriots</p>
                </div>
                <div class="d-flex flex-column align-items-center">
                    <button type="button" class="btn btn-danger h6 text-white text-center font-weight-bold">Próximo jogo</button>
                    <p class="h6 text-white text-center font-weight-bold">11/11 | 11h11</p>
                    <p class="h1 mt-0 text-danger text-white text-center font-weight-bold">X</p>
                </div>
                <div class="d-flex flex-column align-items-center">
                    <img class="w-75" src="../assets/ico2.png" alt="logo time 1">
                    <p class="w-100 h6 text-white text-center font-weight-bold" style="min-width:96px;">Philadelphia Eagles</p>
                </div>     
            </div>
            <button type="button" class="text-uppercase btn w-100 h6 text-center text-black font-weight-bold py-3 my-2" style="background-color: #ffb32f; max-width: 350px;">Experimente por 1 Mês</button>
            <p class="text-white">Após período, R$ 24,90/mês</p>    
        </div>
    </div>
</div>
</template>

<style>

.banner-container__uol{
    background: linear-gradient(0deg, rgb(54, 169, 319), rgba(49, 141, 255, 0.88)), url('../assets/bg-top.jpg');
    background-position: calc(50% - 15rem);
    min-height: 60vh;
}

@media only screen and (min-width: 992px) {
    .banner-container__uol{
        background: url('../assets/bg-top.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        min-height: 420px;
    }

    .banner-content__uol {
        width: 33rem !important;
        margin-left: 15%;
    }
}

</style>