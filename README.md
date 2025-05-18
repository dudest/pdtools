# Pure Data Tools

A collection of usefull PD abstractions.

## Usage

In PD preferences, include the collection folder to your *path*.

*Help* files with examples are included.

## List of available abstractions

### Utility

- `pdt.master~` - Stereo audio out to DAC. Integrated mute and record to stereo *.wav* file.
- `pdt.master5.1~` - 6-channel audio out to DAC. Integrated mute and record to 6-channel *.wav* file.
- `pdt.pan~` - Mono to stereo pan
- `pdt.pan2~` - Stereo pannng
- `pdt.xfade~` - Crossfade between two audio rate signals.
- `pdt.ezplay~` - Load a sound file and play it.

### Sequencing

- `pdt.noteseq` - Provides a very basic piano roll editor. Saves and load sequence from text file.
- `pdt.transport` - Transport controls for `pdt.noteseq`.

### Granular synthesis

- `pdt.rtgranular~` - Stereo granular synthesizer for realtime input. Grains are dispersed between left and right channels.
- `pdt.rtgranular5~` - 5-channel granular synthesizer for realtime input. Grains are dispersed across 5 channels.
- `pdt.granular~` - Stereo granular sythesizer for processing sound files. Expects a mono *.wav* file. Grains are evenly dispersed between left and right channels
- `pdt.granular5~` - 5-channel granular sythesizer for processing sound files. Expects a mono *.wav* file. Grains are evenly dispersed across 5 channels.
- `pdt.grainstretch~` - An audio file looper that includes a time streching facility. Rather than slowing or speeding up playback, stretching algorithm adds or removes frames so that the original pitch is maintained.

### Audio effects

- `pdt.delay~` - A rudementary delay object with inputs for *delay time*, *hi pass fequency*, *feedback*, and *mix*.

### Conversion

- `pdt.bpm2ms` - Converts bpm to milliseconds. Useful in concunction with `metro`.
- `pdt.deg2rad` - Converts degrees to radians.
- `pdt.rad2deg` - Converts radians to degrees.

### Logic

- `pdt.counter` - Simple counter. Has arguments for *increment* and *target*
- `pdt.cointoss` - random *true* / *false* with probability arguement.
