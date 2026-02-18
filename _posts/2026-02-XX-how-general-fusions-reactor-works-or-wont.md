---
layout: post
title: "How General Fusion's reactor will work (or won't)"
published: false
---
<p><img src="{{ site.baseurl }}content/images/2026/general_fusion_reactor.jpg" alt="How General Fusion's reactor will work (or won't)"></p>

*Closely following TAE's merger with the public company TMTG, General Fusion has [announced](https://generalfusion.com/post/general-fusion-business-combination-announcement/) that they are [going public through a SPAC](https://generalfusion.com/wp-content/uploads/2026/01/General-Fusion-Investor-Presentation-January-2026-2.pdf). As with my [TAE article](https://www.fusionconclusion.com/how-taes-fusion-reactor-will-work-or-wont/), I aim to answer for non-experts: "What, exactly, is General Fusion building and how close is it to working?"*

This piece is the second in a series where I'll explain the fusion reactor concepts being pursued by fusion companies and then evaluate the company claims using the standard metrics of fusion physicists: plasma temperature, density, and confinement (plus the realities of power balance and economics).

For this article, I'll start with the story of how General Fusion came to be, tying it to the work done on similar concepts at the U.S. Naval Research Laboratory (NRL) and Los Alamos National Laboratory (LANL). Then I'll lay out General Fusion's argument advocating for its approach to compressing a plasma target to fusion conditions using a steam piston driven shockwave launched into a spinning lead-lithium vortex. Finally, I'll show the company’s progress against what they need to achieve fusion energy and show why many are skeptical that they can achieve it. My goal is to give a clear and sober picture of where General Fusion is and what they need to do to get to where they say they are going.

## Background

Before diving into General Fusion's reactor concept and critiques, it is important to set the stage of how this concept evolved. See my previous article on [TAE](https://www.fusionconclusion.com/how-taes-fusion-reactor-will-work-or-wont/#Background) for a brief history of "mainline" and "alternative" fusion concepts, of which General Fusion is considered an alternative.

### Compressing plasmas in the U.S.S.R., NRL, and LANL

