<template>
    <div class="main__container">
        <div class="hero-main">
            <div class="hero-text">
                <h1>Front-End Developer</h1>
                <img src="/waving.png" alt="waving_hand" />
                <p>
                    Hi, I'm Stefan Topalovic. A passionate Front-end React Developer based
                    in Belgrade, Serbia. 📍
                </p>
                <span>
                    <a aria-label="linkedin" rel="noreferrer" target="_blank"
                        href="https://www.linkedin.com/in/stefan-topalovic-dev/">
                        <i class="fa-brands fa-linkedin"></i>
                    </a>
                    <a aria-label="github" rel="noreferrer" target="_blank" href="https://github.com/stefvndev">
                        <i class="fa-brands fa-github"></i>
                    </a>
                </span>
            </div>
            <div class="hero-img">
 
            </div>
        </div>
    </div>
</template>

<style lang="scss">
.hero-text h1 {
    color: #2d2e32;
    font-size: 4rem;
    line-height: 1.2;
    margin-bottom: 2rem;
    margin-top: 2rem;
}
.hero-text {
    display: flex;
    flex-direction: column;
    max-width: 35rem;
    position: relative;
 }

 .hero-text img {
    position: absolute;
    right: 12rem;
    top: 7.4rem;
    width: 4rem;
}
.hero-main {
    max-width: 107rem;
    padding: 0 4rem;
    display: flex;
    justify-content: center;
    align-items: center;
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
    
    height: 25rem;
    margin-top: 14rem;
    display: flex;
    align-items: center;
    justify-content: center;

  }
</style>