# wifi-strength

A simple-command line program for Max OS X to print out your Wi-Fi's signal-to-noise ratio (SNR).

I wrote this for fun years ago.  It's not mean to be complete or robust.

## Installation

Copy the `wifi-strength` script to a directory in your `$PATH`.  I use `~/bin`, but make sure `~/bin` is in your `$PATH`.

## Usage

Assuming the `wifi-strength` command is in your `$PATH`, just run it like so:

```console
jesse@peirce ~ $ wifi-strength
50
jesse@peirce ~ $
```

## Mapping Wi-Fi Strength

OS X comes with a `say` command that will use a speech synthesizer to say out loud whatever string is passed to it.  Consider running the following on your laptop as your walk around your home/apartment:

```text
watch -n1 'wifi-strength | say'
```

This will vocalize your SNR every second, even as you move around.

Conversely, put your computer in a fixed location, run the above command, and then go move your router around to find a place with high SNR.
