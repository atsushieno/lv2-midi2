# what is lv2-midi2?

It is an experimental attempt to extend LV2 to add support for MIDI 2.0,
which would look like [existing MIDI 1.0 support](https://lv2plug.in/ns/ext/midi) through Atom.

There is not of much implementation within this extension feature itself.
It resembles how the existing MIDI 1.0 support is done.
In LV2, most of the existing work (packet processing) is done through LV2 Atom API.

## implementing MIDI 2.0 support

So far I use my cmidi2 library (which is also experimental UMP processing library). Note that lv2-midi2 extension does not depend on it. It only specifies the URI and implementors should be free to choose any library behind.

(I'm doing this mostly to have MIDI 2.0 as the MIDI support core in [android-audio-plugin-framework](https://github.com/atsushieno/android-audio-plugin-framework/) and [aap-lv2](https://github.com/atsushieno/aap-lv2).)


