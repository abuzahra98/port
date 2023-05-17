<template>
    <div class="footer-container">
        <div class="footer">
            <div class="footer-text">Copyright © 2023. All rights are reserved</div>
            <div>
                <img class="footer_image" src="/GitHub.png" alt="">
                <img style="background-color: white;" class="footer_image" src="/linkedin.png" alt="">

            </div>
        </div>

    </div>

</template>
<style>
.footer_image{
    border-radius: 50%;
    width: 50px;
    margin-inline-end: 10px;
}

@media (max-width: 1000px) {
    .footer {
    width: auto !important;
  }

    
}
.footer-text {
    font-size: 20px;
    color: white;
    font-weight: 600;
}
.footer {
    align-items: center;
    display: flex;
    justify-content: space-between;
    width: 61rem;
    margin: auto;
}

.footer-container {
    background-color: #2d2e32;
    padding: 4rem 0;
    width: 100%;
}
</style>