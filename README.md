# Kimeera: Hybrid Tools for Human-Scale Speech Technology

Carnegie Mellon University's historical speech recognition engines
used a charming naming theme revolving around mythological beasts.
Unfortunately the last in the line, [CMU
Sphinx](https://cmusphinx.github.io/) has had its name largely usurped
by [a considerably more useful piece of
software](https://www.sphinx-doc.org/).  In addition, most of the
technologies in it have long since become quite obsolete.

On the other hand, I *like* CMU Sphinx.  Being written in good old
fashioned C, with old fashioned algorithms like MFCCs, GMMs, and
context-dependent triphones, it builds quickly, uses a fairly small
amount of memory and storage by 2022 standards, produces fairly small
models without passing through a costly distillation phase, runs
offline, and so forth.  We have much better options now, free ones
even, for full-on large-vocabulary continuous speech recognition, but
the barriers, both technical and financial, to entry for doing
something other than the small set of tasks for which pre-trained
models exist are, in my opinion, very high.

Many of the efforts to modernize CMU Sphinx seem to have floundered
due to the overwhelming complexity of the task and a severe lack of
resources compared to other academic groups, not to mention the GAFAMs
of this world.  But more fundamentally, researchers have no incentive
to do things that make for useful technology, such as:

- Reimplementing proven algorithms in a robust and user-friendly way
- Reusing existing implementations of these algorithms

It would be nice to take advantage of things that were Invented
Elsewhere.  Back in the bad old days when the only other openly
available system was HTK, which wasn't actually free, this was not an
option.  Nowadays we even have free *datasets!*

With that in mind, I've created this "project", which is more of a
personal playground than anything.  As mentioned above, *some LVCSR
tasks for some languages* are now well handled by free software
packages too numerous to name.  We can of course say the same thing
for text-to-speech, machine translation, information extraction,
information retrieval, and so on.  The main questions I want to
answer, then, are:

- Name these tasks!  What are the *actually useful* things I can do
  with speech and language technology?  And are these things *actually
  worth doing*?
- Name these packages!  What combination of free software exists that
  will allow a moderately experienced researcher like me to accomplish
  them?
- What is missing that would enable an average technologically
  literate person to put the pieces together to accomplish the tasks?
  (feel free to insert intermediate steps like "linguist", "CS
  undergrad", "web developer", etc)
  
In other words, this is intended to be a space for free,
*user-centered* and *application-driven* (rather than
technology-centered and data-driven) speech technologies, with a hard
focus on:

- Accessibility to people outside of academia and industry
- Equal treatment of all languages and dialects, or perhaps even an
  emphasis on minority and endangered languages
- Supporting language workers and language learners rather than trying
  (explicitly or implicitly) to replace them
- Interpretability of models and explainability of decisions
- Data sovereignty, privacy, freedom, avoiding social bias in models
- Documentation that tells you how to make things work and not just
  how they work

It is not another toolkit, because we have enough of those already.
It is my firm belief that most of the pieces needed to make
applications satisfying the goals listed above already exist, and the
large amount of research into transfer learning for "low-resource"
scenarios would seem to confirm this.  What is missing, in my opinion,
though I would like to be proven wrong, is the ability to use the
models, features, and algorithms that make sense without being locked
into, and I cringe every time I hear this word used in this context, a
particular "ecosystem", usually associated with a company that wants
to sell you something, or to sell *you* (or at least your data).

The recent trend in ASR (and machine learning in general) has been
towards "end-to-end" models, because supervised learning has been
solved since 2015, or so I'm told - meaning, given an ever-expanding
amount of computing power, with ever-increasing amounts of data and
brute-force techniques for augmenting it, the word error rate can
ultimately be abolished, at least for LibriSpeech and maybe a few
other datasets in a few other languages.  That's great, but what gets
lost along the way is, well, exactly the things I listed previously.

Perhaps that's okay.  We'll soon be eight billion content creators
(not all of us were given the choice) and more content is on the way
every microsecond.  Perhaps quantum computing, or some other future
breakthrough, will allow us to break through the current limits of
computing capacity.  Perhaps all the silicon and copper that was
wasted on cryptocurrency "mining" can be recycled or at least
repurposed for something useful.  Perhaps we'll all end up speaking
"Anglic", even the dolphins and chimpanzees, and none of this will
matter anymore.

Perhaps.

In the meantime, I will be creating some chimeras in the biological
and mythological sense, hybrid (in French I would say *bâtards*)
models and systems, bolting together bits and bobs to make some
hopefully useful things, and documenting them.  Things that should not
work, but which do.  And you can too!

Since the name [Chimera](https://www.cgl.ucsf.edu/chimera/) is already
taken, and since a theme of Leena Krohn fandom has already been
established with
[SoundSwallower](https://github.com/ReadAlongs/SoundSwallower), I've
used ... a slightly different spelling ... from the original title of
the chapter "The Son of the Chimera" ([Kimeeran
poika](http://www.kaapeli.fi/krohn/pereat/hakanin_suku.htm)) in
*Pereat Mundus: A Sort of Novel*.

I hope that its life will be short, but I cannot find anything like it.

David Huggins-Daines <dhdaines@gmail.com>
