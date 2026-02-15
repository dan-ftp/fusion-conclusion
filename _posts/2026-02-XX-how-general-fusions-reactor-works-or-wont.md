---
layout: post
title: "How General Fusion's reactor will work (or won't)"
published: false
---
<p><img src="{{ site.baseurl }}/content/images/2025/12/DPK-TAE-Technologies-Norm-Rendering-Exterior-Full-View-Cropped.jpg" alt="How TAE's fusion reactor will work (or won't)"></p>

*Closely following TAE's merger with the public company TMTG, General Fusion has [announced](https://generalfusion.com/post/general-fusion-business-combination-announcement/) that they are [going public through a SPAC](https://generalfusion.com/wp-content/uploads/2026/01/General-Fusion-Investor-Presentation-January-2026-2.pdf). As with my [TAE article](https://www.fusionconclusion.com/how-taes-fusion-reactor-will-work-or-wont/), I aim to answer for non-experts: "What, exactly, is General Fusion building and how close is it to working?"*

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

A problem that spans most fusion concepts—magnetic confinement, inertial confinement, and magnetized target alike—is the [Rayleigh–Taylor instability](https://en.wikipedia.org/wiki/Rayleigh%E2%80%93Taylor_instability) (RTI), among other [hydrodynamic instabilities](https://en.wikipedia.org/wiki/Hydrodynamic_stability). RTI occurs when a light fluid  supports a heavy fluid: small interface perturbations can grow and drive mixing.

A helpful tabletop analogy is the “upside-down glass of water” family of demos. Hydrostatics makes the setup seem plausible: atmospheric pressure corresponds to roughly a 10 m water head. So an inverted, water-filled container can be in static force balance in principle and it typically is when a playing card is used between the water-air interface. But dense water sitting above light air is an unstable equilibrium: once the water–air interface deforms, perturbations can grow and the configuration fails in the Rayleigh–Taylor sense.

This maps to fusion because gravity is replaced by an effective acceleration from inertia, pressure gradients, or magnetic curvature/field gradients. For liner-based approaches (including dense liquid-metal liners compressing a much lower-density plasma), the same intuition applies: keeping interfaces smooth during rapid acceleration is hard, and hydrodynamic instabilities are a common failure mode. Much of the research is in techniques to reduce 

### Calculatus eliminatus
*[The way to find a missing something is to find out where it's not](https://www.youtube.com/watch?v=KoBhw3nvBkc)*

From the outside, General Fusion's MTF experiments may look like an exercise in The Cat in the Hat's Calculatus eliminatus: figuring out every plasma target that's not stable through compression to find the one that is. But, to be fair, there is logic to what they tried and they learned along the way. The many different things they tried demonstrates how hard their plasma compression challenge is.

From conception through as late as 2008, General Fusion had published that its target plasma was a [Field-Reversed Configuration (FRC)][https://doi.org/10.1007/s10894-007-9091-4] and that it was using a very fast compression to outrun the relatively poor energy confinement of the FRC. The FRC was created by injecting a [spheromaks](https://en.wikipedia.org/wiki/Spheromak) from each side of the liquid metal vortex. This has the benefit of easy "catching" within the vortex due to the near zero velocity of the FRC after spheromak merger. The spheromaks were injected with opposite helicity, which converts much of the toroidal magetic field energy into ion heating.

Some time in 2008 it became clear General Fusion was exploring options beyond the FRC, publishing on ["spheromak-like or an FRC-like plasma"](https://doi.org/10.1007/s10894-008-9167-9) in a publication on their plasma accelerators. It it they explored potential ways the spheromak merger could go wrong and postulated that injecting a single plasma could be an option.

Experimental compression results in [2013 were only on spheromaks](https://doi.org/10.1109/SOFE.2013.6635495), with no mention of FRCs. While a compression of $2\times$ showed increases in plasma temperature and density as expected, a $4\times$ compression had and electron temperature "far below adiabatic expectations", indicating heat was leaking out. In that work General Fusion also had results from their small scale liquid metal vortex and compression experiment, which had 14 pistons to form a compression wave. The pistons were able to reach their design velocity and timing. But, it was found that there was significant liquid metal spray into the center of the vortex, which would be ruinous if there were a plasma inside. The spray was postulated to be due to a combination of the (Richtmyer–Meshkov instability)[https://en.wikipedia.org/wiki/Richtmyer%E2%80%93Meshkov_instability] (the impulse limit of the Rayliegh-Taylor instability) and (cavitation)[https://en.wikipedia.org/wiki/Cavitation].

This was a double-whammy of bad news: The plasma targets confinement was margingal, indicating that very fast compression was needed for even a hope of getting to fusion conditions. But faster compression increases hydrodynamic stability and symmetry requirements. The easiest system‑level way out was to improve target confinement by changing targets so they can compress more gently, reducing the instability drive.

In 2015 it was reported that the target had evolved into a tokamak. The experimental setup had a shaft in the center of the plasma in which current could be drien and case a ["transition from familiar spheromak behavior to tokomak-like [sic] behavior"](https://www.cns-snc.ca/wp-content/uploads/2021/12/no-04-CWFEST-B-CASSIDY-2015-10-18-General-Fusion.pdf). The tokamak targets had increased plasma lifetimes due in part to reduced plasma turbulence and radiation.

A [full reconceptualization](https://doi.org/10.1007/s10894-018-0180-3) of General Fusion's system was published in 2019. It was to use a spherical tokamak as the target plasma due the high beta potential (~40%). Compression was no longer driving by an accoustic shock wave in the liquid metal liner but instead by a slower pushing of liquid into the chamber by external pistons. 

The high toroidal magnetic field needed to maintain the superior plasma confinement came at an expense. The fusion gain, Q, was estimated to be near unity due to the harder compressibility of the strong toroidal magnetic field. This then requires effecient energy recapture by the liner and pistons. It also complicated the core of the machine: what once only contained the liquid metal liner and plasma now also had to have an electrical conductor running down the center.

To test the new slow compression concept, General Fusion built and operated a pair of experiments. The first being the Cylindrical Water Compressor (CWC). At 1/10th the scale of their Fusion Demonstration Prototype, the goal of the CWC was to demonstrate, using water, that liner rotation along with a slower compression would supress the hydrodynamic instabilities seen in previous fast compressions. Results [published in 2024](https://doi.org/10.1016/j.fusengdes.2023.114087) demonstrated compression ratios approaching 8 and liner perturbations <10%, in comparison to a calculated [compression ratio of 12[(https://firefusionpower.org/FPA24_3-7_Laberge_GENFUS.pdf) to surpass the Lawson criterion..

The second experiments involved plasma formation, injection, and compression. General Fusion has [achieved their target energy confinement time of ~10 ms](https://iopscience.iop.org/article/10.1088/1741-4326/adb8fb), hitting a best energy confinement time of 12 ms with $6\times10^19 m^{-3}$ plasma density and 400 eV plasma temperature. This injector was incorperated onto Lawson Machine 26 (LM26) in early 2025. LM26 uses a solid lithium liner that is compressed with external electromagnets to compress the plasma target. It was [reported](https://generalfusion.com/post/watch-general-fusions-lm26-achieves-first-plasma-compression/) that initial compression tests resulted in densification and heating. 

By late spring 2025, the General Fusion CEO [wrote an open letter](https://web.archive.org/web/20260113160615/https://generalfusion.com/post/open-letter-from-ceo-greg-twinney-general-fusion-at-a-crossroads/) describing a funding crises for the company that resulted in reducing LM26 experiments and laying off 25% of the staff. This letter has since been removed from the General Fusion website since the SPAC announcement. 

From the outside, this situation does not look good. Why would the company struggle to raise funds after reportedly making progress? If I were an investor in General Fusion and the initial LM26 results were promizing, I would invest more to keep it going.

### Lawson benchmarking

As with TAE, General Fusion has made some performance improvements but is nowhere near the conditions needed for fusion energy production. What General Fusion does have on TAE though is they are setting the bar lower and only aiming for deuterium-tritium fuel. 

General Fusion has published a lot on their pre-compression target plasma parameters, but has only one peer-reivewed compressed plasma data point (PCS-16) to plot against the Lawson criterion. Because of this, I will also include the pre-compression PI3 results to show where they are presently starting from. The energy confinement time in PCS-16 was ~35% of the compression time, so it was not adiabatic. The ion temperature in the PCS-16 compression was $\sim 40 \times$ less than the Lawson minimum and the Lawson parameter $\sim 400 \times$ less. The PI3 pre-compression results demonstrated they improved the target performance

<figure>
  <img src="{{ site.baseurl }}/content/images/2026/gf_ti_progress.png" alt="General Fusion's one published compressed plasma ion temperature measurement compared to the minimum needed for D+T fusion.">
  <figcaption>General Fusion's one published compressed plasma ion temperature measurement compared to the minimum needed for D+T fusion.</figcaption>
</figure>

<figure>
  <img src="{{ site.baseurl }}/content/images/2026/gf_lawson_progress.png" alt="General Fusion's one published compressed plasma Lawson parameter measurement compared to the minimum needed for D+T fusion.">
  <figcaption>General Fusion's one published compressed plasma Lawson parameter measurement compared to the minimum needed for D+T fusion.</figcaption>
</figure>

Given how far General Fusion is away from what is needed, it is hard to take the title of their SPAC investor slide seriously: [*An Engineering Approach to Delivering Fusion Energy*](https://generalfusion.com/wp-content/uploads/2026/01/General-Fusion-Investor-Presentation-January-2026-2.pdf). There is a lot of plasma physics left to be done!

### Repetition rate problem

Even if General Fusion could get one pulse to fusion energy production levels, the repetition rate is then the key determinant if it is an economic energy source. This is because each plasma pulse only delivers a certain amount of energy and the plant must deliver power to make a profit. So the profitability determines the minimum repetition rate and a higher rate results in a more profitable system. The primary challenge here is the coupled injection-compression-evacuation-reset problem. The plasma must be formed externally to the chamber, translated into the chamber, and compressed to fusion conditions. The byproducts, unused fuel, and vaporized liner must then be evacuated from the chamber, likely aided by condensation on the liquid metal liner. The rotating liquid metal line must rest to allow the next plasma to be injected.


## Conclusions

General Fusion's story has always been around "engineering" their way to fusion energy and operating at an optimal middle density. On paper their reactor looks attractive: inject a simple magnetized plasma into the center of a rotating liquid metal liner and compress it with steam driven pistons. No fancy schmancy superconducting magnets and no highfalutin lasers. But, their own history of performance has clearly demonstrated that a simple-on-paper fusion concept does not make it simple in practice.  

![General Fusion, like TAE, has had over a decade of slipping fusion commercialization timeline claims. Unlike TAE, General Fusion seems to be ~50% more pessimistic on how far away they are from commercialization.](/assets/images/gf_timeline_transparent.png)

Over a decade has been spent on finding less-bad plasmas targets to compress and dealing with hydrodynamic instabilities in their liquid metal liner. Yet, the company has barely improved plasma performance relative to the Lawson criterion and is no closer to their commercialization predictions than when the company started. 

Like TAE going public, General Fusion going public is more likely a sign of financing of last resort than being ready for commercial fusion energy production. 

