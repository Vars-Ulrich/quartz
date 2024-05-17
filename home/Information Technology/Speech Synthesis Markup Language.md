---
aliases:
  - SSML
---
Speech Synthesis Markup Language. It's an [[XML]]-based [[Markup Language|markup language]] used to control aspects of synthetic speech generation, such as voice, volume, rate, pitch, and pronunciation. Developers use SSML to enhance the spoken output of [[Text-To-Speech|text-to-speech (TTS)]] systems by specifying how the text should be articulated. This can be particularly useful in applications like [[Virtual Assistants|virtual assistants]], accessibility tools, and any other systems that convert text into spoken audio.

For example, you can use SSML to make a virtual assistant emphasize certain words, pause for effect, or change the pitch or speed of the speech to sound more natural or to convey different emotions. Here’s a simple example of how SSML might look to alter the way a sentence is spoken:

```xml
<speak> Hello, <break time="500ms"/> this is an example of <emphasis level="strong">SSML</emphasis>. </speak>
```

