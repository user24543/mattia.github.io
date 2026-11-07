# mattia

**developer & digital artist.**

a personal site and a series of interactive studies about brains, senses and living things.
every study is a single html file with its own simulation running live in the browser:
no frameworks, no build step, nothing pre-rendered.

## the studies

| | study | what you can do |
| --- | --- | --- |
| 01 | [glitch](glitch.html) | a glitch-art piece with shaders and generated sound |
| 02 | [gradient](gradient.html) | walk a chrome loss landscape and watch a neural network train live |
| 03 | [wetware](wetware.html) | explore a 3d brain built from a real mri scan, a spiking neuron and a network you teach by touch |
| 04 | [umwelt](umwelt.html) | see one garden at dusk as a human, a honeybee, a bat, a pit viper, a dog and a tick |
| 05 | [302](302.html) | poke the whole nervous system of *c. elegans*, all 302 neurons on their real wiring |
| 06 | [insular](insular.html) | set an island and watch mice grow and elephants shrink (foster's rule) |
| 07 | [circa](circa.html) | jet-lag a body clock, put it on night shifts or send it into a cave |
| 08 | [hypnos](hypnos.html) | follow a sleep recording through a whole night, from brainwaves to binaural beats |

## built with

- **webgl and glsl** for the 3d scenes, with [three.js](https://threejs.org) r149 on some pages
- **canvas 2d** for the charts, recordings and simulations
- **web audio** for every sound, all generated in code (there are no audio files)
- **[syne](https://fonts.google.com/specimen/Syne)** and **[fragment mono](https://fonts.google.com/specimen/Fragment+Mono)** from google fonts

## run it locally

open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
```

then visit `http://localhost:8000`. fonts and three.js load from the web, so an internet connection is needed.

## files

```
index.html       the main page
glitch.html      01
gradient.html    02
wetware.html     03 · includes the compressed brain model
umwelt.html      04
302.html         05 · includes the worm's wiring data
insular.html     06
circa.html       07
hypnos.html      08
.nojekyll        tells github pages to serve the files as they are
```

## data and credits

- **wetware**: brain meshes from [brain for blender](https://brainder.org/brain-for-blender) by anderson m. winkler,
  [cc by-sa 3.0](https://creativecommons.org/licenses/by-sa/3.0/). the simplified brain model embedded in
  `wetware.html` is shared under the same licence.
- **302**: neuron positions and wiring packaged by [openworm](https://openworm.org)
  ([c302](https://github.com/openworm/c302) and the
  [connectome toolbox](https://github.com/openworm/ConnectomeToolbox), mit licence); wiring from cook et al.,
  *nature*, 2019.
- the science on every page is simplified from published research, and each page says where its models are
  teaching versions rather than real data.

© 2026 mattia
