# Thismatters' Eurorack Modules

This is a project to track the progress in replicating and updating modules originally published by [Yusynth](https://yusynth.net/Modular/modular.html). You must check out his site before going any further, he has so much information published there which is omitted from this collection of repositories. I'm just a hobbyist and a fan of his exemplary work. As he states on his site:

> All circuits, schematics, printed circuit board, panel design and associated data published on this site can be used for private use only.

No mass-producing these modules! Friends and family only!

In addition to the Yusynth line I'm also using [Moritz Klien's youtube channel](https://www.youtube.com/@MoritzKlein0) as a source for circuit designs and education. His videos are really fun and informative. It is worth a subscribe!

This is a collection of submodules, each of which is itself a Eurorack format module produced in [KiCAD](https://www.kicad.org/) (an open source circuit design suite). These modules are 3U and 1U sized. Widths are given in HP and referenced from [this random page on the internet](https://midisoft.de/EuroRackDimensions/EuroRack_Dimensions.html). The 1U modules adhere to the [Intellijel Technical Specifications](https://intellijel.com/support/1u-technical-specifications/).

Each of the completed modules below has had at least one prototype manufacturing run and has been installed in my synth cabinet. Some of them require some amount of hacking to be made functional. If that is the case a warning will appear in the notes. Each repo will have a "tag" for each version that has been sent out for a prototype run. Prototype boards are made by [OSHPark](https://oshpark.com/) which sells in lots of three (3) (plan accordingly), and solder paste stencils by [OSHStencils](https://www.oshstencils.com/). If you're doing a run of these modules I fully recommend getting a stencil for the SMD soldering and using good solder paste.

You may find some other Eurorack modules among my repositories which are **not** in this collection. These have not been sent to OSHPark for prototyping or have not been fully assembled and validated. Once they are validated I will add the repo here.

All of the repositories in this collection use this [library of KiCAD symbols and footprints](https://github.com/thismatters/EurorackKiCAD).

## Completed Modules

| Name         | Size | Current PCB | Notes                     |
|--------------|------|-------------|---------------------------|
| [VCO](https://github.com/thismatters/EurorackVco/) | 10hp | [V2](https://oshpark.com/shared_projects/FmhO6zEO) | Works great, but relies on a part which may be really hard to source. |
| [VCA](https://github.com/thismatters/EurorackVca/) | 6hp  | ~[V2](https://oshpark.com/shared_projects/JfrQFvFI)~ | Has bug: used wrong pin markings for Q2 and Q3; component is `BEC` and footprint is `CBE`. This can still be assembled by rotating the Q2 and Q3 parts by like 120 degrees CCW. |
| [ADSR](https://github.com/thismatters/EurorackAdsr/) | 6hp  | [V2](https://oshpark.com/shared_projects/UEztaF3P) | Works great! |
| [LFO](https://github.com/thismatters/EurorackLfo/) | 6hp  | [V0](https://oshpark.com/shared_projects/wfHu28zj) | Really hard to dial in / Doesn't quite work right |
| [Moog VCF](https://github.com/thismatters/EurorackVcf/) | 8hp  | [V0](https://oshpark.com/shared_projects/SO7swty4) | I'm pretty happy with this. |
| [Mult](https://github.com/thismatters/EurorackMult) | 1U 12hp | [V1](https://oshpark.com/shared_projects/OAOenJKo) | Works great! |
| [Mix](https://github.com/thismatters/EurorackMix/) | 1U 30hp | [V0](https://oshpark.com/shared_projects/xlEAsl8K) | Works well enough in its primary function as a mixer, but the LED display is not very good. A new iteration is in order. |
| [Slew](https://github.com/thismatters/EurorackSlew/) | 1U 12hp | [V0](https://oshpark.com/shared_projects/VN6XGUSn) | Works great! |
| [Sample Hold](https://github.com/thismatters/EurorackSampleHold/)  | 1U 13hp | [V0](https://oshpark.com/shared_projects/IxCpIOaM) | Works great! Needs standoffs to secure 3rd layer of PCB. |
| [Saw Animator](https://github.com/thismatters/EurorackSawAnimator/) | 1U 10hp | [V0](https://oshpark.com/shared_projects/MXBVaxpS) | Works, but there is a slight distortion of the output waveform that I would like to investigate. Needs standoffs to secure 3rd layer of PCB |
| [Clock Divider 1](https://github.com/thismatters/EurorackClockDiv/) | 1U 11hp | [V0](https://oshpark.com/shared_projects/ADWTtPJV) | Works great! Needs standoffs to secure 3rd layer of PCB |
| [Clock Divider 2](https://github.com/thismatters/EurorackClockDivTwo/) | 1U 10hp  | [V0a](https://oshpark.com/shared_projects/LyyWQIPF) | Requires a clean input clock signal, but otherwise works great. Needs standoffs to secure 3rd layer of PCB |
| [Balanced Modulator](https://github.com/thismatters/EurorackBalancedModulator) | 1U 12hp | [V0](https://oshpark.com/shared_projects/MmM817Fr) | Works Great! |
| [Turing Machine](https://github.com/thismatters/EurorackTuringMachine) | 10hp | V1a | Works great! (The V1a board hasn't been sent to manu yet, but the [V1](https://oshpark.com/shared_projects/wF94N3Eb) boards can be refit to the V1a design) |
| [Gate Delay](https://github.com/thismatters/EurorackGateDelay) | 1U 12hp | [V1](https://oshpark.com/shared_projects/XnestbOz) | Works great! (The V0 board (in the link) is the same as the V1 board... all that changed was 1 resistor value) |
| [Pulse Delay](https://github.com/thismatters/EurorackPulseDelay) | 1U 13hp | [V0](https://oshpark.com/shared_projects/BQrPkI6H) | Works great! |
| [Wavefolder](https://github.com/thismatters/EurorackWavefolder/) | 4hp | [V1](https://oshpark.com/shared_projects/R6z3tv0Q) | Works great, but the CV level knob is backward :( (accidentally labelled this as `v1` on the PCB even though it is the first release, oopsP) |
| [Pulses Expander](https://github.com/thismatters/EurorackPulses/) for Turing Machine | 6hp | [V0](https://oshpark.com/shared_projects/ie2On50L) | Works fine, but two of the jacks are mislabeled (12 and 24 are swapped) |
| [Volts Expander](https://github.com/thismatters/EurorackVolts/) for Turing Machine | 6hp | [V0](https://oshpark.com/shared_projects/RRs3dh0Z) | Works great! |
| [Kick Drum](https://github.com/thismatters/EurorackKickDrum/) | 6hp | ~[V0](https://oshpark.com/shared_projects/wLEqkfuk)~ | Has critical bugs: Scrape the trace between R15 and C5; The footprint for Q2 is `CBE` (the BC847 is actually `BEC`), you can still place the BC847 by rotating it about 120 degrees CCW (hacks for the win). The V1 board has both bugs corrected, but I haven't sent it to manu at this point. |
| [Snare Drum](https://github.com/thismatters/EurorackSnareDrum/) | 6hp | [V0](https://oshpark.com/shared_projects/vcqO2do3) | Works great! |
| [Mix (vertical)](https://github.com/thismatters/EurorackMix2/) | 6hp | [V0](https://oshpark.com/shared_projects/MPUfY34w) | Works great! |
| [Wet Mix](https://github.com/thismatters/EurorackWetMix/) | 1U 9hp | [V0](https://oshpark.com/shared_projects/SWKAWrO8) | Works great, but I want to do a second revision with built-in mults for A and B channels and an LED slider |
| [Add](https://github.com/thismatters/EurorackAdd/) | 1U 7hp | [V0](https://oshpark.com/shared_projects/97ymydub) | Works great! |


## In-Progress Modules

As the header implies, these modules are in varying degrees of readiness: Design, Manu(facturing the PCB), Assembly, and Validation. Once a module is validated then it will move up to the list above and it's repo will be added as a submodule here.

| Name         | Size | Current PCB | Notes                     |
|--------------|------|-------------|---------------------------|
| [High Hat]() | 6hp | ~[V0]()~ | Design |


## Assembly Process

You will need: an SMD hot-plate (ebay has these pretty cheap), a conventional soldering iron (fine tip is pretty nice to have), tweezers, solder, solder paste, isopropyl alcohol, and a soft bristle toothbrush.

- Order bill of materials from your vendors of choice. Do this first because it really sucks to get the PCB and not have the parts to populate on it! Mouser and Tayda Electronics are my go-to for 90% of components, but you may have local vendors that are sufficient.
- Order PCBs from OSHPark.
- Order solder stencil from OSHStencils (They don't let you share projects like OSHPark, so you're on your own for that!). They also sell solder paste and kits to help secure the board for paste application.
- Patiently await the 2 week manufacturing time from OSHPark.
- Seriously, you're still waiting.
- File the little nubs off the PCB once it arrives before starting assembly. If you're making one of the 1U modules and it is a triple-stacked PCB then you may notice that two of the three boards have SMD pads, in this case OSHPark will keep the two boards with SMD parts attached to each other; this makes SMD assembly much easier, don't separate these.
- Populate SMD
  - Set up solder paste stencil for applying solder paste. Generally this involves taping some "L" shaped acrylic to the desk to hold the PCB securely, then carefully register the stencil above the pads and tape it down securely in such a way that it can be released without losing registration to swap out boards.
  - Clean boards with isopropyl alcohol.
  - Apply paste to the boards. It's exactly like screen-printing if you've ever done that. Squeeze out some paste onto the stencil and use a squeegee (like a credit card or something) to force the paste through the stencil onto the board. The paste should exactly and fully cover all the SMD pads.
  - Put on some music and pretend to be a pick-and-put machine. Use tweezers to place SMD components on their pads. This is forever-taking, tedious work. However, it must be done in a timely fashion: Solder paste at room temperature will melt into an unaccountable liquid after some time as the flux separates from the solder. Move through this step with all deliberate speed, because you've only got about 75 minutes to get those boards onto your hot-plate.
- Cook the boards (temperatures here are appropriate for the Kester EP256 solder paste available from OSHStencils during checkout)
  - Pre-heat your hot plate to about 175C and let it come to temperature
  - Hold your populated board about an inch off the surface of the hot-plate for 30 seconds to gently bring its temperature up. This avoids too much thermal shock on the components and board.
  - Place the board onto the hot plate. Generally I'm doing three boards at a time, so after placing the first board I do the second and third in succession.
  - Allow the boards heat for 60 seconds. Components may start to drift on the board during this phase, keep a careful eye and use your tweezers to move things back in to place. Some heat proof gloves make this much safer.
  - Raise the temperature set-point of the hot plate to 255C.
  - Observe the boards as the temperature rises past 240C, you should see the the solder joints start to wet. Remain watchful for drifing components.
  - Reset the temperature on the hot-plate to 175C in order to prepare for future boards, then switch the hot-plate off.
  - Remove the boards following a similar process as placing them. Elevate them an inch or so off the hot-plate and let them cool slightly while still near the heat to avoid thermal shock. Set the boards aside to cool to room temperature.
- Use isopropyl alcohol and a soft-bristle toothbrush to clean the flux and solder residue from the boards. Don't skimp on this part of the process.
- Visually inspect the boards looking for any poor quality or incomplete solder joints, during this inspection further clean the boards of solder residue and balls of solder which may have cooled near components.
- Do any rework on SMD components
- Clean the boards again!
- Populate through-hole components (shortest to tallest) on the non-face boards. Some through-hole components may have a critical fit (especially on triple-stacked modules), so be sure everything is aligned nicely after soldering one pad, then solder the other pads. Crop the leads on through hole components close to the board
- Clean the boards again. Get rid of the flux before moving on.
- Install Faceplate
  - Loosely attach face components to the faceplate with their threaded connections.
  - Align all the pins on face components with their respective footprints.
  - Ensure that everything is well-aligned vertically before soldering. Switches may present challenges here, adjust their bottom-nut to suit.
  - Solder face components to their footprints.
  - Tighten face components to face (I like to use some [Rocket Sockets](https://lovemyswitches.com/rocket-sockets-pedal-building-socket-set/) to protect the lovely purple finish on the faceplates!)
- Adjust trimmers to achieve sonic perfection (Each repo will have instructions for trimming as needed).
  - So far all modules in this collection can be trimmed in using a single [Mordax Data](https://www.mordax.net/products/data) as a multi-channel oscilloscope and a VCO as a signal generator.
- Install and enjoy

## Lessons Learned

- Don't put vias on pads. The wet solder will disappear into the hole!
- Use good solder paste! The stuff from OSHStencils works great.
- Use new solder paste! Solder paste separates over time, don't expect a tube to last more than 6 months without noticable degradation in solder joint quality.
- Use high-concentration isopropyl alcohol and a soft toothbrush to clean your boards thoroughly at several stages in manufacture:
  - Prior to SMD soldering to remove fingerprints and residue from the boards,
  - After initial SMD soldering prior to visual inspection,
  - After through hole component soldering,
  - After faceplate components are soldered.
  - The flux from soldering, if left on the board, will oxidize into an unsightly crust after some months of using the module. I don't think this degrades the performance of the synth, but it does look really ugly, and makes handling the modules a little ikky. Moreover, a clean board is much easier to inspect.
- Inspect SMD soldering with the utmost scrutiny. It's pretty easy to get poor quality solder joints during reflow soldering (at least with my janky rig), so I like to use a microscope (or at least the magnifier app on my tablet) to inspect each joint. I use some little pokey tools to remove soldering residue that accumulates between the pins and little solder balls that collect near components. Doing a preliminary cleaning with isopropyl alcohol before inspection makes it a lot easier to see where rework may be needed. During inspection I note any joints which look poor. Subsequently, I use a soldering iron to remove the component, clean the pads with flux and solder braid, then re-solder the component. After the inspection I do another thorough cleaning putting extra focus on the places which weren't perfectly cleaned before. This inspection step is vital to getting good function from the modules; it is much more difficult to correct poor SMD soldering once the through-hole components have been populated on the board.
- Set aside proper time for building modules. Don't try to rush through building one of these! Enjoy the process.
- If you're unsure about a design, only assemble one module at first (not the lot of three) so that you can address any issues found with the first module while building the others (or scrap the boards).
- [OSHPark has a "medium run" offering](https://docs.oshpark.com/services/two-layer-medium-run/) which lets you order 10 boards for the price of 6 (2x regular run), but it takes a little longer to produce. It's a pretty good deal if you know you want a lot of one modules (you can never have enough VCAs!).
