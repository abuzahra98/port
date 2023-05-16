<template>
    <div id="projects" class="project">
        <div class="projects-grid">
            <div class="sub-header">PORTFOLIO</div>
            <div class="project-content-header">
                Each project is a unique piece of development 🧩
            </div>
            <div class="project-container">
                <div class="pro__img">
                    <a href="">
                        <img style="" class="project__image" src="/car-rental-full.webp" alt="">
                    </a>
                </div>
                <div class="pro__text">
                    <div class="pro-text__1">
                        CAR RENTAL 🚗

                    </div>
                    <div class="pro-text__2">
                        A car rental website is an online platform that allows users to rent cars for personal or business
                        use. The website provides an interface for searching, comparing, and reserving cars.
                    </div>
                    <div class="stack">
                        <p>React</p>
                        <p>SCSS</p>
                    </div>
                    <div class="link">
                        <a class="any-project" target="_blank"   rel="noreferrer">Code <i
                                class="fa-brands fa-github"></i></a>
                        <a class="any-project" target="_blank" href="https://car-rental-dawood.vercel.app/" rel="noreferrer">Live
                            Demo<i class="fa-solid fa-arrow-up-right-from-square link-icon"></i></a>

                    </div>

                </div>

            </div>
        </div>

    </div>
</template>

<style>
.sub-header {
    color: #147efb;
    font-size: 17px;
    font-weight: 700;
    margin-bottom: 1rem;
    text-transform: uppercase;
}
.project-content-header {
    color: #2d2e32;
    font-size: 25px;
    margin-bottom: 6rem;
    font-weight: 800;
}
.link {
    align-items: center;
    display: flex;
    justify-content: space-evenly;
}

.any-project {
    color: #2d2e32;
    font-size: 17px;
    font-weight: 500;
    padding: 10px;
     text-decoration: none;
}

.stack {
    display: flex;
    gap: 1rem;
    justify-content: center;
    margin-block: 1rem;
}

.stack p {
    background-color: #fff;
    box-shadow: 0 0 10px rgba(0, 0, 0, .1);
    color: #000 !important;
    font-family: Mulish, sans-serif !important;
    font-weight: 700 !important;
    padding: 10px 15px;
}

.pro-text__1 {
    color: #2d2e32;
    font-size: 1rem;
    margin-bottom: 1rem;
    position: relative;
    text-transform: uppercase;
    font-weight: 800;

}

.pro-text__2 {

    color: #767676;
    font-size: 17px;
    font-weight: 500;
    text-align: center;
    text-transform: none;

}

.pro__text {
    display: flex;
    flex-direction: column;
    height: auto;
    justify-content: center;
    text-align: center;
    width: 30rem;
}

.project__image:hover {
    transform: translateY(-81%);
    transition: transform 10s ease-in-out;
}

.project__image {
    transform: translateY(0%);
    transition: transform 8s ease-in-out 0s;
    width: 100%;
}

.pro__img {
    background-color: hsla(0, 0%, 46%, .2);
    border-radius: 1.7rem;
    box-shadow: 0 0 10px rgba(0, 0, 0, .1);
    height: auto;
    overflow: hidden;
    width: 50rem;
}

.project {
    background-color: #f9f9f9;
    padding: 11rem 0;
}

.projects-grid {
    margin: 0 auto;
    max-width: 68rem;
    padding: 0 4rem;
}

.project-container {
    padding: 1.5rem;
    background-color: #fff;
    border-radius: 1.7rem;
    box-shadow: 0 0 10px rgba(0, 0, 0, .1);
    height: 25rem;
    display: flex;
    gap: 5rem;

}
@media (max-width: 850px) {
    .project-container {
    flex-direction: column;
    gap: 3rem;

}

.pro__text {
    display: flex;
    flex-direction: column;
    height: auto;
    justify-content: center;
    text-align: center;
    width: 100%;
}

.pro__img {
    width: 100%;
}

.project-container{
    height: 45rem;
}
.projects-grid {
    padding: 10px;
}
}
</style>