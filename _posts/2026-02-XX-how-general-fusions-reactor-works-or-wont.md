---
layout: post
title: "How TAE's fusion reactor will work (or won't)"
published: false
---
<p><img src="{{ site.baseurl }}/content/images/2025/12/DPK-TAE-Technologies-Norm-Rendering-Exterior-Full-View-Cropped.jpg" alt="How TAE's fusion reactor will work (or won't)"></p>

*Closely following TAE's merger with the public company TMTG, General Fusion has announced that they are going public through a SPAC. As with my [TAE article](https://www.fusionconclusion.com/how-taes-fusion-reactor-will-work-or-wont/), I aim to answer for non-experts: "What, exactly, is General Fusion building and how close is it to working?"*

This piece is the second is a series where I'll explain the fusion reactor concepts being pursed by fusion companies and then evaluate the company claims using the standard metrics of fusion physicists: plasma temperature, density, and confinement (pluse the realities of power balance and economics).

For this article, I'll start with the story of how General Fusion came to be, tieing it to the work done on similar concepts at the U.S. Naval Research Laboratory (NRL) and Los Alamos National Laboratory (LANL). Then I'll lay out General Fusion's argument for its steam piston driven shockwave into a spinning lead-lithium vortex to compress a plasma target to fusion conditions. Finally, I'll show their progress against what they need to achieve fusion energy and show why many are skeptical that they can achieve it. My goal is to give a clear and sober picture of where General Fusion is and what they need to do to get to where they say they are going.

## Background

Before diving into General Fusion's reactor concept and critiques, it is important to set the stage of how this concept evolved. See my previous article on [TAE](https://www.fusionconclusion.com/how-taes-fusion-reactor-will-work-or-wont/) for a brief history of "mainline" and "alternative" fusion concepts, of which General Fusion is considered an alternative.

### Compressing plasmas in the U.S.S.R., NRL, and LANL

In the 1960's researchers at the Kurchatov Institute in the U.S.S.R. were using rapidly compressing solid metal liners to compress plasmas to near the conditions needed to generate fusion energy, in a process called [magnetized target fusion (MTF)](https://en.wikipedia.org/wiki/Magnetized_target_fusion). This works as follows: A a mangetically confined plasma is formed inside of an electrical conductor. The conductor is compressed rapidly around the plasma. A conductor with high enough electrical conductivity does not allow the magnetic field to penetrate through it on the short timescales of compression. As the plasma is compressed (with $C=R_0/R$ as the ratio between the initial plasma radius $R_0$ and the compressed plasma radius $R$) the magnetic field increases $B \propto C^2$ to conserve magnetic flux. The compression also increases the plasma density $n \propto C^3$ if the particles are well confined and increases the plasma temperature $T \propto C^2$ if the system is [adiabatic](https://en.wikipedia.org/wiki/Adiabatic_process) and does not leak energy.

