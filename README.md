<a href="https://thepreservedbible.com/" title="Why the King James Bible?"><img src="https://i.ibb.co/svCrDys/The-Preserved-Bible-Small.jpg" width="300" align="right"></a>

# kjv

Read the Word of God from your terminal

Forked from (layeh/kjv)[https://github.com/layeh/kjv] to include apocrypha, sourced from (lukesmithxyz/kjv)[https://github.com/lukesmithxyz/kjv].

## Usage

    usage: kjv [flags] [reference...]

    Flags:
      -A num  show num verses of context after matching verses
      -B num  show num verses of context before matching verses
      -C      show matching verses in context of the chapter
      -e      highlighting of chapters and verse numbers
              (default when output is a TTY)
      -p      output to less with chapter grouping, spacing, indentation,
              and line wrapping
              (default when output is a TTY)
      -l      list books
      -h      show help

    Reference:
        <Book>
            Individual book
        <Book>:<Chapter>
            Individual chapter of a book
        <Book>:<Chapter>:<Verse>[,<Verse>]...
            Individual verse(s) of a specific chapter of a book
        <Book>:<Chapter>-<Chapter>
            Range of chapters in a book
        <Book>:<Chapter>:<Verse>-<Verse>
            Range of verses in a book chapter
        <Book>:<Chapter>:<Verse>-<Chapter>:<Verse>
            Range of chapters and verses in a book

        /<Search>
            All verses that match a pattern
        <Book>/<Search>
            All verses in a book that match a pattern
        <Book>:<Chapter>/<Search>
            All verses in a chapter of a book that match a pattern

## Build

kjv can be built by cloning the repository and then running gmake:

    git clone https://github.com/calebstein1/kjv.git
    cd kjv
    gmake
    doas make install

## License

Public domain
