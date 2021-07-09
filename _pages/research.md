---
title: "Research"
layout: gridlay
sitemap: false
permalink: /research/
---


## Research


<style>
img{
  border-radius: 10px;
}
.col-md-3 {
  margin-top:10px;
  margin-bottom:10px;
  padding:0px;
  display:block;
  overflow:hidden;
  text-align:center;
  display: table-cell;
  background: white;
  border-radius: 20px;
  height: auto;
  <!-- border: 1px solid black; -->
}
iframe {
  margin:0;
  padding:0;
  width: 175px;
  display: inline;
  vertical-align: middle;
}
</style>

<div class="jumbotron">
<div class="row align-items-end">
<div class="col-md-12 col-sm-12">
### Cavitation as a gateway to better therapies
<img align="right" src="{{site.url}}{{site.baseurl}}/images/respic/lithotripsy.jpg" width="390px"/>
Cavitating bubbles can ablate cancer cells, fragment tissues, and deliver drugs, among other functions.
I create high-fidelity computational methods to simulate these dynamics.

Examples are:
* Euler--Euler and Euler--Lagrange <a href="{{ site.url }}{{ site.baseurl }}/papers/bryngelson-IJMF-19.pdf" target="_blank">sub-grid bubble cloud models</a>
* Accelerated models using a <a href="{{ site.url }}{{ site.baseurl }}/papers/bryngelson-IJMF-20.pdf" target="_blank">statistical paradigm and neural networks</a>
* Implementation in my open-source solver <a href="{{ site.url }}{{ site.baseurl }}/papers/bryngelson-CPC-19.pdf" target="_blank">MFC</a>

These enable realistic simulation of the bubble populations that nucleate during treatment.
This has impacted application-specific treatments, including:



* Improved _burst-wave lithotripsy administration_ in human trials 
* Understanding of <a href="{{ site.url }}{{ site.baseurl }}/papers/bryngelson-JCP-20.pdf" target="_blank">bubble-collapse-rebound</a> dynamics
* Cavitation-induced <a href="{{ site.url }}{{ site.baseurl }}/papers/bryngelson-JFM-19.pdf" target="_blank">erosion potential</a> for rough materialsrough materialsrough materialsrough materialsrough materialsrough materials


</div>
</div>
</div>


<div class="jumbotron">
<div class="row align-items-end">
<div class="col-md-9 col-sm-12">
### Learning from animals: Humpback whales
Specifically, they
* Release air from their blowholes while swimming, spiraling downwards
* Surround their prey with a wall of bubbles
* Vocalize from the exterior, trapping small fish in loud sound (~190dB!)
* Swim up and through the interior, lunge feeding on the fish

While fascinating, the acoustic mechanisms enabling this behavior are not understood.
My ensemble-averaged bubbly flow model simulates the relevant acoustic phenomena, <a href="{{ site.url }}{{ site.baseurl }}/papers/bryngelson-JASA-20.pdf" target="_blank">advancing our interpretation of this behavior</a>.
Similar outcomes are desirable for sensitive, implanted biomedical devices.
</div>
<div class="col-md-3 col-sm-12" >
  <img src="{{ site.url }}{{ site.baseurl }}/images/respic/lithotripsy.jpg" width="175px"/>
</div>
</div>
</div>
 