To get to fusion energy production conditions requires that the magnetic field confines the plasma all the way through the compression. [Beta](https://en.wikipedia.org/wiki/Plasma_beta) ($\beta$) is the ratio of the plasma pressue to the magnetic pressure. Every mangetic fusion plasma has a maximum beta it can support. In adiabatic compression beta increases as $\beta \propto C$, so there is a finite limit to which the plasma can be stabily compressed.

While the soviet scientists achieved some success in compressing plasmas, it was realized that the cost of the metal liners would exceed the value of the fusion energy generated. This is a problem common to many of the pulsed fusion concepts where the cost to produce the target and anything else destroyed in the pulse must be less than that of the value of the energy produced. It is termed the "kopeck problem" after Russian [kopeck](https://en.wikipedia.org/wiki/Kopeck), which was worth 0.01 rubles or $0.00013 USD as of mid-February 2026 (it was essentially the value of a U.S. penny in the 1960's).

The kopeck problem pushed researchers to use liquid liners for compression as they could be recycled in situ with minimal efforts to reform it between pulses. The NRL and LANL picked up on this concept and did a series of experiments in the 1970's along with detailed reactor conceptual designs through their [Linus program](https://en.wikipedia.org/wiki/Linus_(fusion_experiment)). MTF fusion suffered a similar fate to other alternative fusion concepts and, at least according to its propoents, has been underfunded for decades.

## Framing the discussion

To fusion outsiders – and some insiders – it's hard to differentiate among the different concepts and separate out fact from opinion in the narratives that are told around them. For any given concept: there are proponents who will argue to the grave that theirs is the only way to a fusion power plant, there are opponents who will argue with absolute conviction that it has no chance of working, and there are many people occupying the middle.

In discussing contentious issues like the tradeoffs of different fusion reactor concepts, I lean on [Rapoport’s Rules](https://bigthink.com/the-learning-curve/rapoports-rules-arguments/) for a productive framing:

1. Explain the other person’s position clearly, vividly, and justly.
2. Mention anything you’ve learned.
3. List the points on which you agree.
4. Only now make a critique or refutation.

Due to the efforts of many brilliant fusion physicists, we understand much of the physics to point to where the challenges of different concepts can be laid out quantitatively. We know the targets in temperature, density, and confinement time that a fusion reactor must achieve to have even a hope of being a power plant, and we can measure what they are in experiments. We can calculate and estimate how power flows and where it is lost. Thus, we can have productive discussions on how concepts fare as potential fusion power plants.

With that as the backdrop, I'll now frame the fusion industry's discussions on how General Fusion's fusion reactor will work (or won't) using Rapoport's Rules.

## General Fusion's public position

Fortunately for this discussion, General Fusion has [published peer-reviewed articles](https://generalfusion.com/post/category/research-library/) on their experiments and their results as well as put out public information on their vision for how that translates to a fusion power plant. While some of the specifics have changed over the years, especially the target plasma, the basic concept has reamined constant: Inject a stable plasma into the vortex created in the center of a spinning volume of liquid lead-lithium and use precicely-timed, steam-driven pistons to send a pulse through the liquid that compresesses the plasma to fusion energy production conditions. This is the most [steampunk](https://en.wikipedia.org/wiki/Steampunk) fusion concept out there. I am disapointed they missed the marketing opportunity to go hard into the steampunk esthetic and instead have a very sterile white lab and uniform red labcoats for their team.

General Fusion has the following claimed concept advantages:

!!show their classice optimium plot!!

### MTF is the optimal between the titans of ITER (magnetic fusion) and NIF (inertial fusion). 

The most common refrain from the MTF proponents is that it operates at intermediate plasma energy and driver power scales, which allows it to have a simpler and less expensive overall plant. The argument is a natural result of the [Lawson criterion](https://en.wikipedia.org/wiki/Lawson_criterion), which dictates there is a minimum product (~10^20 s/m^3) of the plasma density and [energy confinement time](https://wiki.fusion.ciemat.es/wiki/Energy_confinement_time) (i.e., how well the system insulates the fusion plasma) and that the two of them can be traded off each other. The story goes as follows:

Magnetic fusion operates at the low density end of the spectrum (~10^20/m^3) and long (~1 s) energy confinement time. The long energy confinement requires that the reactor operates effectively in steady state and have very high stored energy. This translates into needing large (>GJ-scale stored energy in the magnets), expensive superconducting magnets to maintain plasma confinement. As the plasma density is increased, the size of the required system decreases and therefor, at least those costs associated with the size and stored energy decreases. This is a similar argument used for the high-field path for magnetic fusion energy, which allows for shorter energy confinement times and therefor smaller machines; albeit at less of an extreme change in density as needed for MTF.

Inertial fusion operates at very high density (~10^31/m^3) with very short confinement times (~10^-10 s, given by the "stagnation time" of the compression). While reacting these requires no external confinement means, it requires putting the energy in very short pulses, which then requires very high pulsed power systems (>TW-scale) that are very expensive. 

MTF proponents predict that the space inbetween pure magnetic and pure interial to be a promise land of optimal density that requires modest energy and power scales, where a moderate initial magnetic field helps to contain the plasma and reduce losses, allowing gentler compression forces to densify and heat up the plasma to fusion conditions.

### The liquid lead-lithium metal wall and blanket is the solution to fusion nuclear damage.

One of the largest technical hurdles to economic fusion energy development is damage of components by the fusion [neutron bombardment](https://en.wikipedia.org/wiki/Neutron_radiation). The neutrons in fusion, especially the high-energy neutrons of deuterium-tritium fusion, must deposite their energy in whatever comprises the blanket surrounding the fusion plasma. This allows the fusion energy that they contain to be captured and turned into a useful form, typically in a thermal-to-electricity cycle.

The downside is that the neutrons damage solid materials along the way, through changing the material structure and transmutation. This typically reduces the engineering properties of the materials (e.g., structural strength, thermal conductivity, electrical resistivity, etc.) over time. Eventually the material no longer has sufficiently good properties to perform as designed and must be replaced.

The survivability of materials in a fusion neutron environment is one of the key factors that will determine how well fusion will economically compete with other energy sources. This comes through both in the costs of replacing components as well as the loss of revenue during maintenance periods.

A solution for dealing with the fusion neutron material damage problem is to minimize the amount of solid material in the damage pathway of neutrons, instead using liquids wherever possible. While this is not an idea pioneed by General Fusion, they are one of the primary fusion companies persuing it. Similarly, companies like Commonwealth Fusion Systems, are  planning on using a molten salt blanket; yet they still have a solid plasma-facing surface which will be subject to intense nuclear damage. Where General Fusion stands out is having basically no solid structure subject to the intense inner neutron flux. Although this has changed in recent years, as the company has moved to find a more stable plasma target and the present plans do have some functional solid material in the core of the plasma to maintain plasma stability.

### Fuel sustainability via tritium breeding.

While the [deuterium-tritium](https://en.wikipedia.org/wiki/Deuterium%E2%80%93tritium_fusion) fusion fuel has the easiest requirements on plasma conditions, [tritium](https://en.wikipedia.org/wiki/Tritium) has no significant natural source and must be made. Present supplies are mostly from fission power plants, specifically [CANDU reactors](https://en.wikipedia.org/wiki/CANDU_reactor). A fusion industry based on dueterium-tritium will need [tritium production](https://en.wikipedia.org/wiki/Breeding_blanket#Tritium_breeding) at a much larger scale, likely bred on site from the fusion-produced neutrons and lithium in the blanket.

A major challenge in breeding tritium is making enough to both sustain the use at the reactor it is being produced at as well as producing an excess to supply new fusion reactors. The excess must also account for tritium that gets "stuck" in the system, i.e., effectively trapped as it dissolves into metal and other parts of the system, as well as make up for the 5%/year that decays into [helium-3](https://en.wikipedia.org/wiki/Helium-3) (a valuable byproduct). The figure of merit for this is the tritium breeding ratio (TBR), which is the ratio of the amount of tritium bred to that burned in the reactor. TBR~1.05 is often given as the bare minimum to sustain a single plant. Ratios >1 require a neutron multiplier, with beryllium and lead being the most common.

In toroidal systems like tokamaks and stellarators, the volume available for a blanket and tritium breeding is limited and a complex trade-off of space with other systems. The resulting design often ends up having TBRs that are considered marginal: ~1.10-1.15. Some of these designs require the lithium in the blanket to be [isotopically enriched](https://doi.org/10.1016/j.joule.2025.101997) to have more lithium-6, which requires new industrial processes to produce.  Other solid structures that don't contain lithium (e.g., the vacuum vessel and plasma facing components) which need to be between the plasma and the blanket are a major culprate for the low TBR.

General Fusion's concept, having a liquid lithium-lead blanket completely surrounding the fusion plasma is esstentially the ideal design from a tritium breeding efficiency standpoint: The TBR is almost entirely determined by the blanket material and thickness. If General Fusion could get their system to work, it would have a TBR~1.5, which is more than enough to sustain its own operation and supply a growing fusion economy. Improving TBR from 1.50 to 1.15 results in a ~3.5x potential faster ramp up rate for the fusion industry, if tritium supply were the rate limiting factor.

### Steam: the simpler driver

In addition to using drivers and confinement at lower powers and energies, General Fusion claims to have a much simpler driver technology: steam-driven pistons, combining industrial revolution era technology with modern controls and material science. This is in contrast to inertial fusion using the world's most complex and powerful laser systems and magnetic fusion has a variety of bespoke, expensive heat techniques ([ICRH](https://en.wikipedia.org/wiki/Ion_cyclotron_resonance#Ion_cyclotron_resonance_heating), [ECRH](https://en.wikipedia.org/wiki/Electron_cyclotron_resonance), [neutral beams])https://en.wikipedia.org/wiki/Neutral-beam_injection)). Steam driven pistons are a relatively simple technology, so they should be low cost per unit power delivered to the plasma. They also can directly use the steam power already created as part of the heat-to-electricity conversion system in the plant, saving on conversion efficiencies to other heating technologies.

A major "why now?" question for General Fusion has been within this driver technology. Inertial fusion requires very symetric implosions. One piston being slightly off would be ruinous to effective compression. Modern control electronics, as the General Fusion story goes, now allows for precise enough control of the pistons to enable symetric enough implosions.

## Learnings from General Fusion

1. **The middle ground is an interesting place to look for fusion energy systems.** At the time of General Fusion's founding in the early 2000s, the global fusion research had largely calcified into big-magnetic (ITER) and big-inertial (NIF). General Fusion opened up the area in between for a whole new generation of scientists and engineers. Concepts in the intermediate density will have catching up to do in plasma performance. Still, there is a very wide playing field to look for better overall fusion energy systems.

2. **There is appetite for more than one private fusion company.** TAE is the pioneer of the modern private-fusion era. General Fusion is the second mover, and the first to validate TAE’s business model, [turning a lone nut into a leader](https://sive.rs/ff).

3. **Iterate, iterate, iterate.** In the face of plasma compression challenges, General Fusion continued to iterate on the target plasma it was using as well as how they compressed it.

## Agree with General Fusion

1. **Fusion has to be designed as a power plant, not just a plasma experiment.** For fusion energy production to be economically competitive

2. **The first-wall/blanket problem is existential, and thick liquid metal concepts are worth taking seriously.**

3. **Cost and manufacturability matter, so exploring drivers that might avoid ultra-expensive systems is legitimate. **

4. **magneto-inertial / magnetized-target fusion is a real, recognized research area that combines elements of magnetic and inertial approaches—and it warrants careful experimental validation.**


## General Fusion critiques

While General Fusion claims to operate at an optimal density between magnetic and inertial fusion, combining the best of those two worlds, it could also be combining the worst of them as well. It is both:
  1. *a plasma physics problem:* they need to make a magnetically confined target that stays well behaved and
  2. *a pulsed hydrodynamics problem:* they need to compress it cleanly and repeatably.

### Squeezing jelly with rubber bands

General Fusion relies on the compression being adiabatic, which means that little to no energy leaks out while the plasma target is compressed. In practicle this means that the energy confinement time of the target during compression is longer than that of the time it takes to compressively heat it. If the energy confinement time is less than the compression time, then energy leaks out and the target does not heat up enough to get to fusion energy production conditions.

Just because a target plasma is well performing and initial compression looks good, does not mean that it can be compressed all the way to fusion conditions. Especially challenging for magnetized target fusion is the evolution of the magnetic confinement of the plasma as it is heated up and densified. As described above, the plasma beta increases with compression and is limited in how high it can go. [Edward Teller](https://en.wikipedia.org/wiki/Edward_Teller) memorably described the challenge of magnetic confinement as being like trying to [hold together a blob of jelly with rubber bands](https://research.princeton.edu/news/celebrating-lyman-spitzer-father-pppl-and-hubble-space-telescope): the harder you hold onto it, the more that squeezes out. 

General Fusion has learned, through years of compressing different magnetic target plasmas, just how challenging plasma compression is. A history is given in a following section.

### Holding water upsidedown in a cup

Rotating the liquid metal liner opened up a [void in the center](https://en.wikipedia.org/wiki/Vortex#Pressure_in_a_vortex), into which the plasma can be injected. The liquid rotation also helps reduce [Rayleigh Taylor instabilities](https://en.wikipedia.org/wiki/Rayleigh%E2%80%93Taylor_instability), a major challenge in fusion plasma confinement. 




The compression challenges are in part evident in the evolution of General Fusion's target plasma strategy. 
- From conception through as late as 2008, it had published that its target plasma was a [Field-Reversed Configuration (FRC)][https://doi.org/10.1007/s10894-007-9091-4].
- A later publication that year stated it was a ["spheromak-like or an FRC-like plasma"](https://doi.org/10.1007/s10894-008-9167-9).
- By 2013 it appears to have coallesced into a [spheromak](https://doi.org/10.1063/1.4819307) target.
- In 2015 ["transition from familiar spheromak behavior to tokomak-like [sic] behavior"](https://www.afs.enea.it/project/protosphera/Proto-Sphera_Full_Documents/EPR2016/Contributions/Acoustically_Driven_Magnetized_Target_Fusion.pdf).
- In 2017 it had transformed into the [spherical tokamak](https://doi.org/10.1007/s10894-018-0180-3) target they use to this day.

In a [2013 paper](https://proceedings.cns-snc.ca/index.php/pcns/article/view/6765) about their acoustic concept, they say the earlier LINUS-style liner “could not be accelerated to sufficiently high velocities to compress plasma within its thermal lifetime,” and describe their acoustic wave compressing “in less than 200 µs,” matched to “practically achievable plasma lifetimes.” They had to move away from this fast compression concept because, as indicated in a [2018 poser](https://generalfusion.com/wp-content/uploads/2022/05/ICPP_2018_OShea.pdf) the large magnetic fields that resulted because of the fast and high compression would vaporize the surrounding metal. This both allowed magnetic flux to diffuse away as well as the vapor could penetrate the plasma, causing radiation losses. Thus, they moved back to a slow compression concept, which required a target with much better energy confinement and the move to a spherical tokamak target.



### Calculatus eliminatus
*[The way to find a missing something is to find out where it's not](https://www.youtube.com/watch?v=KoBhw3nvBkc)*

### Rep rate problem

Even if General Fusion could get one fusion pulse to work, the repetition rate is then the key determinant if it is an economic energy source. There are many things that could limit this.
