NOTE: BELOW IS THE ORIGINAL README FROM THE ORIGINAL REPO FOR PYSYNTH BY MDOEGE. I WILL BE PLAYING WITH IT AND IT WILL EVENTUALLY BECOME ITS OWN SEPARATE, YET RELATED, PROJECT. FOR NOW, NOTHING HAS BEEN CHANGED, AND SO IT IS A SIMPLE FORK. ALL THE USUAL RULES APPLY, IT'S JUST THAT IN A FEW MONTHS IT MIGHT LOOK NOTHING LIKE THIS. FOR THOSE WHO DID NOT KNOW, THE ORIGINAL SOFTWARE WAS PROVIDED UNDER A [GPL LICENSE] (http://www.gnu.org/copyleft/gpl.html), i.e.

"The GPL is a copyleft license, which means that derived works can only be distributed under the same license terms."

UNTIL FURTHER NOTICE, THIS IS A MERE FORK OF THE ORIGINAL REPO, BUT EVENTUALLY IT HOPES TO BE A DERIVED WORK. I HAVE RENAMED IT PyTonnetz AS A TEMPORARY DUMMY TITLE. -antiface

## Overview

PySynth is a simple music synthesizer written in Python. The goal is not to produce many different sounds, but to have scripts that can turn ABC notation into a WAV file without too much tinkering.

There are three variants: **PySynth A** is faster, only depends on Python 2, and sounds like a cross between a flute and organ. **PySynth B** is more complex in sound and needs [NumPy][2]. It's supposed to be a little closer to a piano. Finally, **PySynth S** is more comparable to a guitar, banjo, or harpsichord, depending on note length and pitch.

The current release of the synthesizer can only play one note at a time. (Although successive notes can overlap in PySynth B and S, but not A.) However, two output files can be mixed together to get stereo sound.

## Sample usage

Read ABC file and output WAV:

    python read_abc.py straw.abc

As a module from the Python interpreter:

    from pysynth_b import *
    make_wav(song, fn = "danube.wav", leg_stac = .7, bpm = 180)

## Site

More documentation and examples at the [PySynth homepage][1].

[1]: http://home.arcor.de/mdoege/pysynth/
[2]: http://numpy.scipy.org/
