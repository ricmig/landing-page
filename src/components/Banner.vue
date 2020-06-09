<template>
<div class="banner-container__uol">
</div>
</template>

<style>
.banner-container__uol{
    background: linear-gradient(0deg, rgb(54, 169, 319), rgba(49, 141, 255, 0.88)), url(/static/img/bg-top.fe6f12e.jpg);
    background-position: calc(50% - 15rem);
    min-height: 65vh;
}

@media only screen and (min-width: 992px) {
    .banner-container__uol{
        background: url(/static/img/bg-top.fe6f12e.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        min-height: 420px;
    }
}


</style>