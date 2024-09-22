+++

template = "page.html"
title = "Personal"
[extra]
+++


<h3 class="title is-3" id="scicom">
    <a class="has-text-{{ colors::style() }}" href="#/scicom">
        Outreach
    </a>
</h3>

Throughout my development as a scientist, I have always been passionate about sharing my excitement for science with others. This passion has fueled my enthusiasm for scientific outreach, a journey that began in high school and has continued ever since. Over the years, I have honed my ability to communicate complex scientific concepts in ways that are accessible and engaging for the general public.

I have also explored novel methods of public engagement. During my undergraduate studies, I developed a live, computer-based outreach event in which my fellow students and I invited the public to ask any astronomy or space-related questions. We would discuss these topics using visual aids like Universe Sandbox, Stellarium, and Space Engine, creating an interactive and immersive experience.

My recent outreach endeavor has been exploring the use of social virtual reality (VR) tools for online science communication. In 2020, shortly after the pandemic began, I began utilizing social VR to reach a broader audience and engage in various outreach activities. Initially, these events were small, focusing mainly on answering questions. However, I soon expanded my approach by using 3D modeling tools to import life-sized models of space telescopes, Mars probes, and even a full recreation of the Apache Point Observatory 3.5-meter telescope into the virtual space.

In addition to these efforts, I have been actively building a STEM community within social VR to support other scientists and STEM professionals interested in utilizing VR platforms for public engagement. Our work has been recognized by social scientist Dr. Ruth Diaz, who featured it <a href="https://youtu.be/VaAk5bjegso" target="_blank">in this video</a>, which also includes a preview of the Apache Point Observatory 3.5-meter model.


<h3 class="title is-3" id="scicom">
    <a class="has-text-{{ colors::style() }}" href="#/hobby">
        Hobbies
    </a>
</h3>


Outside of work, I engage in a wide range of hobbies that keep me mentally stimulated. Some are related to my VR outreach endeavors, like learning 3D modeling and game engine scripting. Others stem from sheer curiosity, such as obtaining my amateur radio license and gradually learning new languages (Spanish and German). Since childhood, I’ve also had an interest in hands-on activities like woodworking, electronics, and other "garage" hobbies.

My personal favorite achievement has been my progress toward obtaining a private pilot’s license. Flying has always been a dream of mine, and I’m thrilled to be making it a reality. There’s nothing quite like the freedom and perspective that comes with being up in the air.

<div class="slideshow-container">
    <div class="mySlides fade">
    <img src="\img\NMFlying.jpg" style="height:600px; object-fit:contain; display: block ;margin: 0 auto;">
    <div class="text" style="background-color: rgba(0, 0, 0, 0.5); color: white; padding: 10px;">Magdalena Peak near Las Cruces, NM</div>
    </div>
    <div class="mySlides fade">
    <img src="\img\meFlying.jpg" style="height:600px; object-fit:contain; display: block ;margin: 0 auto;">
    <div class="text" style="background-color: rgba(0, 0, 0, 0.5); color: white; padding: 10px;">Solo Flight</div>
    </div>
    <div class="mySlides fade">
    <img src="\img\Training.jpg" style="height:600px; object-fit:contain; display: block ;margin: 0 auto;">
    <div class="text" style="background-color: rgba(0, 0, 0, 0.5); color: white; padding: 10px;">Photo of me by my flight instructor</div>
    </div>
    <div class="mySlides fade">
    <img src="\img\CampfireGuitar.jpg" style="height:600px; object-fit:contain; display: block ;margin: 0 auto;">
    <div class="text" style="background-color: rgba(0, 0, 0, 0.5); color: white; padding: 10px;">Camping and Music. A great combo</div>
    </div>
    <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
    <a class="next" onclick="plusSlides(1)">&#10095;</a>
</div>
<br>
<div style="text-align:center">
    <span class="dot" onclick="currentSlide(0)"></span>
    <span class="dot" onclick="currentSlide(1)"></span>
    <span class="dot" onclick="currentSlide(2)"></span>
    <span class="dot" onclick="currentSlide(3)"></span>
</div>

<!-- Slideshow CSS -->
<style>
.slideshow-container {
    position: relative;
    max-width: 100%;
    margin: auto;
}

.mySlides {
    display: none;
}

.fade {
    animation-name: fade;
    animation-duration: 1.5s;
}

@keyframes fade {
    from {opacity: .4} 
    to {opacity: 1}
}

.text {
    color: #f2f2f2;
    font-size: 15px;
    padding: 8px 12px;
    position: absolute;
    bottom: 8px;
    width: 100%;
    text-align: center;
}

.prev, .next {
    cursor: pointer;
    position: absolute;
    top: 50%;
    width: auto;
    margin-top: -22px;
    padding: 16px;
    color: white;
    font-weight: bold;
    font-size: 18px;
    transition: 0.6s ease;
    border-radius: 0 3px 3px 0;
}

.next {
    right: 0;
    border-radius: 3px 0 0 3px;
}

.prev:hover, .next:hover {
    background-color: rgba(0,0,0,0.8);
}

.dot {
    cursor: pointer;
    height: 15px;
    width: 15px;
    margin: 0 2px;
    background-color: #bbb;
    border-radius: 50%;
    display: inline-block;
    transition: background-color 0.6s ease;
}

.active, .dot:hover {
    background-color: #717171;
}
</style>

<!-- Slideshow JavaScript -->
<script>
let slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
    showSlides(slideIndex += n);
}

function currentSlide(n) {
    showSlides(slideIndex = n);
}

function showSlides(n) {
    let i;
    let slides = document.getElementsByClassName("mySlides");
    let dots = document.getElementsByClassName("dot");
    if (n > slides.length) {slideIndex = 1}    
    if (n < 1) {slideIndex = slides.length}
    for (i = 0; i < slides.length; i++) {
        slides[i].style.display = "none";  
    }
    for (i = 0; i < dots.length; i++) {
        dots[i].className = dots[i].className.replace(" active", "");
    }
    slides[slideIndex-1].style.display = "block";  
    dots[slideIndex-1].className += " active";
}
</script>