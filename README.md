# Spatializer++
Spatializer++ aims to increase Beat Saber immersion by allowing charters to put Dolby Atmos files into their charts in a fully vanilla-compatible manner!

## How does it work?
> [!NOTE]  
> **This mod is not Atmos, in the traditional "object-based" context.** Dolby does not disclose information on how the Joint Object Coding (JOC) system behind Atmos works.
> Luckily for us, though, all Atmos tracks have a backwards compatible Dolby Digital Plus 5.1/7.1 mix encoded in the same file. This is the audio data we actually use.
>
> While it may lack in some aspects, **it is still Atmos**, and you will hear things moving around you in charts that take advantage of Atmos capabilities, so, give it a go!

When a charter is creating a chart, they can opt to put an E-AC-3 encoded Atmos file in their chart directory alongside the default `.wav` or `.ogg`. This file is what powers the mod.

The mod detects these files and does a series of things:
- The mod will parse the file and separate the major channels (front left, front right, center, surround left and surround right). This is used for the general spatialization.
- It will also synthesise an LFE ("subwoofer") channel based on the data from the front channels. This is used for the Bass Boost toggle.
- When you play the chart, it will override the default sound system with the 5.1 data it processed, and you're in for an extremely immersive experience!

## For Chart Creators
> [!IMPORTANT]  
> **DO NOT OMIT INCLUDING A VALID `.wav` OR `.ogg` FILE WITH YOUR CHART.**
>
> Vanilla Beat Saber **CANNOT** read `.m4a` or `.eac3` files, so omitting one will render your chart **UNPLAYABLE** on any Beat Saber version without this mod.

To make your chart Atmos-supported, simply put an E-AC-3 encoded file in either `.m4a` or `.eac3` format in your chart directory, with the same name as your `.wav` or `.ogg` file.

## Where do I get Atmos mixes?
> [!CAUTION]
> **Ripping Atmos mixes from streaming services may be against the service's Terms of Service, or even illegal in some jurisdictions!**
>
> Please exercise caution when doing any of the things listed here, as you are doing so **at your own risk!**

**There's currently not many legal places to get Atmos mixes at the moment**... BUT if you're willing to get your hands dirty, then you can certainly rip Atmos mixes from your streaming service of choice! Listed are a few repositories for Atmos-capable streaming services, that allow downloading of Atmos streams.

- **Apple Music:** https://github.com/zhaarey/apple-music-downloader
- **TIDAL [UNTESTED]:** https://github.com/Dniel97/orpheusdl-tidal

...more will be added when discovered.
