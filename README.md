# midimonitor
Midimonitor displays incoming MIDI messages in a web-browser using the WebMIDI API.

MIDI is a communication standard describing how musical instruments can communicate with computers, other musical instruments, or other hardware. 

Midimonitor is a single page and single file web application with no external dependencies (well, it downloads a free font from Google, but will work just fine without it).

This is the first web application I created using the WebMIDI API, so it's been my way of learning this API.

## Tips and tricks
If you're working with MIDI software development (WebMIDI or native applications), running a MIDI loopback adapter together with this midimonitor is really useful for debugging / monitoring the MIDI messages you send. On Windows, I recommend https://www.tobias-erichsen.de/software/loopmidi.html.

A good native Windows application for monitoring MIDI messages is MIDI-OX - http://www.midiox.com.

## Todo
- [ ] Display CC type (rename note column to misc, move to the right, use for CC), from https://www.midi.org/specifications-old/item/table-3-control-change-messages-data-bytes-2
- [ ] Display NRPN-messages (in the new misc column, only for the last CC value, perhaps)
- [ ] Enable message filters (checkboxes)
- [ ] Display MIDI activity as colored circle
- [ ] Support MIDI tempo
- [ ] Support System Real-Time and System Common messages
- [ ] Support lots of midi inputs and outputs without cluttering the display, e.g. by letting user collapse list, and/or make a more compact list / grid
- [ ] Create node.js-version, using https://jazz-soft.net/doc/JZZ/webmidi.html

## Misc useful links
- https://webaudio.github.io/web-midi-api/  
- https://www.w3.org/TR/webmidi/ 
- https://css-tricks.com/dip-your-toes-into-hardware-with-webmidi/ 
- https://webmidi-examples.glitch.me  
- https://www.midi.org/specifications/item/table-1-summary-of-midi-message 
