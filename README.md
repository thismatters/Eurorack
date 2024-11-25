# Thismatters' Eurorack Modules

This is a project to track the progress in replicating and updating modules originally published by [Yusynth](https://yusynth.net/Modular/modular.html). You must check out his site before going any further, he has so much information published there which is omitted from this collection of repositories. I'm just a hobbyist and a fan of his exemplary work. As he states on his site:

> All circuits, schematics, printed circuit board, panel design and associated data published on this site can be used for private use only.

No mass-producing these modules! Friends and family only!

This is a collection of submodules, each of which is itself a Eurorack format module produced in [KiCAD](https://www.kicad.org/) (an open source circuit design suite). These modules are 3U and 1U sized. The 1U modules adhere to the [Intellijel Technical Specifications](https://intellijel.com/support/1u-technical-specifications/).

Each of the modules below has had at least one prototype manufacturing run and has been installed in my synth cabinet. Some of them require some amount of hacking to be made functional. If that is the case a warning will appear in the notes. Each repo will have a "tag" for each version that has been sent out for a prototype run.

You may find some other Eurorack modules among my repositories which are **not** in this collection. These have not been sent to OSHPark for prototyping or have not been fully assembled and validated. Once they are validated I will add the repo here.

## Repositories

| Name         | Size | Current PCB | Notes                     |
|--------------|------|-------------|---------------------------|
| [VCO](https://github.com/thismatters/EurorackVco/) | 12hp | [V1](https://oshpark.com/shared_projects/N1VjtYdp) | Works well, though there can be some inconsistency with trimming. |
| [VCA](https://github.com/thismatters/EurorackVca/) | 6hp  | [V1](https://oshpark.com/shared_projects/VmwAFYtq) | Works fine! |
| [ADSR](https://github.com/thismatters/EurorackAdsr/) | 6hp  | [V2](https://oshpark.com/shared_projects/UEztaF3P) | Works great! |
| [LFO](https://github.com/thismatters/EurorackLfo/) | 6hp  | [V0](https://oshpark.com/shared_projects/wfHu28zj) | Really hard to dial in / Doesn't quite work right |
| [Moog VCF](https://github.com/thismatters/EurorackVcf/) | 8hp  | [V0](https://oshpark.com/shared_projects/SO7swty4) | I'm pretty happy with this, but there is some room for improvement. I want to do another iteration someday. |
| [Mult](https://github.com/thismatters/EurorackMult) | 1U 11hp | [V0](https://oshpark.com/shared_projects/0YTEwnCD) | This circuit is broken, needs a new iteration. Technically it can be hacked to make functional, but it isn't good. Don't recommend ordering that PCB. |
| [Mix](https://github.com/thismatters/EurorackMix/) | 1U 30hp | [V0](https://oshpark.com/shared_projects/xlEAsl8K) | Works well enough in its primary function as a mixer, but the LED display is not very good. A new iteration is in order. |
| [Slew](https://github.com/thismatters/EurorackSlew/) | 1U 12hp | [V0](https://oshpark.com/shared_projects/VN6XGUSn) | Works great! |
| [Sample Hold](https://github.com/thismatters/EurorackSampleHold/)  | 1U 13hp | [V0](https://oshpark.com/shared_projects/IxCpIOaM) | Works great! |
|--------------|------|-------------|---------------------------|

All of the aforementioned repositories use this [library of KiCAD symbols and footprints](https://github.com/thismatters/EurorackKiCAD).
