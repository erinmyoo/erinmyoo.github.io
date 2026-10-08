---
title: "Solar Car"
---

<p align="center">
  <img alt="Solar Car" src="/../portfolio-images/SolarCar.png">
</p>

## Wheel Assembly
Designing the front hub and rear rim on the 2025 Solar Car to fit new packaging constraints and interface with the new motor.
<!-- 
<div style="text-align: center;">
  <img alt="Machined Front Hub bolted to the rotor disc for mule car testing" src="/../portfolio-images/MachinedFrontHub.png" width="40%">
</div>
-->
<div class="slideshow">
  <button class="prev" onclick="changeSlide(-1)">&#10094;</button>

  <div class="slides">
    <img src="/../hub-ppt-images/Hub_DR_slide_1">
    <img src="/../hub-ppt-images/Hub_DR_slide_2">
    <img src="/../hub-ppt-images/Hub_DR_slide_3">
    <img src="/../hub-ppt-images/Hub_DR_slide_4">
    <img src="/../hub-ppt-images/Hub_DR_slide_5">
    <img src="/../hub-ppt-images/Hub_DR_slide_6">
    <img src="/../hub-ppt-images/Hub_DR_slide_7">
    <img src="/../hub-ppt-images/Hub_DR_slide_8">
    <img src="/../hub-ppt-images/Hub_DR_slide_9">
    <img src="/../hub-ppt-images/Hub_DR_slide_10">
    <img src="/../hub-ppt-images/Hub_DR_slide_11">
    <img src="/../hub-ppt-images/Hub_DR_slide_12">
  </div>

  <button class="next" onclick="changeSlide(1)">&#10095;</button>
</div>

<script>
let slideIndex = 0;
const slides = document.querySelectorAll(".slides img");

function showSlide(index) {
  if (index >= slides.length) slideIndex = 0;
  if (index < 0) slideIndex = slides.length - 1;

  slides.forEach(slide => slide.style.display = "none");
  slides[slideIndex].style.display = "block";
}

function changeSlide(direction) {
  slideIndex += direction;
  showSlide(slideIndex);
}

showSlide(slideIndex);
</script>

## Axle Optimization
The axle on the 2023 Solar Car (Astrum) was optimized to reduce mass and deflection while prioritizing minimizing bearing resistance. Analysis of the stress and deflection of the axle under 3 load cases was done through ANSYS, also exploring different axle geometries and materials. This analysis will inform the design of the 2025 Solar Car axle as cell as its impact on race time vs cost.

<div class="slideshow">
  <button class="prev" onclick="changeSlide(-1)">&#10094;</button>

  <div class="slides">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_1.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_2.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_3.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_4.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_5.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_6.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_7.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_8.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_9.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_10.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_11.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_12.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_13.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_14.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_15.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_16.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_17.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_18.png">
    <img src="/../axle-ppt-images/Axle_Opt_DR_slide_19.png">
  </div>

  <button class="next" onclick="changeSlide(1)">&#10095;</button>
</div>

<script>
let slideIndex = 0;
const slides = document.querySelectorAll(".slides img");

function showSlide(index) {
  if (index >= slides.length) slideIndex = 0;
  if (index < 0) slideIndex = slides.length - 1;

  slides.forEach(slide => slide.style.display = "none");
  slides[slideIndex].style.display = "block";
}

function changeSlide(direction) {
  slideIndex += direction;
  showSlide(slideIndex);
}

showSlide(slideIndex);
</script>

## Mule Car Chassis
The creation, design and manufacturing of the Mule Car Chassis on the Solar Car team was completed in a 2 week span for the Mechanical and Electrical Divisions to test their systems and components. I created the CAD design and ran beam-bending hand calcs as well as FEA to meet safety regulations and safety factor of 1.5. I also complied a BOM and coordinated the manufacturing process (welding and waterjet) for the chassis. I had complete ownership of this project as a new member of the team.
<p align="center">
  <img alt="Mule Car Chassis Steel Frame" src="/../portfolio-images/MuleCarChassisSteelFrame.png" width="45%">
&nbsp; &nbsp; &nbsp; &nbsp;
  <img alt="Assembled Mule Car" src="/../portfolio-images/AssembledMuleCar.png" width="45%">
</p>

## Tooling: Initial Upper and Lower Plug Design 
The tooling, initial plugs, for the upper and lower parts of the car was designed in Siemens NX. I communicated with the manufacturer to determine any important features to add to the tooling such as surface finish, split lines and mold lines. Additionally, I researched optimal tooling board density and plug to mold composite manufacturing process for a better surface finish.
<div style="text-align: center;">
  <img alt="Initial Lower Plug Isometric View" src="/../portfolio-images/InitialLowerPlugIsometricView.png" width="45%">
</div>


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

.prev {
  left: 0;
}

.next {
  right: 0;
}

.prev:hover,
.next:hover {
  background: rgba(31, 63, 111, 1);
}
</style>
