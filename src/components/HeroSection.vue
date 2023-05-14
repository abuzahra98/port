<template>
    <div class="hero" id="home">
        <div class="main__container">
            <div class=" content">
                <div class="hero-main">
                    <div class="hero-text">
                        <h1>Front-End Web Developer</h1>
                        <img class="hero__wave" src="/waving.png" alt="waving_hand" />
                        <p>
                            Hi, I'm Dawood Abuzahra. A passionate Front-end Web Developer based
                            in Amman, Jorden. 📍
                        </p>
                        <div class="any">
                            <a aria-label="linkedin" rel="noreferrer" target="_blank" href="https://github.com/abuzahra98">
                                <img class="hero-icon" src="/GitHub.png" alt="">
                            </a>
                            <a aria-label="github" rel="noreferrer" target="_blank"
                                href="https://www.linkedin.com/in/dawood-abuzahra/">
                                <img class="hero-icon" src="/linkedin.png" alt="">
                            </a>
                        </div>
                    </div>
                    <div class="hero-img">

                    </div>
                </div>

                <div class="skills">
                    <p>Tech Stack</p>
                    <div class="logos">
                        <ul>
                            <li><img src="/html.svg" title="HTML5" alt="program_img">
                            </li>
                            <li><img src="/css3.svg" title="CSS3" alt="program_img">
                            </li>
                            <li><img src="/javascript.svg" title="Javascript" alt="program_img"></li>
                            <li><img src="/react.svg" title="React JS" alt="program_img"></li>
                            <li><img src="/tailwind.svg" title="Tailwind CSS" alt="program_img"></li>
                            <li><img src="/scss.svg" title="Sass/Scss" alt="program_img"></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
.any {
    cursor: pointer;
    display: flex;
    gap: 1.3rem;
    margin: 2.5rem 0;
}

.hero-icon {
    width: 3rem;
    margin-inline-end: 1rem;
}

.content {
    margin-top: 5rem;
    align-items: center;
    display: flex;
    gap: 10rem;
    height: 35rem;
    justify-content: center;
    position: relative;
}

@media (min-width: 1900px) {
    .content {
        margin-top: 10rem;
    }
}

.hero {
    background-color: #f9f9f9;
    display: flex;
    flex-direction: column;
    height: 100vh;
    position: relative;
    width: 100%;
}

.hero-text h1 {
    color: #2d2e32;
    font-size: 3.5rem;
    line-height: 1.2;
    margin-bottom: 2rem;
    margin-top: 2rem;
}

.hero-text {
    display: flex;
    flex-direction: column;
    max-width: 27rem;
    position: relative;
}

.hero__wave {
    position: absolute;
    right: 6rem;
    top: 6.4rem;
    width: 4rem;
}

.hero-main {
    align-items: center;
    display: flex;
    gap: 7rem;
    justify-content: center;
    position: relative;
}

.hero-text p {
    color: #767676;
    font-family: Mulish, sans-serif;
    font-size: 16px;
    font-weight: 500;
    line-height: 1.6;
}

.hero-img {
    -webkit-animation: morph 8s ease-in-out infinite;
    animation: morph 8s ease-in-out infinite;
    background-image: url(/dawood.jpg);
    background-position: 50%;
    background-repeat: no-repeat;
    background-size: cover;
    border: 3px solid #2d2e32;
    border-radius: 60% 40% 30% 70%/60% 30% 70% 40%;
    height: 22rem;
    position: relative;
    transition: all 1s ease-in-out;
    width: 22rem;
}

@keyframes morph {
    0% {
        border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
    }

    50% {
        border-radius: 30% 60% 70% 40% / 50% 60% 30% 60%;
    }

    100% {
        border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
    }
}

.main__container {
    margin: 0 auto;
    max-width: 107rem;
    padding: 0 4rem;

}

@media (max-width: 500px) {
    .main-container{
        padding: 0 !important;
    }
}
@media (max-width: 900px) {
    .hero-main {
        flex-direction: column-reverse;
        gap: 0;
    }

    .content {
        height: auto;
        margin-top: 0;
    }

    .hero-text {
        text-align: center;
    }

    .hero__wave {
        right: 1rem;
        top: 5.4rem;
    }
    .any{
        gap: 0;
        justify-content: center;
        margin: 1.5rem;
    }

 
    .hero {
    height: auto;
    padding: 11rem 0;
}

.skills {
    flex-direction: column;
    position: static;
    bottom: -10rem !important;
    gap: 40px;
}

.content {
    flex-direction: column;
    gap: 3rem;
    height: auto;
    text-align: center;
}

.skills p {
    border-bottom: 2px solid rgba(45,46,50,.5);
    border-right: none !important;
    margin: 0 !important;
    padding: 0 !important;
  }

  .skills ul {
    justify-content: center;
    gap: 1rem !important;
}

.skills ul li {
    width: 3.4rem !important;
    height: 3.4rem !important;
}
}

.skills {
    align-items: center;
    bottom: 0;
    color: #767676;
    display: flex;
    font-size: 1.7rem;
    left: 0;
    position: absolute;
}

.skills p {
    border-right: 2px solid rgba(45, 46, 50, .5);
    color: #2d2e32;
    font-family: Mulish, sans-serif;
    font-weight: 600;
    margin-right: 3rem;
    padding-right: 2rem;
    font-size: 1.2rem;
}

.skills ul {
    display: flex;
    flex-wrap: wrap;
    gap: 1.5rem;
    list-style: none;
}

.skills ul li {
    align-items: center;
    background-color: #fff;
    border-radius: 50%;
    box-shadow: 0 0 10px rgba(0, 0, 0, .09);
    cursor: pointer;
    display: flex;
    height: 4rem;
    justify-content: center;
    width: 4rem;
}

.skills ul li img {
    height: auto;
    width: 2rem;
}
</style>