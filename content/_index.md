---
layout: alps-home
toc: true
---

<style>
.leftX {
  #flex: 1 1 1%;
  padding-right: 1em;
  #outline: 1px solid red;
}
.rightX {
  #flex: 1 1 1%;
  padding-left: 1em;
  #outline: 1px solid blue;
  float: left;
}

.flexBox {
  display: flex;
  #justify-content: space-around;
  flex-flow: row wrap;
}


@media (min-width: 800px) {
  .flexBox {
    grid-template-columns: 1fr 5fr;
  }
  .leftX {
    flex: 1 1 1%;
    padding-right: 1em;
    #outline: 1px solid red;
  }
 .rightX {
    flex: 1 1 1%;
    padding-left: 1em;
    #outline: 1px solid blue;
    float: left;
  }
}


.logoX {
  content:url("/figs/Alps-disciplines.webp");
}

:is(html[class~="dark"]) .logoX {
  content:url("/figs/Alps-disciplines-dark.webp");
}

</style>

<div class="flexBox" >
<div class="leftX">

## Welcome to the ALPS Software Package

The ALPS (Algorithms and Libraries for Physics Simulations) software package aims to provide a set of well tested, robust, and standardized components for numerical simulations of condensed matter systems, incluing bosonic, fermionic, and spin systems. They consist of a set of components that are used in state-of-the-art high performance codes.

<div class="cta-buttons" style="text-align:left;width:100%;">
{{< cta-button text="Get started" link="documentation/start/intro" icon="build"  prim="yes" >}}
{{< cta-button text="Tutorials" link="tutorials/" icon="launch" >}}
</div>
</div>
<div class="rightX" >
<img class="logoX" />
</div>

</div>






## Our Impacts
ALPS has been used by hundreds of researchers in 52 countries since its inception and has produced thousands of publications by different groups. In addition, ALPS has been applied to more than 20 research disciplines, as evidenced by the research citations. We are pround of its contribution in advancing the understanding of material properties.

## Our Systems
One-, two-, and three-dimensional lattice systems with model parameters that describe real materials. 

## Our Evolution
ALPS progress needs the support of the user community. If you identify any potential bugs in the codes, please submit a [bug report](https://github.com/ALPSim/ALPS/issues).

## Our Collaborations
We are happy to collaborate with researcher and educators around the world on projects or codes that can have an ALPS application or can be included in the ALPS framework. If you are interested, please reach out to one of our [steering committee members](govern#alps-community-steering-committee).

## Our Acknowledgement
ALPS software package results from the contributions of numerous researchers around the world in the past 20+ years. Without their efforts, the current state of the software is impossible to exist. We hope that more researchers will join us in promoting and developing this open source ecosystem to further advance ALPS's capabilities in research and education. 


