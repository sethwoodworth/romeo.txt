-----------
Annotations
-----------

In a few different annotations projects, there is an ongoing conversation about efficient coordinate systems for annotations of text.
Take the line: "wherefor art thou Romeo".
An annotation of this line might explain the use of the word 'wherefor'.
The problem is that there isn't a canonical linenumber or pagenumber that can be used to line up this annotation to the source document.
For things like Aristotle, there are agreed upon line numbers, but for modern texts, say *Ulysses*, there is no cannon.


My current thought is: "why must annotation coordinates be efficient?".
Taking an aribitrary copy of *Romeo and Juliet* and a set of arbitrarily sourced annotations, aligning the two could happen by finding the annotation's 'sourcetext' field.
This would be innefficient, but for a given pair of text and annotations, they could be aligned once on a server, and rendered into more efficient html for the client.
Further, this suggests three alignment placeholders:

    * Local xpath/css-selector for the current html
    * canonical line number system from academic or traditional sources (act V, scene ii, line 32)
    * full resource matching (annotation would contain source text "Wherefor art thou Romeo"
