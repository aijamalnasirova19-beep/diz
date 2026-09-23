// ==========================
// TOY KҮНҮ
// ==========================

const weddingDate = new Date(
    2026,
    11,
    2,
    17,
    0,
    0
);

// ==========================
// COUNTDOWN  артка санак
// ==========================

function updateCountdown() {

    const now = new Date().getTime();

    const distance =
        weddingDate.getTime() - now;

    if(distance < 0){

        document.getElementById("days").innerHTML="00";
        document.getElementById("hours").innerHTML="00";
        document.getElementById("minutes").innerHTML="00";
        document.getElementById("seconds").innerHTML="00";

        return;
    }

    const days = Math.floor(
        distance /
        (1000*60*60*24)
    );

    const hours = Math.floor(
        (distance %
        (1000*60*60*24))
        /
        (1000*60*60)
    );

    const minutes = Math.floor(
        (distance %
        (1000*60*60))
        /
        (1000*60)
    );

    const seconds = Math.floor(
        (distance %
        (1000*60))
        /
        1000
    );

    document.getElementById("days")
    .innerHTML =
    String(days).padStart(2,"0");

    document.getElementById("hours")
    .innerHTML =
    String(hours).padStart(2,"0");

    document.getElementById("minutes")
    .innerHTML =
    String(minutes).padStart(2,"0");

    document.getElementById("seconds")
    .innerHTML =
    String(seconds).padStart(2,"0");
}

updateCountdown();

setInterval(
    updateCountdown,
    1000
);

// ==========================
// MUSIC
// ==========================

const music =
document.getElementById("music");

const musicBtn =
document.getElementById("musicBtn");

musicBtn.addEventListener(
    "click",
    ()=>{

        if(music.paused){

            music.play();

            musicBtn.innerHTML =
            "⏸";

        }else{

            music.pause();

            musicBtn.innerHTML =
            "🎵";

        }

    }
);

// ==========================
// HERO FADE IN бащкы сурот 
// ==========================

window.addEventListener(
    "load",
    ()=>{

        const hero =
        document.querySelector(
            ".hero-content"
        );

        hero.style.opacity="0";
        hero.style.transform=
        "translateY(40px)";

        setTimeout(()=>{

            hero.style.transition=
            "1.5s";

            hero.style.opacity="1";

            hero.style.transform=
            "translateY(0)";

        },300);

    }
);

// ==========================
// SCROLL REVEAL жылдырганда корсотуу
// ==========================

const revealElements =
document.querySelectorAll(
    "section"
);

function revealOnScroll(){

    revealElements.forEach(
        (item)=>{

        const top =
        item.getBoundingClientRect()
        .top;

        if(
            top <
            window.innerHeight-120
        ){

            item.style.opacity="1";

            item.style.transform=
            "translateY(0)";
        }

    });

}

revealElements.forEach(
    (item)=>{

    item.style.opacity="0";

    item.style.transform=
    "translateY(60px)";

    item.style.transition=
    "1s";

});

window.addEventListener(
    "scroll",
    revealOnScroll
);

revealOnScroll();

// ==========================
// PARALLAX HERO
// ==========================

window.addEventListener(
    "scroll",
    ()=>{

    const scroll =
    window.pageYOffset;

    const hero =
    document.querySelector(
        ".hero"
    );

    hero.style.backgroundPositionY =
    scroll * 0.4 + "px";

});

// ==========================
// FLOWERS FLOAT гулдор калкып журот
// ==========================

const flowers =
document.querySelectorAll(
    ".flower"
);

setInterval(()=>{

    flowers.forEach(
        (flower)=>{

        flower.style.transform =
        `translateY(${
            Math.random()*10
        }px)`;

    });

},2500);
const photoss =
document.querySelectorAll(
".event-details"
);

photoss.forEach((img)=>{

    img.addEventListener(
        "mouseenter",
        ()=>{

        img.style.transform=
        "scale(1.08)";

    });

    img.addEventListener(
        "mouseleave",
        ()=>{

        img.style.transform=
        "scale(1)";

    });

});
// ==========================
// GALLERY EFFECT галерея
// ==========================

const photos =
document.querySelectorAll(
".gallery-grid img"
);

photos.forEach((img)=>{

    img.addEventListener(
        "mouseenter",
        ()=>{

        img.style.transform=
        "scale(1.08)";

    });

    img.addEventListener(
        "mouseleave",
        ()=>{

        img.style.transform=
        "scale(1)";

    });

});

// const photos =
// document.querySelectorAll(
// ".cards"
// );

// photos.forEach((h3)=>{

//     h3.addEventListener(
//         "mouseenter",
//         ()=>{

//         h3.style.transform=
//         "scale(1.08)";

//     });

//     h2.addEventListener(
//         "mouseleave",
//         ()=>{

//         h3.style.transform=
//         "scale(1)";

//     });

// });

// ==========================
// RSVP FORM
// ==========================

// const form =
// document.querySelector("form");

// if(form){

// form.addEventListener(
//     "submit",
//     function(e){

//         e.preventDefault();

//         alert(
//             "Рахмат! Сиздин маалыматыңыз кабыл алынды ❤️"
//         );

//         form.reset();

//     }
// );

// }

// ==========================
// SMOOTH BUTTON баскыч
// ==========================

const heroBtn =
document.querySelector(
    ".hero-btn"
);

if(heroBtn){

heroBtn.addEventListener(
    "click",
    function(e){

        e.preventDefault();

        document
        .querySelector(
            "#invitation"
        )
        .scrollIntoView({

            behavior:"smooth"

        });

    }
);

}