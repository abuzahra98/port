<template>
    <div id="contact" class="contactus">
        <div class="contactus-container">
            <div class="sub-header">CONTACT</div>
            <div class="project-content-header">
                Don't be shy! Hit me up! 👇
            </div>
            <div class="contactus__text-container">
                <div class="flex">
                    <div class="circle">

                        <img src="/location.svg" alt="">
                    </div>
                    <div class="contactus__content-text">
                        <div class="contact-us__text">Location</div>
                        <div class="location__text">Amman,Jordan</div>

                    </div>

                </div>
                <div class="flex">
                    <div class="circle">
                        <img src="/mail.svg" alt="">

                    </div>
                    <div class="contactus__content-text">
                        <div class="contact-us__text">Mail</div>
                        <div class="location__text">dawoodbasher@gmail.com</div>
                    </div>

                </div>
            </div>
        </div>

    </div>
</template>

<style>
@media  (max-width:850px) {
    .contactus {
        padding:9rem 10px !important;
    }
}

@media  (max-width:640px) {
    .contactus-container {
        width: auto !important;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;

    }
    .contactus__text-container {
        flex-direction: column;
        gap: 4rem !important;

    }
    .flex {
        flex-direction: column;
        align-items: center;
        justify-content: center;

    }
    .circle {
        margin-inline-end:0px !important;
        margin-block-end: 15px;
    }

    .contactus__content-text {
        text-align: center;
    }
    .project-content-header {
 
    font-size: 23px !important;
 
}
}
.circle {
    background-color: #2a95ff30;
    margin-inline-end: 15px;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 75px;
    height: 75px;
    border-radius: 50%;
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}

.flex {
    align-items: center;
    justify-content: center;
    display: flex;
}

.contactus {
    padding: 9rem;
}

.contactus-container {
    max-width: 60rem;
    margin: auto;

}

.contactus__text-container {
    display: flex;
    gap: 8rem;
}

.contact-us__text {
    font-size: 17px;
    color: black;
    font-weight: 800;
}

.location__text:hover{
    color: #147efb;
    transition: all .3s;
    cursor: pointer;
}
</style>