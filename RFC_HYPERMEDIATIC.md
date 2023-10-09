%%%
Title = "hypermediatic"
area = "Internet"
workgroup = "Internet"

[seriesInfo]
name = "hypermediatic"
value = "draft-hypermediatic-leonvankammen-00"
stream = "IETF"
status = "informational"

date = 2022-08-01 

[[author]]
initials="L.R."
surname="van Kammen"
fullname="L.R. van Kammen"

%%%

<!-- for annotated version see: https://raw.githubusercontent.com/ietf-tools/rfcxml-templates-and-schemas/main/draft-rfcxml-general-template-annotated-00.xml -->

.# Abstract

**hypermediatic** browsers, are browsers which allow hypermedia navigation by treating ALL fileformats (with outbound/embedded links) equally as first-class citizens by default, rather than getting served through hyperscripted single-layer like HTML.
A hypermediatic browser <b>MEDIATES</b> in hyperconnecting URIs/URLs, by treating HTML as **JUST** a fileformat, rather then **THE** doorway to hypermedia.

<img src="droste.jpg" style="max-width:600px"/>

{mainmatter}

# Redefining the hypermedia experience 

Traditionally, hypermedia experiences seem to be explained like this: hypermedia (images/sound/video) is 'carried' by hypertext (HTML):

**The carrier is HTML, the modulator is hypermedia.**

However, these days, a more appropriate way of looking at things is this:

**The carrier IS the URL, the modulators ARE hypermedia (URLs)**

> HTML brought us a lot, but it also is becoming a bottleneck for highperformance hypermedia experiences, pushing developers towards publishing native non-hyperconnected apps into appstores.

If we want the web to be inclusive for spatial computing and other future formats (gaming e.g.), we must stop looking at it like a web of textdocuments with bells and whistles.

# Criteria for a hypermediatic browser or fileformats

1. when possible, convert filenames in documents ('see foo.pdf') to navigatable hyperlinks when they exist in the current filesystem/directory.
2. if online: scan for words containing `://` or multiple dots and a slash, and present them as navigatable hyperlinks
3. (any) fileformats with outbound/embedded links are the focus (not only HTML)
4. toplevel URLs with an unknown file-extension or mimetype should trigger the fileformat store 
5. Outbound links are supported (like `href` in HTML)
6. Embedded links are supported (like `src` in HTML)
7. Tagging/Classifying nodes or items is supported (like `class` in HTML)
8. Naming nodes or items is supported (like `id` in HTML, or object names in glTF)
9. Positioning the user in 2D/3D is supported (like a spawn-point in games, or URI Fragment-jump-to-page-position in HTML)

> Subsets are encouraged too (hypermediatic is a spectrum). For example 1 & 2 are nice usecases for terminal/ereaders.

## Native top-level URL browsin

1. if an extension or mimetype is unknown
1. search the fileformat store for supported fileformatviewers (and offer installation)
1. search the browser extension store for fileformat-related support (and offer installation)


# Hypermediatic hypermedia vs shallow webbrowsers 

The following feature-stack timeline has introduced lots of good, but also introduced hyperscripted unhyperified websites, causing trending technologies like [htmx.org](https://htmx.org) and native appstores:

1. Hypertext format (HTML)
2. Embedded Hypermedia in HTML 
3. 1995: Javascript in HTML 
4. 1999: Browser extensions (store)

One could argue that at some point the webbrowser was THE disrupting appstore, by hyperconnecting data itself.<br>
In retrospect, a more hypermediatic browser however, could perhaps be achieved along these lines:

1. support popular fileformats containing outbound/embedded links
2. filetype extensions (store) to support viewing fileformats with native highperformance 
3. browser extensions (store) only place to allow logic/scripting (javascript e.g.)

# Benefits 

1. non-HTML fileformats are treated as first-class hypermedia too, fostering latest hardware-to-software hypermedia experiences.
2. filetype organisations can publish highperformance extensions to the filetype store.
3. unrecognized fileformats can automatically consult the filetype and/or browser extension-store, and trigger an installation CTA
4. closing the gap between native highperformance games/spatial computing and the (lower performing security-sandboxed) webbrowser
5. preventing the security/privacy traps of hyperscripted HTML, by pushing/allowing logic-layer (javascript e.g.) only in browser-extension space

# Hypermediatic as a selfmodulating synthesizer

Lets take this hypermediatic slogan:

**The carrier IS the URL, the modulators ARE hypermedia (URLs)**

Why does it say URLs in brackets?<br>
Well the observation is actually that URLs modulate URLs too.<br> 
An example is a share-button as a hypermediatic phenomenon: in most cases it shares an URL to another URL.<br>
When the enduser presses the share-button, an URL (usually on the backend) is requesting by sending the shared URL along.<br>
In other words: the URL is the carrier of another URL.<br>

> Therefore, thru the lens of McLuhan the following applies: "The URL IS the message"

# Questioning the conservative interpretation of hypermedia

Let us focus on the spirit of the following ideas, rather than getting caught up in the forthcoming conflation of 'hyper' terms.<br>
The reframing of hypermedia towards hypermediatic raises several questions that challenge current hypermedia:<br>

1. Until which point is HTML holding back highperformant hypermedia-surfing of images/sound/video/3D?
1. Why are webbrowsers poorly supporting other fileformats using URLs? And does the individual decide which fileformats are (not) deferred to the (browser-extension) backseat?
1. Why are hypermedia fileformats not encouraged to support the outbound/embedded hyperlink-paradigm like HTML?
1. Why are operating systems not supporting/encouraging outbound/embedded links in fileformats out of the box? (liquid information/hyperwords e.g.)

A lot of it, can perhaps be explained by the **hypertext-first-hypermedia-later vision** which most webbrowsers and operating systems seem to share.<br>
From an historical perspective this makes sense (it was easier to project text than images back in the days).<br>
However, it also means that whatever fileformat is consumed in the webbrowser, gets served through this lens (through HTML) or indirectly via browser extensions.<br>

# Contact

* leonvankammen|gmail.com

# IANA Considerations

This document has no IANA actions.

# Acknowledgments

TODO acknowledge.