<figure>
  <img src="{{ site.baseurl }}/content/images/2026/MTF-schematic.png" alt="Schematic of a MTF concept.">
  <figcaption>Schematic of a [MTF concept](https://doi.org/10.1109/TPS.2004.823974).</figcaption>
</figure>

In the 1960's, researchers at the Kurchatov Institute in the U.S.S.R. were using rapidly compacted solid metal liners to compress plasmas to near the conditions needed to generate fusion energy, in a process called [magnetized target fusion (MTF)](https://en.wikipedia.org/wiki/Magnetized_target_fusion). This works as follows: a magnetically confined plasma is formed inside of an electrical conductor, in this case a solid. The conductor is compressed rapidly around the plasma. A conductor with sufficiently high electrical conductivity does not allow the magnetic field to penetrate through it on the short timescales of compression. As the plasma is compressed (with $C=R_0/R$ as the ratio between the initial plasma radius $R_0$ and the compressed plasma radius $R$) the magnetic field increases $B \propto C^2$ to conserve magnetic flux. The compression also increases the plasma density $n \propto C^3$ if the particles are well confined and increases the plasma temperature $T \propto C^2$ if the system is [adiabatic](https://en.wikipedia.org/wiki/Adiabatic_process) and does not leak energy during the compression.

Getting to fusion energy production conditions requires that the magnetic field confines the plasma all the way through the compression. However, there is a finite limit to which any given plasma can be stably compressed. For instance, in adiabatic compression, beta increases as $\beta \propto C$, where [beta](https://en.wikipedia.org/wiki/Plasma_beta) ($\beta$) is the ratio of the plasma pressure to the magnetic pressure. Every magnetic fusion plasma has a maximum beta it can support, and it or another physics barrier may limit how far the target can be stably compressed. 

While the U.S.S.R. scientists achieved some success in compressing plasmas, it was realized that the cost of the metal liners would exceed the value of the fusion energy generated. This is a problem common to many of the pulsed fusion concepts where the cost to produce the target and anything else destroyed in the pulse must be less than that of the value of the energy produced. It is termed the "[kopeck problem](https://en.wikipedia.org/wiki/Magnetized_target_fusion#Kopeck_problem)" after Russian [kopeck](https://en.wikipedia.org/wiki/Kopeck), which was worth 0.01 rubles or $0.00013 USD as of mid-February 2026 (it was about the value of a U.S. penny in the 1960's).

The kopeck problem pushed researchers to use liquid liners for compression because the liquid liners could be recycled in situ with minimal efforts to reform the liners between pulses. The NRL and LANL in the U.S. picked up on this concept and did a series of experiments in the 1970's along with detailed reactor conceptual designs through their [Linus program](https://en.wikipedia.org/wiki/Linus_(fusion_experiment)). MTF fusion suffered a similar fate to other alternative fusion concepts and, at least according to its proponents, has been underfunded for decades.

## Framing the discussion

Due to the contentious nature of discussions on different fusion energy concepts, I will frame it using [Rapoport’s Rules](https://www.fusionconclusion.com/how-taes-fusion-reactor-will-work-or-wont/#framing-the-discussion) as I had done in the TAE article.

## General Fusion's public position

<figure>
  <img src="{{ site.baseurl }}/content/images/2026/General_Fusion_steampunk.png" alt="General Fusion’s liquid metal compression experiment.">
  <figcaption>General Fusion’s liquid metal compression experiment, from [Scientific American](https://www.scientificamerican.com/article/can-small-fusion-energy-start-ups-conquer-the-problems-that-killed-the-giants/).</figcaption>
</figure>

Fortunately for this discussion, General Fusion has [published peer-reviewed articles](https://generalfusion.com/post/category/research-library/) on their experiments and their results as well as put out public information on their vision for how that translates to a fusion power plant. While some of the specifics have changed over the years, especially the target plasma, the basic concept has remained constant: Inject a stable plasma into the vortex created in the center of a spinning volume of liquid metal and use precisely-timed pistons to send a pulse through the liquid that compresses the plasma to fusion energy production conditions. This is the most [steampunk](https://en.wikipedia.org/wiki/Steampunk) fusion concept out there and, in my opinion, they missed the marketing opportunity to go hard into the steampunk aesthetic.

General Fusion has the following claimed concept advantages:

### MTF is the optimal between the titans of ITER (magnetic fusion) and NIF (inertial fusion)

<figure>
  <img src="{{ site.baseurl }}/content/images/2026/MTF_optimum.png" alt="General Fusion’s rallying cry for the MTF optimum between ITER and NIF.">
  <figcaption>General Fusion’s rallying cry for the MTF optimum between ITER and NIF.</figcaption>
</figure>

The most common refrain from the MTF proponents is that it operates at intermediate plasma energy and driver power scales compared to magnetic fusion and inertial fusion, which allows MTF to have a simpler and less expensive overall plant. The argument is a natural result of the [Lawson criterion](https://en.wikipedia.org/wiki/Lawson_criterion), which dictates there is a minimum product ($\sim10^{20} s/m^3) of the plasma density and [energy confinement time](https://wiki.fusion.ciemat.es/wiki/Energy_confinement_time) (i.e., how well the system insulates the fusion plasma) and that the two of them can be traded off each other. The justification goes as follows:

Magnetic fusion operates at the low density end of the spectrum ($\sim10^{20}/m^3$) and long ($\sim1 s$) energy confinement time. The long energy confinement requires that the reactor operates effectively in steady-state and has very high stored energy. This translates into needing large, expensive superconducting magnets (>GJ-scale stored energy in the magnets) to maintain plasma confinement. As the plasma density is increased, the size of the required system decreases and therefore, costs associated with the size and stored energy decrease. This is a similar argument used for the high-field path for magnetic fusion energy, which allows for shorter energy confinement times and therefore smaller machines; albeit at less of an extreme change in density as needed for MTF.

Inertial fusion operates at very high density ($\sim10^{31}/m^3$) with very short confinement times ($\sim10^{-10} s$, given by the "stagnation time" of the compression). While reaching these parameters requires no external confinement systems, it requires injecting the energy in very short pulses, which then requires very high pulsed power systems (>TW-scale) that are very expensive. 

MTF proponents predict that the space in between pure magnetic and pure inertial will be a promised land of optimal density that requires modest energy and power scales, where a moderate initial magnetic field helps to contain the plasma and reduce losses, allowing gentler compression forces to densify and heat up the plasma to fusion conditions.

### The liquid lead-lithium metal wall and blanket is the solution to fusion nuclear damage

One of the largest technical hurdles to economic fusion energy development is damage of components by the fusion [neutron bombardment](https://en.wikipedia.org/wiki/Neutron_radiation). The neutrons in fusion, especially the high-energy neutrons of deuterium-tritium fusion, must deposit their energy in whatever comprises the blanket surrounding the fusion plasma. This allows the fusion energy that they contain to be captured and turned into a useful form, typically in a thermal-to-electricity cycle.

The downside is that the neutrons damage solid materials along the way, through changing the material structure and transmutation. This typically degrades the engineered properties of the materials (e.g., structural strength, thermal conductivity, electrical resistivity, etc.) over time. Eventually, the properties of the materials are no longer sufficient for the materials to perform as designed. The materials must then be replaced.

The survivability of materials in a fusion neutron environment is one of the key factors that will determine how well fusion will economically compete with other energy sources. This manifests both in the costs of replacing components as well as the loss of revenue during maintenance periods.

A solution for dealing with the fusion neutron material damage problem is to minimize the amount of solid material in the pathway of neutrons by using liquids wherever possible. While this is not an idea pioneered by General Fusion, they are one of the primary fusion companies pursuing it. Similarly, companies like Commonwealth Fusion Systems and Xcimer, are planning on using a molten salt blanket. 

### Fuel sustainability via tritium breeding

While the [deuterium-tritium](https://en.wikipedia.org/wiki/Deuterium%E2%80%93tritium_fusion) fusion fuel has the easiest requirements on plasma conditions, [tritium](https://en.wikipedia.org/wiki/Tritium) has no significant natural source and must be made. Present supplies are mostly from fission power plants, specifically [CANDU reactors](https://en.wikipedia.org/wiki/CANDU_reactor). A fusion industry based on dueterium-tritium will need [tritium production](https://en.wikipedia.org/wiki/Breeding_blanket#Tritium_breeding) at a much larger scale, likely bred on site from the fusion-produced neutrons and lithium in the blanket.

A major challenge in breeding tritium is making enough to both sustain the use at the reactor it is being produced at as well as producing an excess to supply new fusion reactors. The excess must also account for tritium that gets "stuck" in the system, i.e., effectively trapped as it dissolves into metal and other parts of the system, as well as make up for the 5%/year that decays into [helium-3](https://en.wikipedia.org/wiki/Helium-3) (a valuable byproduct). The figure of merit for this is the tritium breeding ratio (TBR), which is the ratio of the amount of tritium bred to that burned in the reactor. TBR~1.05 is often given as the bare minimum to sustain a single plant. Many designs use a neutron multiplier in the blanket, with beryllium and lead being the most commonly used to increase the TBR.

In toroidal schemes like tokamaks and stellarators, the volume available for a blanket and tritium breeding system is limited resulting in a complex trade-off of space with other systems. The resulting design often ends up having TBRs that are considered marginal: ~1.10-1.15. Some of these designs require the lithium in the blanket to be [isotopically enriched](https://doi.org/10.1016/j.joule.2025.101997) to have more lithium-6, which requires new industrial processes to produce.  Other solid structures that don't contain lithium (e.g., the vacuum vessel and plasma facing components) which need to be between the plasma and the blanket are a major cause for the low TBR.

General Fusion's concept, having a liquid lithium-lead blanket completely surrounding the fusion plasma is essentially the ideal design from a tritium breeding efficiency standpoint: The TBR is almost entirely determined by the blanket material and thickness. If General Fusion could get their system to work, it would have a TBR~1.5, which is more than enough to sustain its own operation and supply a growing fusion economy. Improving TBR from 1.15 to 1.50 results in a $\sim3.5\times$ potential faster ramp up rate for the fusion industry assuming tritium supply is the rate limiting factor.

Note that General Fusion has [switched to a pure lithium blanket](https://infuse.ornl.gov/wp-content/uploads/2024/07/2022a-GF-SRNL-Tritium-Fuel-Cycle-Modelling-and-Optimization.pdf) to avoid the "poisoning" of the high-Z lead that could get into the plasma and radiate power away. With this switch, much of the liquid blanket benefits remain, although the tritium is harder to extract from pure lithium. 

### Steam: the simpler driver

In addition to using drivers and confinement at lower powers and energies, General Fusion claims to have a much simpler driver technology: steam-driven pistons, combining industrial revolution era technology with modern controls and material science. This is in contrast to inertial fusion which uses  the world's most complex and powerful laser systems and magnetic fusion which uses has a variety of bespoke, expensive heat techniques ([ICRH](https://en.wikipedia.org/wiki/Ion_cyclotron_resonance#Ion_cyclotron_resonance_heating), [ECRH](https://en.wikipedia.org/wiki/Electron_cyclotron_resonance), [neutral beams])https://en.wikipedia.org/wiki/Neutral-beam_injection)). Steam driven pistons are a relatively simple technology, so they should be low cost per unit power delivered to the plasma. They also can directly use the steam power already created as part of the heat-to-electricity conversion system in the plant, saving on conversion efficiencies when compared to other heating technologies.

A major "why now?" question for General Fusion has concerned this driver technology. Steam pistons have been around for a while, so why hasn’t anyone successfully used them as a driver in the past? Inertial fusion requires very symmetric implosions. One piston being slightly off would be ruinous to effective compression. Modern control electronics, as the General Fusion argument goes, now allows for precise enough control of the pistons to enable sufficiently symmetric implosions.

## Learnings from General Fusion

1. **The middle ground between magnetic fusion and inertial fusion is an interesting place to look for fusion energy systems.** At the time of General Fusion's founding in the early 2000s, global fusion research had largely calcified into big-magnetic (ITER) and big-inertial (NIF). General Fusion opened up the area in between for a new generation of scientists and engineers. Concepts in the intermediate density range need to catch up with magnetic and inertial fusion  in terms of plasma performance. Still, there is a very wide playing field in which to look for better overall fusion energy systems.

2. **There is an appetite for more than one private fusion company.** TAE is the pioneer of the modern private-fusion era. General Fusion is the second mover, and the first to validate TAE’s business model, [“turning a lone nut into a leader”](https://sive.rs/ff).

3. **Iterate, iterate, iterate.** In the face of plasma compression challenges, General Fusion continued to iterate on the target plasma it was using as well as how they compressed it.

## Agree with General Fusion

1. **Fusion has to be designed as a power plant, not just a plasma experiment.** For fusion energy production to be economically competitive, the end goal must always be kept in mind.

2. **The first-wall and blanket problem is existential, and thick liquid metal concepts are worth taking seriously.** Nuclear and plasma damage of materials is one of the critical problems to solve for fusion, liquids are one of the compelling options to explore as a solution.

3. **Cost and manufacturability matter, so exploring drivers that might avoid ultra-expensive systems is legitimate.** Many fusion concepts appear to be a [Rube Goldberg-style](https://en.wikipedia.org/wiki/Rube_Goldberg_machine) assemblage of complex systems to solve all of the challenges of fusion. Going simpler wherever possible is needed to make fusion competitive. 

4. **Magnetized-target fusion is a real, recognized research area that combines elements of magnetic and inertial approaches and it warrants careful experimental validation.** This field has a large area of opportunity to explore and may ultimately yield economically viable fusion power plants.

## General Fusion critiques

General Fusion claims to operate at an optimal density between magnetic and inertial fusion, combining the best of those two worlds. However, General Fusion is likely to be combining the worst of them as well. This manifests as:
  1. *a plasma physics problem:* General Fusion needs to make a magnetically confined target that stays well behaved; and
  2. *a pulsed hydrodynamics problem:* General Fusion needs to compress the target cleanly and repeatably.

### Squeezing jelly with rubber bands

General Fusion relies on the compression being adiabatic, which means that little to no energy leaks out while the plasma target is compressed. In practice this means that the energy confinement time of the target during compression is longer than that of the time it takes to compressively heat the target. If the energy confinement time is less than the compression time, energy leaks out and the target does not heat up enough to get to fusion energy production conditions.

Just because a target plasma performs well and initial compression looks good, that does not mean that it can be compressed all the way to fusion conditions. Especially challenging for magnetized target fusion is the evolution of the magnetic confinement of the plasma as it is heated up and densified. [Edward Teller](https://en.wikipedia.org/wiki/Edward_Teller) memorably described the challenge of magnetic confinement as being like trying to [hold together a blob of jelly with rubber bands](https://research.princeton.edu/news/celebrating-lyman-spitzer-father-pppl-and-hubble-space-telescope): the harder you hold onto the jelly, the more it squeezes out. 

Magnetic compression has been explored as a heating and densification method in tokamaks – including JET and TFRT, the only two to operate with deuterium-tritium fuel to date – and is the only heating and densification method Helion is using. The [JET](https://scipub.euro-fusion.org/wp-content/uploads/2014/11/JETR99013.pdf) and [TFTR](https://www.osti.gov/servlets/purl/5851324) “experiments on compression heating were unfruitful” due to non-uniform magnetic fields induced in the machine during compression, which reduced the energy confinement. Magnetic confinement was consequently abandoned in favor of other external heating methods.

General Fusion has learned, through years of experimenting with different magnetic target plasmas, the extreme difficulties of plasma compression. In fact, General Fusion and collaborators [published a paper](https://iopscience.iop.org/article/10.1088/1741-4326/ab74a2) examining just how challenging it is to thread the needle of plasma conditions from target to fully compressed plasma.

### Holding water upside down in a cup

A problem that spans most fusion concepts – magnetic confinement, inertial confinement, and magnetized target alike – are [hydrodynamic instabilities](https://en.wikipedia.org/wiki/Hydrodynamic_stability) including the [Rayleigh-Taylor instability](https://en.wikipedia.org/wiki/Rayleigh%E2%80%93Taylor_instability) (RTI). RTI occurs when a light fluid supports a heavy fluid against a body force like gravity: small perturbations at the interface of these two fluids can grow and drive mixing.

A helpful tabletop analogy is the “upside-down glass of water” experiment. Hydrostatics makes the setup seem plausible: atmospheric pressure corresponds to roughly a 10 m water head. So an inverted, water-filled container can in principle be in static force balance and it typically is when a playing card is used between the water-air interface. But dense water sitting above light air is an unstable equilibrium: once the water-air interface deforms, perturbations can grow and the configuration fails as per Rayleigh-Taylor.

This maps to fusion because gravity is replaced by an effective acceleration from inertia, pressure gradients, or magnetic curvature/field gradients. For liner-based approaches (including dense liquid-metal liners compressing a much lower-density plasma), the same intuition applies: keeping interfaces smooth during rapid acceleration is exquisitely difficult, and hydrodynamic instabilities are a common cause of failures that cool the plasma: the non-uniform surface can disrupt the uniformity of the magnetic field, the liner can splash and eject material into the plasma, etc.

### Calculatus eliminatus
*[The way to find a missing something is to find out where it's not](https://www.youtube.com/watch?v=KoBhw3nvBkc)*

From the outside, General Fusion's MTF experiments may look like an exercise in The Cat in the Hat's Calculatus eliminatus: figuring out every plasma target that's not stable through compression to find the one that is. But, to be fair, there is logic to what they tried and they have learned along the way. 

From conception through as late as 2008, General Fusion had published that its target plasma was a [Field-Reversed Configuration (FRC)][https://doi.org/10.1007/s10894-007-9091-4] and that it was using a very fast compression to outrun the relatively poor energy confinement of the FRC plasma. The FRC plasma was created by injecting a toroidally shaped plasma called a [spheromak](https://en.wikipedia.org/wiki/Spheromak) from each side of the liquid metal vortex. This has the benefit of easy "catching" within the vortex due to the near zero velocity of the FRC plasma after the merger of the injected spheromak plasmas. The spheromak plasmas are injected with opposite helicity, which converts much of the toroidal magnetic field energy into ion heating.

Some time in 2008 it became clear that General Fusion was exploring options beyond the FRC as a target, publishing on ["spheromak-like or an FRC-like plasma"](https://doi.org/10.1007/s10894-008-9167-9) in a paper on their plasma accelerators. They report having explored potential ways the spheromak plasma merger could go wrong and postulated that injecting a single plasma as the target for compression is an option.

Experimental compression results in [2013 were only on spheromaks plasmas](https://doi.org/10.1109/SOFE.2013.6635495), with no mention of merging them into FRC plasmas. While a compression of $2\times$ showed increases in plasma temperature and density as expected, a $4\times$ compression resulted in the electron temperature "far below adiabatic expectations", indicating energy was leaking out. 

In that work General Fusion also had results from their small scale liquid metal vortex and compression experiment, which had 14 pistons to form a compression wave. The pistons were able to reach their design velocity and timing. But, it was found that there was significant liquid metal spray into the center of the vortex, which would be ruinous if there were a plasma inside. The spray was postulated to be due to a combination of the (Richtmyer-Meshkov instability)[https://en.wikipedia.org/wiki/Richtmyer%E2%80%93Meshkov_instability] (the impulse limit of the Rayliegh-Taylor instability) and (cavitation)[https://en.wikipedia.org/wiki/Cavitation].

This was a double-whammy of bad news: The confinement of the plasma targets was marginal, indicating that very fast compression was needed for even a hope of getting to fusion conditions. But the speed of their acoustic compressions was already demonstrating ruinous hydrodynamic instabilities. The system‑level way out was to improve target confinement by changing targets so they can compress more gently, reducing the instability drive.

In 2015, General Fusion reported that they evolved their target into a tokamak plasma. The experimental setup had a solid conductor shaft in the center of the plasma in which current could be driven and cause a ["transition from familiar spheromak behavior to tokomak-like [sic] behavior"](https://www.cns-snc.ca/wp-content/uploads/2021/12/no-04-CWFEST-B-CASSIDY-2015-10-18-General-Fusion.pdf). The tokamak plasma targets had increased plasma lifetimes due in part to reduced plasma turbulence and radiation.

General Fusion subsequently published a [full reconceptualization](https://doi.org/10.1007/s10894-018-0180-3) of their system in 2019. The new concept was to use a spherical tokamak plasma as the target due the high beta potential (~40%). Compression was no longer driven by an acoustic shock wave in the liquid metal liner but instead by a slower pushing of liquid into the chamber by external pistons. 

The high toroidal magnetic field needed to maintain the superior confinement in the tokamak plasmas compared to the spheromak plasmas came at an expense. The fusion gain, Q, was estimated to be limited to $\sim1$ due to the harder compressibility of the strong toroidal magnetic field. This then requires efficient energy recapture by the liner and pistons. The new concept also complicated the core of General Fusion’s machine: what once only contained the liquid metal liner and plasma now also had to have an electrical conductor running down the center to maintain the toroidal magnetic field and plasma stability through compression.

To test this new slow compression concept, General Fusion built and operated a pair of experiments. The first being the Cylindrical Water Compressor (CWC). At 1/10th the scale of their Fusion Demonstration Prototype, the goal of the CWC was to demonstrate, using water, that liner rotation along with a slower compression would suppress the hydrodynamic instabilities seen in previous fast compressions. Results [published in 2024](https://doi.org/10.1016/j.fusengdes.2023.114087) demonstrated compression ratios approaching 8 and liner perturbations <10%, in comparison to a calculated [compression ratio of 12](https://firefusionpower.org/FPA24_3-7_Laberge_GENFUS.pdf) needed to surpass the Lawson criterion.

The second experiments involved plasma formation, injection, and compression. General Fusion has [achieved their target energy confinement time of ~10 ms](https://iopscience.iop.org/article/10.1088/1741-4326/adb8fb), hitting a best energy confinement time of 12 ms with $6\times10^{19}/m^{3}$ plasma density and 400 eV plasma temperature. This injector was incorporated onto their new plasma compression device Lawson Machine 26 (LM26) in early 2025. LM26 uses a solid lithium liner that is compressed with external electromagnets to compress the plasma target. General Fusion [reported](https://generalfusion.com/post/watch-general-fusions-lm26-achieves-first-plasma-compression/) that initial compression tests resulted in densification and heating. Going to a tokamak plasma improved the pre-compression target Lawson parameter $\sim30\times$.

Following this late spring 2025, the General Fusion CEO [wrote an open letter](https://web.archive.org/web/20260113160615/https://generalfusion.com/post/open-letter-from-ceo-greg-twinney-general-fusion-at-a-crossroads/) describing a funding crises for the company, “today’s funding landscape is more challenging than ever.” Which conflicts with the fact that about [$3B has been raised by fusion companies](https://www.fusionenergybase.com/articles/full-year-2025-fusion-equity-financing-update) outside of China in 2024-2025. General Fusion’s budget crunch resulted in reducing LM26 experiments and laying off 25% of the staff. This letter has been removed from the General Fusion website since the SPAC announcement. 

From the outside, this situation does not make sense: Why would a company struggle to raise funds after its first major experiments on its machine built to demonstrate Lawson-criterion level conditions? If I were an investor in General Fusion and the initial LM26 results were promising, I would have invested more to keep it going. The answer likely lies in their underwhelming performance with respect to the Lawson criterion.

### Lawson benchmarking

As with TAE, General Fusion has made some performance improvements but is far from the conditions needed for fusion energy production. General Fusion does have an advantage over TAE  in that they are setting the bar lower and only aiming for deuterium-tritium fuel. However, deuterium-tritium fuel will not be enough to get General Fusion over that bar. 

General Fusion has published a lot on their pre-compression target plasma parameters, but has only [one peer-reivewed compressed plasma data point](https://iopscience.iop.org/article/10.1088/1741-4326/ad9033) (PCS-16) to plot against the Lawson criterion. Because of this, I will also include the pre-compression PCS-16 and PI3 results to show where they are starting from. The energy confinement time in PCS-16 was ~35% of the compression time, so it was not adiabatic. The ion temperature in the PCS-16 post-compression was $\sim 40 \times$ less than the Lawson minimum and the Lawson parameter $\sim 400 \times$ less. The PI3 pre-compression results demonstrated they improved the target performance in the Lawson parameter but reduced the pre-compression ion temperature. To get above the minimums needed for the Lawson criterion, LM26 needs to increase the PI3 ion temperature $\sim 60 \times$ and Lawson parameter $\sim 50 \times$.

<figure>
  <img src="{{ site.baseurl }}/content/images/2026/gf_ti_progress.png" alt="General Fusion's one published compressed plasma ion temperature measurement compared to the minimum needed for D+T fusion.">
  <figcaption>General Fusion's one published compressed plasma ion temperature measurement compared to the minimum needed for D+T fusion.</figcaption>
</figure>

<figure>
  <img src="{{ site.baseurl }}/content/images/2026/gf_lawson_progress.png" alt="General Fusion's one published compressed plasma Lawson parameter measurement compared to the minimum needed for D+T fusion.">
  <figcaption>General Fusion's one published compressed plasma Lawson parameter measurement compared to the minimum needed for D+T fusion.</figcaption>
</figure>

Given how far General Fusion is away from what is needed for fusion plasma performance, it is hard to take the title of their SPAC investor slide seriously: [*An Engineering Approach to Delivering Fusion Energy*](https://generalfusion.com/wp-content/uploads/2026/01/General-Fusion-Investor-Presentation-January-2026-2.pdf). There is a lot of plasma physics left to be done!

### Repetition rate problem

Even if General Fusion could get one pulse to fusion energy production levels, the repetition rate is then the key determinant of whether their approach can be an economically competitive energy source. This is because each plasma pulse only delivers a finite amount of energy at a specific time whereas the plant must deliver pulses frequently enough to make sufficient power to turn a profit. So the profitability determines the minimum repetition rate; a higher rate results in a more profitable system. 

The primary challenge here is the coupled injection-compression-evacuation-reset problem: The plasma must be formed externally to the chamber, translated into the chamber, and compressed to fusion conditions. The byproducts, unused fuel, and vaporized liner must then be evacuated from the chamber, likely aided by condensation on the liquid metal liner. The rotating liquid metal line must rest to allow the next plasma to be injected. Successful and rapid repetition of this injection-compression-evacuation-reset cycle is highly non-trivial, and has not come close to being demonstrated.

## Conclusions

General Fusion's story has always been around "engineering" their way to fusion energy and operating at an optimal middle density. On paper, their reactor looks attractive: inject a simple magnetized plasma into the center of a rotating liquid metal liner and compress it with steam driven pistons. No expensive superconducting magnets and no complex lasers. But, their own history of performance has clearly demonstrated that a simple-on-paper fusion concept does not translate to simplicity in practice.  

<figure>
  <img src="{{ site.baseurl }}/content/images/2026/gf_timeline_transparent.png" alt="General Fusion, like TAE, has had over a decade of slipping fusion commercialization timeline claims. Unlike TAE, General Fusion seems to be ~50% more pessimistic on how far away they are from commercialization.">
  <figcaption>General Fusion, like TAE, has had over a decade of slipping fusion commercialization timeline claims. Unlike TAE, General Fusion seems to be ~50% more pessimistic on how far away they are from commercialization.</figcaption>
</figure>

General Fusion has spent over a decade on finding less-bad plasma targets to compress and dealing with hydrodynamic instabilities in their liquid metal liner. Yet, the company has barely improved plasma performance relative to the Lawson criterion and is no closer in time to their commercialization predictions than when the company started. 

General Fusion’s decision to go public is more likely a sign of financing-of-last-resort than of really being ready for commercial fusion energy production. 
