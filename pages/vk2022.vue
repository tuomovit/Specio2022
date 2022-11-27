<template>
  <div class="event">
    
        <div class="block bg hero-event">
            <div class="container">
                <div class="row">
                    <div class="col-12 col-lg-6">
                        <h1>Specion vuosikokous 2022</h1>
                        <h2 class="quote">Kaljaa ja softia -edition</h2>
                        <div class="event-info">
                            <h3 class="date">26-28.8 2022</h3>
                            <h3 class="location">Otava</h3>
                        </div>
                    </div>
                    <div class="col-12 offset-lg-1 col-lg-5">
                        <div class="image-wrapper">
                        <img class="blur" src="~/assets/images/vk22/vk2022-hero.JPG" />
                        <img class="image" src="~/assets/images/vk22/vk2022-hero.JPG" />
                        </div>
                    </div>
                </div>
            </div>
        </div>


        <div class="block gallery">
            <div class="container">
                <div class="row">
                    <div class="col-12 col-md-6 col-lg-4">
                        <div class="image-holder">
                            kuva
                        </div>
                    </div>
                    <div class="col-12 col-md-6 col-lg-4">
                        <div class="image-holder">
                            kuva
                        </div>
                    </div>
                    <div class="col-12 col-md-6 col-lg-4">
                        <div class="image-holder">
                            kuva
                        </div>
                    </div>
                    <div class="col-12 col-md-6 col-lg-4">
                        <div class="image-holder">
                            kuva
                        </div>
                    </div>
                    <div class="col-12 col-md-6 col-lg-4">
                        <div class="image-holder">
                            kuva
                        </div>
                    </div>   
                </div>
            </div>
        </div>
   
  </div>
</template>

<style lang="scss">

h1 {
    font-size: 2rem;
    @media (min-width: 1200px) { 
    font-size: 4rem;
   }
}

h1, h2 {
    font-weight: bold;
}

.event-info {
    margin-top: 3rem;
}

.image-wrapper {
    position: relative;
    width: 100%;
    padding-bottom: 120%;

    .blur {
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        object-fit: cover;
        border-radius: 8px;
        z-index: 0;
        background-size: cover;
        background-repeat: no-repeat;
        background-position: 50%;
        filter: blur(30px);
    }

    .image {
        position: absolute;
        top: 0;
        left: 0;
        object-fit: cover;
        border-radius: 8px;
        height: 100%;
        width: 100%;
        z-index: 1;
    }
}

.block {
    &.bg {
        padding-top: 6rem;
        padding-bottom: 6rem;
    }
    margin-bottom: 6rem;
}

.hero-event {
    background: linear-gradient(to bottom, #3b664c 65%, rgb(255, 255, 255) 35%);
    padding-bottom: 5rem;
}

.gallery {
    .image-holder {
        margin-bottom: 3rem;
    }
}

.quote {
    font-style: italic;
}

</style>

<script>

</script>
