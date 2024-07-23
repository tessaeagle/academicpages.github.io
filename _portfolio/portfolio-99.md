---
title: "Wave Function Collapse Generated Constellations"
excerpt: "Using the Wave Function Collapse algorithm, we explore the generation of computational constellation art using 77 individual tiles designed in Photoshop.<br><br><img src='/images/wfc.png'>"
collection: portfolio
---

## Background
Wave Function Collapse is an algorithm that takes an input (bitmap or individual tiles) and generates a similar output (see [here](https://github.com/mxgmn/WaveFunctionCollapse)). As part of a class project in CMPM202, my two teammates and I considered themes we wanted to explore through generative art. We considered trying a Where's Waldo style tileset, but ultimately decided to attempt to generate unique sets of star constellations. 

**Project Goal:** Use WFC and our own tiles to generate unique sets of star constellations. <br>
**Project Year:** Winter 2020

## Project Implementation

We initially attempted to use [Isaac Karth's Python port](https://github.com/ikarth/wfc_2019f) of WFC, but ultimately used the initial C# simple tiles implementation. This implementation takes in a set of tiles and adjency rules indicatting how and where tiles can be placed. Utilizing the Wave Function Collapse algorithm with our own tileset to generate computational art. We created a set of 77 tiles in Photoshop (see below) to attempt to generate randomized constellations using WFC. Each tile contained a combination of joints (circles) to represent stars, and arms (lines) to represent the drawing of constellations. Joints could connect to arms or blank tiles, while arms could connect to joints or other arms but not blank tiles as each constellation end had to be a star.

<img src='/images/wfc2.png'>

Our initial attempts led to straight constellations made up of 90 degree angles (see below figure). We adjusted our tileset to include diagonal lines and joints which allowed us to have constellations made up of combinations of 45 and 90 degree angles. 

<img src='/images/wfc5.png'><br>

Below are the finalized images we were able to generate using WFC. 

<img src='/images/wfc.png'><br>

<img src='/images/wfc3.png'><br>

<img src='/images/wfc4.png'><br>
