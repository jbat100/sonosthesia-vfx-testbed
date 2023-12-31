# sonosthesia-unity-demo-deform

Testbed for realtime VFX control using various Sonosthesia [signals](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.signal) and [channels](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.channel). This project uses the following [Sonosthesia dependencies](https://github.com/jbat100/sonosthesia-unity-packages):

- [com.sonosthesia.processing](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.processing)
- [com.sonosthesia.signal](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.signal)
- [com.sonosthesia.flow](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.flow)
- [com.sonosthesia.channel](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.channel)
- [com.sonosthesia.target](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.target)
- [com.sonosthesia.mapping](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.mapping)
- [com.sonosthesia.audio](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.audio)

Audio for these demo scenes was obtained from [epidemicsound](https://www.epidemicsound.com/), namely [jonquilla](https://www.epidemicsound.com/track/s8nGwyBhLq/). 

## Scenes

NOTE : on the first Unity editor play the audio and the graphics are out of sync, due to Unity generating runtime support files. This issue solves itself on second playback. 

### Sketch191003TriEmission

This scene extends a VFX [sketch](https://github.com/keijiro/VfxGraphTestbed/tree/master/Assets/Sketch191003) by Keijiro, adding multiple emissive sources, exposing additional parameters and connecting them to spectral energy band signals.

<p align="center">
  <img src="https://github.com/jbat100/sonosthesia-vfx-testbed/assets/1318918/d01dbd3f-fd3b-42e6-be02-9fb34ab67329" />
</p>

## Realtime control

### Audio in Unity Timeline

A Unity [timeline](https://docs.unity3d.com/Packages/com.unity.timeline@1.8/manual/index.html) is used to play audio files through audio sources. The energy in different spectral bins is [extracted]([com.sonosthesia.audio](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.audio)) and fed into [signals](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.signal) which are [mapped](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.mapping) to [targets](https://github.com/jbat100/sonosthesia-unity-packages/tree/main/packages/com.sonosthesia.target) controlling exposed VFX properties.

## License

MIT License applies to Sonosthesia packages. VFX graphs used, modified and extended from external sources inherit the license of their original authors.
