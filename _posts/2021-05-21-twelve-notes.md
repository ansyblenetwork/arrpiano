---
title: "The twelve notes of music"
---

Today's quote of the day comes from Richard Feynman:

<div class="media">
<p>All the kids were playing in the field and one kid said to me, “See that bird, what kind of a bird is that?” And I said, “I haven’t the slightest idea what kind of a bird it is.” He says, “It’s a brown-throated thrush,” or something, “Your father doesn’t tell you anything.”</p>

<p>But it was the opposite: my father had taught me. Looking at a bird he says, “Do you know what that bird is? It’s a brown-throated thrush; but in Portuguese it’s a Bom da Peida. In Italian a Chutto Lapittida.” He says “In Chinese it’s a Chung-long-tah, in Japanese a Katano Tekeda,” etcetera. “Now,” he says, “you can know in all the languages you want to know what the name of that bird is and when you’ve finished with all that,” he says, “you’ll know absolutely nothing whatever about the bird. You’ll only know about humans in different places and what they call the bird.</p>

<p>“Now,” he says, “let’s look at the bird.”</p>

</div>

So let's look at the notes of music. Why are there twelve notes in Western and modern music?



In the spirit of my [recent commentary]({% post_url 2021-05-19-music-and-mathematics %}) on taking a systematic approach, we first observe that this question can be decomposed into two:

1. Why are there not more than twelve notes?
2. Why are there not fewer than twelve notes?

The short answer to the first question is that _consonances_ are distinguished and rare. This is already somewhat evident within the twelve notes: Slamming the keys on a piano is more likely than not to produce some dissonant sounds. Having fewer notes helps control the dissonances. Blowing arbitrarily into say, a harmonica, typically doesn't sound so unpleasant, because there are fewer "open notes."

The answer to the second question is, I think, more subtle. My short answer would be that it is related to _symmetry_. By a quirk of the arithmetic involved with consonance, having only say, two or some other small number of consonant notes yields an asymmetric and scattered arsenal of pitches. In fact, insisting on a truly symmetric set of consonant notes is untenable: It would require the set to have infinitely many notes (or just one). 

We will see that by imposing some reasonable compromises, we find ourselves with twelve notes.

### Consonance

Humans distinguish different sound frequencies through pitches, with higher frequencies corresponding to higher pitches. Conventional musical wisdom says that simpler ratios of frequencies correspond to more consonant intervals of pitches. There is some ambiguity as to what "simple" means in this context, and in fact there is some subjective disagreement as to which intervals are more consonant than others.

However, it turns out that for the purpose of constructing the twelve notes, we needn't worry about subtle gradations of consonance yet. There is essentially universal agreement that intervals corresponding to frequency doubling and tripling (or alternatively, halving and trisecting) are the most consonant. In fact, doubling a frequency corresponds to raising by an octave, while tripling a frequency corresponds to raising by a perfect fifth. We will see that using these ratios already suffices to justify using twelve notes. 

### Symmetry

Music consists of a sequence of notes. Due to _octave equivalence_, it would not be very interesting to restrict ourselves to only octaves. But it also wouldn't be very interesting to restrict ourselves to adding just the one note that forms a perfect fifth with our starting note. This is because the new note too would like the option of having somewhere to go - preferably to another consonant but interesting relative perfect fifth. But we see that taking powers of three will never yield a power of two, so this cycle of taking perfect fifths will never bring us to an octave equivalent of our starting note.

The resolution to this is essentially to stop this _circle of fifths_ when the spread of our notes (and their octave equivalents) has become sufficiently even. It turns out that this happens after generating twelve notes, because 3^12 = 531441 is approximately 2^19 = 524288. The human ear is only barely refined enough to detect the difference between the ratio of these two numbers and 1. Furthermore, the approximation can be made almost imperceptible after applying an appropriate _temperament_, which we discuss next.

### Temperament

One can imagine constructing the keys of a piano by cycling through the fifths as described until all twelve notes have been generated, and then completing the rest of the piano by simply extending by octaves. For instance, starting with C, we would end with F.

Almost every fifth on the piano would be exact and beautiful. However, the perfect fifth extending from F to C would not have been constructed manually, but instead rely on the approximation discussed above. (Other consonances which we have not discussed - notably the important major third corresponding to a 5/4 frequency ratio - would also suffer.) This approach is known as _Pythagorean tuning_.

When musicians and composers started frequently employing modulation (and I suspect as pitch-inflexiable keyboard instruments grew more popular), _equal temperament_ was introduced. This approach evenly shares the approximation error across all twelve notes, making it almost imperceptible.
