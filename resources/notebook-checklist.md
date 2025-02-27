# Notebook Checklist & Guide

In this class, it is not enough to create a notebook that contains code to compute correct results.
You also need to ensure that your notebooks are well-structured documents that communicate your work
and findings.

## Standalone Documents

As I discuss in {video}`week3:notebooks`, a notebook is first a **document** — a document that
incorporates code and visuals to present data with written explanation.

This means that you need to provide text that walks your reader through the story of your
data analysis: what you are doing, why, how, and what we learn.  This does not mean you need
to describe every little detail, but you need to provide the context for what the analyses mean
and what we can learn from them.

Further, your assignment notebooks should be readable even without having read the original
assignment description: they should stand alone.  You can reuse a moderate amount of text
from the assignment description (e.g. including the questions verbatim in block quotations is
entirely acceptable), but you're going to need to do more writing and structuring to present
your results in a readable document.

The document also needs to include the Jupyter outputs — the reader should be
able to read it without re-running the code, although the code is there so they
can.

The reason for this is so that you learn to produce outputs that will be useful for your future
studies and work — documents that will communicate results to your colleagues, adviser, etc.
This is a class about doing data science, including communicating it, not just about writing
data science code.

## Writing and Formatting

[cm]: https://commonmark.org/help/

The text cells of notebooks use [Markdown syntax][cm] for formatting, and
support LaTeX math, delimited with `$` characters. For example, this code:

```markdown
The equation $a^n + b^n = c^n$ does not hold for integers $n>2$.
```

will yield:

> The equation $a^n + b^n = c^n$ does not hold for integers $n>2$.

It also supports block-mode math.

I encourage you to make judicious use of Markdown formatting to highlight important points and make
your notebooks easier to read.

One thing that is important to pay attention to is use of section headings, as discussed in the
lecture videos.  Section headings are indicated with `#` characters, as in:

```markdown
# Document Title

## Level 2 heading
```

Section headings are a crucial tool for structuring your document and making it
easier to read.  It's important to note, however, that these have actual
meaning: `##` does not mean “large bold font”; it means “level 2 heading”.  If
you look at the navigation menus on the right-hand side of the pages on the
course web site, these are extracted from the headings in the text.  Properly
structuring headings makes your document easier to read (see above, that a
notebook is a document), and also enables tooling that to support navigating the
document.  JupyterLab and extensions to the notebook server both provide
notebook outlines using the section headings.  Section headings should also be
short.

## Process

I recommend that you leave time before submitting your assignments to go back through the notebook
and clean it up for final presentation.

Sometimes it works best to start with the notebook you have and delete unnecessary code, remove
excess debugging outputs, and improve the writing.

Sometimes it works best to start a fresh notebook, start putting together the structure, and copy
over the code you actually need for the final solution.

Either way, you should produce a final notebook that is:

- readable
- executable from top to bottom
- clean of extraneous or unnecessary outputs, particularly without explanation

This last point is to avoid the “sea of charts” effect.  If there are a lot of charts and tables
that don't advance your story, it is much harder to read.

## Checklist

This checklist is to help you ensure your notebook is well-structured and well-written.
I may expand or revise it as we progress through the semester.

### Structure

-   Does the notebook re-run without error from top to bottom?
-   Does re-running the notebook produce correct charts and results?
-   Does the notebook begin with the document title as an L1 heading?
-   Are headings correctly nested (H2 within H1, H3 in H2, etc.)?
-   Are headings short titles? (No full sentences!)

### Writing and Output

-   Does the introduction state the notebook's purpose?
-   Does either the introduction or the data section describe where the data come from?
    -   If it's publicly downloadable, is there a link?
    -   If there are multiple options, which one is used?
-   Does it use correct grammar and spelling?
-   Does it use formatting to provide appropriate emphasis and clarity?
    -   Are Python variable, function, etc. names marked as `code`?
    -   Are lists used when helpful to break down points?
    -   Is mathematical notation used to precisely define measurements when it will increase clarity?
-   Do all outputs help advance the notebook's story?  Have you removed ones only for debugging or trying things out?
-   Do charts & conclusion-supporting outputs have surrounding text explaining their purpose and any extra information needed for accurate interpretation?
-   Do all relevant outputs have clear and accurate interpretation?

### Graphics

-   Do all charts have properly labeled axes and legends (color codes, etc.)?
-   Do charts have titles if purpose is not clear from axes or immediately preceding text?
    -   If there are multiple variants of a chart w/ same axes, they **must** have titles to quickly distinguish.
-   Are charts legible?
-   Do charts present lessons learned without distortions?
-   If you did not create the chart, would you be able to interpret it correctly?
-   Do facets, colors, and axes draw the reader to the most important comparisons or patterns?
-   Does surrounding text, if any, accurately interpret the chart?

The [Data Visualization Checklist](https://depictdatastudio.com/checklist/) is useful, if opinionated.

### Content

-   Are observations and conclusions substantiated by data and/or sound argument?
-   Are goals and observations made clear, both for the document and for individual pieces of analysis?

### Post-Export

-   Does PDF export include all outputs?
-   Are plots correctly displayed in the resulting PDF?  See [common problems](prob-mangled-pdf) for solutions.
