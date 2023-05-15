<template>
    <div id="about" class="about-container">
        <div class="main__container-about">
            <div class="img-side">
                <img class="about__image" src="/about-img.webp" alt="">
                <img class="work-emoji" src="/working-emoji.ng.png" alt="">
                <span><img src="/text2.svg" alt="text"></span>
            </div>
            <div class="about__text">
                <div class="text-1 ">ABOUT ME</div>
                <div class="text-2">
                    <h3>A dedicated Front-end Developer based in Amman, Jordan 📍</h3>
                </div>
                <div class="text-3">As a Junior Front-End Developer, I possess an impressive arsenal of skills in HTML, CSS,
                    JavaScript,
                    Vue, Tailwind, and SCSS. I excel in designing and maintaining responsive websites that offer a smooth
                    user experience. My expertise lies in crafting dynamic, engaging interfaces through writing clean and
                    optimized code and utilizing cutting-edge development tools and techniques. I am also a team player who
                    thrives in collaborating with cross-functional teams to produce outstanding web applications.</div>
            </div>

        </div>
    </div>
</template>

<style>
.img-side span {
    background-color: #fff;
    border-radius: 50%;
    bottom: -33px;
    height: 11rem;
    position: absolute;
    right: -30px;
    width: 11rem;
}



.img-side {
    align-items: center;
    justify-content: center;
    display: flex;
}

.img-side span img {
    -webkit-animation: rotate 9s linear infinite;
    animation: rotate 9s linear infinite;
    width: 11rem;
}

@keyframes rotate {
    to {
        transform: rotate(360deg);
    }
}

.img-side {
    position: relative;
}

.work-emoji {
    bottom: 35px;
    position: absolute;
    right: 35px;
    width: 3rem !important;
    z-index: 3;
}

.text-3 {
    color: #767676;
    font-family: Mulish, sans-serif;
    font-size: 1.1rem;
    font-weight: 500;
    line-height: 1.5;
}

.text-2 {
    color: #2d2e32;
    font-family: Poppins, sans-serif;
    font-size: 1.5rem;
    line-height: 1.1;
    margin-bottom: 1rem;
}

.text-1 {
    color: #147efb;
    font-size: 1.1rem;
    font-weight: 800;
    margin-bottom: 1rem;
    text-transform: uppercase;
}

.about__text {
    width: 33rem;
    padding-inline-start: 4rem;
}

.about-container {
    align-items: center;
    margin: auto;
    margin-block: 10rem;
    justify-content: center;
}

.main__container-about {
    display: grid;
    grid-template-columns: 1fr 1fr;
    margin: auto;
    display: flex;
    justify-content: center;

}

.about__image {
    border-radius: 1.7rem;
    height: 350px;
    width: 410px;
}

@media (max-width: 900px) {
    
    .main__container-about {
        flex-direction: column;

    }

    .about__text {
        text-align: center;
        width: 33rem;
        padding-inline-start: 0;
    }

    .work-emoji {

        right: 100px;

    }

    .img-side span {

        right: 35px;
    }
}

@media (max-width: 550px) {
    .img-side span {
        display: none;
    }

    .work-emoji {
        display: none;
    }

    .about__text {
        text-align: center;
        width: 19rem;
        padding-inline-start: 0;
    }

    .about__image {
        border-radius: 1.7rem;
        height: 240px;
        width: 300px;
    }
}
</style>