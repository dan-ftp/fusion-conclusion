---
layout: post
title: "How Avalanch Energy's fusion reactor will work (or won't)"
published: False
---
<p><img src="{{ '/content/images/2026/avalanch_energy_reactor.png' | relative_url }}"
     alt="How General Fusion's reactor will work (or won't)"></p>

*It has [leaked](https://www.axios.com/pro/climate-deals/2026/05/27/avalanche-energy-jefferies-fusion-ipo) that Avalanche Energy is working to IPO. As with my [TAE](https://www.fusionconclusion.com/how-taes-fusion-reactor-will-work-or-wont/) and [General Fusion](https://www.fusionconclusion.com/how-general-fusions-reactor-will-work-or-wont/), I aim to answer for non-experts: "What, exactly, is Avalanch Energy building and how close is it to working?"*

This piece is the third in a series where I'll explain the fusion reactor concepts being pursued by fusion companies and then evaluate the company claims using the standard metrics of fusion physicists: plasma temperature, density, and confinement.

## Background

2021-06-17 filed [SEC Form D](https://www.sec.gov/Archives/edgar/data/1867964/000186796321000002/xslFormDX08/primary_doc.xml), indicating incorperated in 2018 with Robin Langtry and Brian Rioand as executive officers and directors and Matthew Nordan as a director with a total sold of $5,131,980 among 15 investors. 

2021-09-02 filed the patent [Orbital confinement fusion device](https://patents.google.com/patent/US11568999B2/en), laying the basic architecture of their concept.

2022-03-30 emerged from stealth as [Blue Origin vets unveil startup seeking small solution to massive challenge of fusion energy](https://www.geekwire.com/2022/blue-origin-vets-unveil-startup-seeking-small-solution-to-massive-challenge-of-fusion-energy/). "The simpler, seemingly elegant approach has left them wondering if it’s possible that no one else has developed or patented the design — or done the research showing it won’t work." "The system that Avalanche Energy is developing would measure about the size of a large shoe box (one-foot diameter, two-feet long). It could be deployed as multiple units to power cargo ships, airplanes and other sectors of the economy that are going to be tricky to wean off of fossil fuels. They estimate it would take six of the devices, for example, to power a passenger car." "Avalanche Energy’s $5 million first round was led by Prime Impact Fund (now Azolla Ventures) and included Congruent Ventures, Chris Sacca’s Lowercarbon Capital, and nearly a dozen smaller investors." "While researching the field, Langtry came across a graduate thesis from a Lockheed Martin researcher named Tom McGuire. It included open source code for simulations for an electrostatic fusion reactor. The idea became the seed for Avalanche Energy’s technology." 

2022-05-17 [won a Defense Innovation Unit prototype contract](https://www.diu.mil/latest/powering-the-future-of-space-exploration-diu-launching-next-generation) for next generation nuclear propulsion in space.

2022-05-26 [This tiny fusion reactor is made out of commercially available parts](https://www.canarymedia.com/articles/nuclear/this-tiny-fusion-reactor-is-made-out-of-commercially-available-parts). “It’s hundreds of little cells that we can mass-produce in a giga-fusion factory. You might need a few of them for a car, a dozen for a bus, maybe 100 for an airplane.” "Avalanche can run real-world experiments a few times per week on single-digit millions” of dollars, according to Clay Dumas, general partner at Lowercarbon Capital and an investor in Avalanche." "The magnetron used by the startup is a variation of a device ​“found in everyday microwave ovens” that enables the ​“densities and cross sections necessary for fusion,” according to Avalanche investor Joshua Posamentier, a managing partner at Congruent Ventures." "its physics didn’t want to be in a form factor larger than a fire extinguisher" "Avalanche anticipates that the proposed modular fusion cell, which will have a diameter of approximately 5 inches, will produce 5 to 15 kilowatts of power." "to build a ​“recirculating beam fusion” prototype" "Avalanche’s CEO also promises a compressed go-to-market schedule: ​“We’re not 10 years away. We’re a lot closer than that.”" 

2023-10-06 [Avalanche Tackles the Next Milestone with NSF Grant](https://web.archive.org/web/20240424200704/https://avalanchefusion.com/blog/avalanche-fusion-nsf-grant/) (404'd on their website). "$275K grant from the National Science Foundation" "Over the next year, our scientists and engineers will be heads down, with their ultimate goal being a technical path to achieving net-positive energy (that's Q>1) using The Orbitron." "The grant focuses on computational fusion gain factor (Q) predictions for Orbitron-based fusion microreactors. We're about improving our modeling game and validating Particle-in-Cell (PIC) code using real-world data." 

2023-10-24 [Behind the Scenes of Our Compact Fusion Machines](https://www.avalanchefusion.com/blog/cwfest2023). "Avalanche’s compact fusion machine is markedly different here; its fusion core can be held in your hands, and fully integrated could fit in a pickup bed." "What important truth the very few people agree with you on? ... So what I'm here to tell you today is that fusion reactors do not need to be large billion dollar machines. Small fusion power can be mobile, distributed and mass produced at scale, kind of like a Tesla battery pack." "The electrons mitigate space charge and help you get to really high plasma densities. The second thing electrons do is their co-rotating with the ions. And so we have to worry about ion thermalization, right. And so electrons are light, they travel really fast. If they're co-rotating with the ions, you can think of them almost like a tailwind at the back of the ions. And if we can get the right tail wind force, we can actually have the ions burn longer long enough to fuse significantly." "And so that would be making sort of mid to high 10 to the 11 neutrons per second, which is a really interesting neutron source. And then if you're operating with deuterium tritium, that would be about a kilowatt. And so if our cathode is consuming 600 Watts and our iron guns are consuming 400 Watts, that is essentially like a huge sigh of something like one in that device." Also a bunch of physics claims to dig into...

2024-01-17 [Fusion Powered Space Travel](https://www.avalanchefusion.com/blog/fusion-powered-space-travel). Just an announcement of their DIU project.

2024-04-02 second patent [Orbital confinement fusion device](https://patents.google.com/patent/US11948697B2/en)

2024-04-24 [Avalanche Energy Achieves Record 200kv Electrostatic Fusion Milestone and Closes $40 Million Series A Funding Round](https://www.avalanchefusion.com/news-release/avalanche-energy-achieves-record-200kv-electrostatic-fusion-milestone-and-closes-40-million-series-a-funding-round). "$40M Series A round led by Lowercarbon Capital, with major participation from Founders Fund and Toyota Ventures. Also following on their Seed round investment are Congruent Ventures, Grantham Foundation and Clear Path. New participants also included Autodesk, MCJ Collective and the Climate Capital Syndicate." "Avalanche recently operated their second prototype reactor at 200 kilovolts making it the highest known operating voltage of any fusion device since the University of Wisconsin at Madison produced 190 kilovolts in a 2006 experiment." 

2024-07-02 [SF Deep Tech Week Recap with Robin Langtry](https://www.avalanchefusion.com/blog/2024-deep-tech-week). Fluff piece but mentioned "show off for the first time our prototype chip for direct energy conversion of fusion plasmas to electricity".

2024-08-01 first peer-reviewed paper [The Orbitron: A crossed-field device for co-confinement of high energy ions and electrons](https://doi.org/10.1063/5.0201470).

2025-01-07 patent [Compact high voltage electric feedthrough](https://patents.google.com/patent/US20250210952A1/en).

2025-04-10 — [Announced FusionWERX in Richland, Washington](https://www.avalanchefusion.com/news-release/avalanche-energy-announces-new-fusionwerx-test-facility-to-accelerate-commercial-fusion-development). "usionWERX is intended to serve as a first-of-its-kind commercial-scale testing facility for advanced fusion technologies, offering access to private companies, universities, national laboratories, and public-private consortia working to accelerate the path to commercial fusion power.‍FusionWERX will operate under a broad-scope radioactive materials license and will have one of the most advanced tritium handling capacities available in the private sector when fully licensed and operational." "High flux fusion neutron sources based on Avalanche's proprietary Orbitron platform, providing tunable neutron energy environments from high energy 14.1 megaelectron volts (MeV) to thermal neutrons for materials testing and fusion system validation.
Blanket and shielding test beds that will enable the demonstration of purpose-fit technologies applicable to multiple plasma and fusion device architectures.
Hot cells designed for remote handling, processing, and analysis of activated materials.
Integrated tritium management systems capable of extracting, purifying, and recycling tritium for continuous experimental operation." "Avalanche also announced that it agreed to a Memorandum of Understanding (MoU) with Fusion Fuel Cycles (FFC), one of the world's leading providers of fusion fuel cycle technologies." "Along with managing the FusionWERX operations, Avalanche intends to incubate a number of neutron-enabled businesses focused on imaging/sensing, radiation effects testing, and fusion materials development. The site will also be the location where Avalanche will operate its Q>1 deuterium-tritium test program with the goal of developing the world's first net-energy compact fusion reactor system." Image at the end of the article finally indicates they realize they need sheilding. 

2025-07-22 [Avalanche Energy Completes Final Series A Voltage Milestone: 300,000 Volts in Compact, High-Efficiency Prototype Fusion Machine](https://www.avalanchefusion.com/news-release/avalanche-energy-completes-final-series-a-voltage-milestone-300-000-volts-in-compact-high-efficiency-prototype-fusion-machine). "Seattle-based Avalanche Energy has achieved a critical high-voltage milestone in its pursuit of compact fusion: sustaining 300,000 volts across just two and a half inches of space—equating to an average electric field gradient of over 4.7 megavolts per meter (MV/m). That field strength rivals some of the steepest natural voltage gradients on Earth—exceeding even lightning—and does so in steady-state, using just 3 watts of power. " Has a graph of voltage and field gradeitns, getting data on C-Mod for comparison (~1 kV and 300 kV/m).

2025-07-23 [Avalanche Energy hits key milestone on the road to a desktop fusion reactor](https://techcrunch.com/2025/07/23/avalanche-energy-hits-key-milestone-on-the-road-to-a-desktop-fusion-reactor/). "Avalanche recently operated its desktop fusion machine for hours on end while maintaining 300,000 volts, a figure the startup predicts will allow it to build a reactor capable of generating more energy than it consumes, the holy grail for any fusion company. " "Sales of radioisotopes and rentals of the FusionWERX facility should make Avalanche profitable in 2028, he said. Langtry is forecasting that the company will generate $30 million to $50 million in revenue in 2029."

2025-09-01 [Mode-enhanced ion loading in a 100 kV orbitrap](https://doi.org/10.1063/5.0278177)

2025-12-19 [Hammerhead: a compact 300 kV vacuum bushing](https://www.nature.com/articles/s41467-025-66194-w)

2026-02-03 [Avalanche Energy Raises $29 Million Following Plasma Physics Breakthroughs](https://www.avalanchefusion.com/news-release/avalanche-energy-raises-29-million-following-plasma-physics-breakthroughs). " $29 million in new funding led by RA Capital Management. New investors include 8090 Industries, Overlay Capital, and others, with full participation from existing investors Congruent Ventures, Founders Fund, Lowercarbon Capital, and Toyota Ventures" "provides the private matching funds for Avalanche's $10M grant issued in July 2025 by the Washington State Department of Commerce Green Jobs Grant Program" "We've achieved significant breakthroughs on the plasma physics side that have kept us intensely focused on advancing our technology over the past six months," said Robin Langtry, CEO and co-founder of Avalanche Energy. "The new funding will enable us to accelerate the company to the next phase - achieving licensing for commercial-scale fusion operations and preparing for our Deuterium-Tritium Q>1 test program. The strong support from both existing and new investors validates the technical progress we're making toward practical fusion energy." "Avalanche's modular design can be stacked for near-endless power applications and unprecedented energy density to provide clean energy for applications in austere and grid-challenged settings (space propulsion, underwater UAVs, data centers, military bases, etc.). "

2026-02-03 [Avalanche thinks the fusion power industry should think smaller](https://techcrunch.com/2026/02/03/avalanche-thinks-the-fusion-power-industry-should-think-smaller/). "Currently, Avalanche’s reactor is only 9 centimeters in diameter, though Langtry said a new version grows to 25 centimeters and is expected to produce about 1 megawatt. That, he said, “is going to give us a significant bump in confinement time, and that’s how we’re actually going to get plasmas that have a chance of being Q>1.”" "Langtry wouldn’t commit to a date when he hopes Avalanche will be able to generate more power than its fusion devices consume, a key milestone in the industry. But he thinks the company is on a similar timeline as competitors like CFS and the Sam Altman-backed Helion. “I think there’s going to be a lot of really exciting things happening in fusion in 2027 to 2029,” he said." 

2026-02-20 [Avalanche Energy Awarded $1.25M AFWERX Contract to Accelerate Advanced Materials Development](https://www.avalanchefusion.com/news-release/avalanche-energy-awarded-1-25m-afwerx-contract-to-accelerate-advanced-materials-development). Nothing of note in the blog, need to find award for details.

2026-04-08 [Avalanche Energy Awarded $5.2M DARPA Contract to Develop Radioisotope Power Technology](https://www.avalanchefusion.com/news-release/avalanche-energy-awarded-5-2m-darpa-contract-to-develop-radioisotope-power-technology). "awarded a $5.2 million contract from the DARPA Rads to Watts program to develop next-gen technology for compact, resilient, nuclear batteries. The 30-month program will mature technologies that directly support Avalanche's mission to commercialize practical, portable fusion power." "the underlying physics is directly relevant to Avalanche's long-term fusion roadmap: converting energetic charged particles into electricity with high efficiency" "will first be used for radioisotope-produced alpha particles, but ultimately support direct energy conversion from the same particles produced in their fusion machines" "The very same fusion machines that produce high-energy alpha particles will also produce high-energy neutrons. The neutrons produced are also efficient at creating the same radioisotopes needed for the Rads to Watts program, creating a reinforcing supply-and-technology flywheel around Avalanche’s core fusion platform."

2026-04-08 [How nuclear batteries could speed the race to fusion power](https://techcrunch.com/2026/04/08/how-nuclear-batteries-could-speed-the-race-to-fusion-power/) "They’ve been around for a while, but they’re not very effective. Existing radiovoltaics are easily damaged by the very radiation they harness and don’t produce that much electricity."



## Framing the discussion

Due to the contentious nature of discussions on different fusion energy concepts, I will frame it using [Rapoport’s Rules](https://www.fusionconclusion.com/how-taes-fusion-reactor-will-work-or-wont/#framing-the-discussion) as I had done in the TAE article: first restating their position, then giving what I learned and what I agree with them on, and finally a critique of what they've done and where they need to go to be relevant for fusion energy production.

## Avalanch Energy's public position

<figure>
  <img src="{{ '/content/images/2026/General_Fusion_steampunk.png' | relative_url }}"
     alt="General Fusion’s steampunk-looking liquid metal compression experiment.">
  <figcaption>General Fusion’s steampunk-looking liquid metal compression experiment, from <a href="https://www.scientificamerican.com/article/can-small-fusion-energy-start-ups-conquer-the-problems-that-killed-the-giants/">Scientific American</a>.</figcaption>
</figure>


## Learnings from Avalanch Energy

1. **TBD.** TBD.

## Agree with Avalanch Energy

1. **TBD.** TBD.

## Avalanch Energy critiques


### Lawson benchmarking

<figure>
  <img src="{{ '/content/images/2026/General_Fusion_Lawson_progress.png' | relative_url }}"
     alt="General Fusion's progress on the Lawson diagram.">
  <figcaption>General Fusion's progress on the Lawson diagram.</figcaption>
</figure>

## Conclusions

<figure>
  <img src="{{ '/content/images/2026/gf_timeline_transparent.png' | relative_url }}"
     alt="General Fusion, like TAE, has had over a decade of slipping fusion commercialization timeline claims. Unlike TAE, General Fusion seems to be ~50% more pessimistic on how far away they are from commercialization.">
  <figcaption>General Fusion, like TAE, has had over a decade of slipping fusion commercialization timeline claims. Unlike TAE, General Fusion seems to be ~50% more pessimistic on how far away they are from commercialization.</figcaption>
</figure>

### About the author

<p><a href="https://www.linkedin.com/in/dan-brunner/" rel="noreferrer">Dan Brunner</a> has a PhD in Applied Plasma Physics from MIT. He is one of the co-founders and former Chief Technology Officer of <a href="https://www.cfs.energy/" rel="noreferrer">Commonwealth Fusion Systems</a> (CFS), "the world's largest and leading commercial fusion energy company." He built and led the team of scientists and engineers that did the conceptual design of <a href="https://www.cfs.energy/technology/sparc" rel="noreferrer">SPARC</a>, the D+T tokamak being built by CFS to demonstrate net fusion energy before 2030. He is now advising fusion investors and startups through <a href="https://futuretech.partners/" rel="noreferrer">Future Tech Partners</a>.</p>
