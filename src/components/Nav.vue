<template>
    <div id="nav" class="row p-md-5 p-3 m-0 w-100">
        <nav class="navbar navbar-expand-sm w-100 sticky-top navbar-light">
            <a class="navbar-brand mr-auto" href="/" data-toggle="tooltip" data-placement="bottom" title="Home"> 
                <img src="../assets/images/logo.svg" class="logo">
            </a>
            <button class="navbar-toggler d-lg-none" type="button" data-toggle="collapse" data-target="#collapsibleNavId" aria-controls="collapsibleNavId"
                aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class=" collapse navbar-collapse" id="collapsibleNavId">
                <ul class="navbar-nav px-4 ml-auto mt-2 mt-lg-0">
                    <li class="nav-item mx-4"> 
                        <a class="nav-link text-dark" href="/about ">About </a>
                    </li>
                    <li class="nav-item mx-4">
                        <a class="nav-link text-dark" href="/work ">Work </a>
                    </li>
                    <li class="nav-item mx-4">
                        <a class="nav-link text-dark" href="/services ">Services </a>
                    </li>
                    <li class="nav-item mx-4">
                        <a class="nav-link text-dark" href="/team ">Team </a>
                    </li>
                    <li class="nav-item mx-4">
                        <a class="nav-link text-dark" href="/contacts ">Contacts </a>
                    </li>
                </ul>                
            </div>
        </nav>
    </div>
</template>

<script>
export default {
    name: 'Nav'
}
</script>

<style>
.logo
{
    max-width: 8vw;
}



@media screen and (max-width: 820px) {

        .logo
        {
            max-width: 25vw;
        }
}

</style>