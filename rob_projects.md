---
title: "Robotics Projects and Experiences"
---

## National Science Foundation - REU: Collaborative Human-Robot Interaction for Robots in the Field
I assisted with optimizing the second iteration of an amphibious UAV for water resistance and endurance for long term autonomous missions. Main task was to test the thrust of all the motors on the UAV for endurance and salt water resistance. This required the design and manufacturing of a dual use motor thrust stand with automated python test scripts to gather data through a DAQ framework.
<div style="text-align: center;">
  <img alt="Motor Thrust Stand" src="/../portfolio-images/MotorThrustStand.png" width="45%">
</div>

<div class="slideshow" id="reu-slideshow">
  <button class="prev" onclick="changeSlide('reu-slideshow', -1)">&#10094;</button>

  <div class="slides">
    <img src="/../reu-ppt-images/REU_slide_1.png">
    <img src="/../reu-ppt-images/REU_slide_2.png">
    <img src="/../reu-ppt-images/REU_slide_3.png">
    <img src="/../reu-ppt-images/REU_slide_4.png">
    <img src="/../reu-ppt-images/REU_slide_5.png">
    <img src="/../reu-ppt-images/REU_slide_6.png">
    <img src="/../reu-ppt-images/REU_slide_7.png">
  </div>

  <button class="next" onclick="changeSlide('reu-slideshow', 1)">&#10095;</button>
</div>

For more information, visit [Motor Testing Documentation](https://github.com/erinmyoo/Motor-Thrust-Test).

## Wolverbot Kickers
To compete in the Robocup Small-Sized Humanoid League, robotic arms with 3 DOF are being designed and rapid prototyped through 3D printed. The first prototype can be seen in the image below. The black wooden dowel is only used for testing purposes to adjust the length of the arm. 
<div style="text-align: center;">
  <img alt="3D printed Arm Design for testing functionality" src="/../portfolio-images/ArmPrototype.png" width="15%">
</div>


<script>
const slideIndexes = {};

function showSlide(slideshowId, index) {
  const slideshow = document.getElementById(slideshowId);
  if (!slideshow) return;

  const slides = slideshow.querySelectorAll(".slides img");
  if (slides.length === 0) return;

  index = (index + slides.length) % slides.length;
  slideIndexes[slideshowId] = index;

  slides.forEach((slide, i) => {
    slide.style.display = i === index ? "block" : "none";
  });
}

function changeSlide(slideshowId, direction) {
  showSlide(
    slideshowId,
    (slideIndexes[slideshowId] || 0) + direction
  );
}

document.addEventListener("DOMContentLoaded", function () {
  document.querySelectorAll(".slideshow").forEach(slideshow => {
    showSlide(slideshow.id, 0);
  });
});
</script>


<style>
.slideshow {
  position: relative;
  width: 80%;
  max-width: 800px;
  margin: 2em auto;
  display: flex;
  align-items: center;
  justify-content: center;
}

.slides {
  width: 100%;
  text-align: center;
}

.slides img {
  display: none;
  width: 100%;
  max-height: 500px;
  object-fit: contain;
  margin: 0 auto;
}

.prev,
.next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background: rgba(31, 63, 111, 0.8);
  color: white;
  border: none;
  padding: 12px 16px;
  cursor: pointer;
  font-size: 20px;
  z-index: 2;
}

.prev { left: 0; }
.next { right: 0; }

.prev:hover,
.next:hover {
  background: rgba(31, 63, 111, 1);
}
</style>
