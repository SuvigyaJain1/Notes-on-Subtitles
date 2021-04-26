# Brief Notes on Various Captioning & Subtitle Standards - By Suvigya Jain

*Disclaimer: none of this is my own work and is mostly paraphrasing of content I have found from tons of webpages and books online. It is merely intended to help people find general information about the topic in one place. I am by no means an authority or claiming that any of this is accurate. Feel free to mail me at suvigyajain1@gmail.com for correction or feedback*

## What are subtitles ?
**Subtitles** are the text you probably have seen on your screens (TV, mobiles, etc) which display the dialgoue on screen or other information related to the video content being played. They were originally created to help those hard of hearing but have also found use in making content accessible to more people across language barriers and just as a means to add translations. **Closed captioning** is the American term for closed subtitles specifically intended for people who are deaf or hard-of-hearing. They consist of non-dialogue audio as well . 
[from Wikipedia](https://en.wikipedia.org/wiki/Subtitles)

These subtitles, subs for short can be pre-rendered with the video (**in-band**), or be separately(**out-of-band**) transmitted in one of these mediums:
- Graphic (tiff, bmp, png for example) 
- Text

The separate ones have the obvious advantage of being hidden until the user explicitly turns them on, as well as easy editing. But they also additionaly require 'markers' to give information about where to place the subtitles in the video. These markers are typically timecodes although they can be length of the film as well for movies stored on reels.

## Major Types
There are 3 major types of caption formats:
[from w3_docs](https://www.w3.org/AudioVideo/TT/docs/TTML-Profiles.html)

- Captions for Analog TV:
    - **CEA-608:** Primary in-band format in the US for analog NTSC(National Television System Committee) transmissions.
            It continues to be used in digital format through "608 over 708". Characters based.
    - **Teletext**: It is mainly used in Europe. Character based. Used in digital TV and online video via DVB Teletext
    - **EBU-STL**: legacy, out of band caption file format.
- Captions for Digital TV:
    - **CEA-708**: Primary format for in-band in the US. Native 708 is character based, but for online transmission it is embedded in the MPEG-2 TS stream
    - **DVB Teletext**: (ETSI 301 775) mainly used in Europe. Embeds teletext into DVB MPEG-2 TS stream
    - **DVB Subtitles**: mainly used in Europe. Allows either image or character based captions to be embedded in DVB MPEG-2 TS stream.
- Online **Captions Format**:
    - **TTML**: is an Authoring, Interchange and Distribution format. More advanced and complex
    - **WebVTT**: Distribution format. Integrates well with HTML5. Used in browsers and native players.
    - **608**: US alternative implemented in native players (Android and iOS)

## TTML
It stands for Timed Text Markup Language. It can be used for interchange or simply to distribute captions or subtitles. It is a superset that supports most of the closed captions files. It uses XML, SMIL, XSL-FO, and CSS for presentation and layout of the text. It also went by the name of DXFP

### Various elements are used by TTML :
* HTML like content elements contain the caption text. Ex: < p>, < span>, < div>, etc 
* Timing attributes define when the caption should appear on screen
* Style elements describe style attributes
* Layout elements
* Animation elements
* Metadata

### TTML profiles
* [TTML1](http://www.w3.org/TR/ttml1/)
* [SDP-US](http://www.w3.org/TR/2013/NOTE-ttml10-sdp-us-20130205/)
* [IMSC1](http://www.w3.org/TR/ttml-imsc1/)
* [SMPE-TT](https://www.smpte.org/standards)
* [EBU-TT](https://tech.ebu.ch/ebu-tt)
* [CFF-TT](http://www.uvcentral.com/sites/default/files/files/PublicSpecs/cff-tt-1_1.zip)

