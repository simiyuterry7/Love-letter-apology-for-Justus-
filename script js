const container = document.getElementById("background-animation");

function createHeart() {

    const heart = document.createElement("div");

    heart.innerHTML = "💙✨";

    heart.style.position = "absolute";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.top = "110vh";
    heart.style.fontSize = (18 + Math.random() * 20) + "px";
    heart.style.opacity = Math.random() * 0.5 + 0.5;
    heart.style.pointerEvents = "none";

    const duration = 6000 + Math.random() * 5000;

    heart.animate([
        {
            transform: "translateY(0px) translateX(0px) rotate(0deg)"
        },
        {
            transform: `translateY(-120vh) translateX(${Math.random() * 120 - 60}px) rotate(${Math.random() * 360}deg)`
        }
    ], {
        duration: duration,
        easing: "linear"
    });

    container.appendChild(heart);

    setTimeout(() => {
        heart.remove();
    }, duration);

}

setInterval(createHeart, 350);

// Create a few hearts immediately
for (let i = 0; i < 12; i++) {
    setTimeout(createHeart, i * 250);
}
