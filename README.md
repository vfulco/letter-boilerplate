# Letter Boilerplate

A boilerplate to quickly and painlessly generate typographically perfect letters using LaTeX. The perfect companion to [cv-boilerplate](https://github.com/mrzool/cv-boilerplate).

![preview](preview.jpg)

## Dependencies

1. LaTeX with the following extra packages: `fontspec` `geometry` `ragged2e` `enumitem` `xunicode` `xltxtra` `hyperref` `polyglossia`
2. Pandoc

To install LaTeX on Mac OS X, I recommend getting the smaller version BasicTeX from [here](https://tug.org/mactex/morepackages.html) and installing the additional packages with `tlmgr` afterwards. Same goes for Linux: install `texlive-base` with your package manager and add the needed additional packages later.

To install pandoc on Mac OS X, run `brew install pandoc`. To install it on Linux, refer to the [official docs](http://pandoc.org/installing.html).

## Getting started

1. Edit `details.yml` with your details, your recipient's details, and the desired settings.
2. Open `content.md` and write your letter in markdown.
2. Run `make` to compile the PDF.

The template automatically includes `signature.pdf` after the letter's body as a final touch. Check out [this method](http://tex.stackexchange.com/a/32940/82423) for importing your own signature.

Refer to [pandoc's documentation](http://pandoc.org/demo/example9/templates.html) to learn more about how templates work.

**Note**: this template needs to be compiled with XeTeX.

## Available settings

- **`mainfont`**: Hoefler Text is the default, but every font installed on your system should work out of the box (thanks, XeTeX!)
- **`sansfont`**: Used to render the recipient address so that it stands out from the rest of the letter.
- **`fontsize`**: Possible values here are 10pt, 11pt and 12pt.
- **`lang`**: Sets the main language through the `polyglossia` package. This is important for proper hyphenation, among other things.
- **`geometry`**: A string that sets the margins through `geometry`. Read [this](https://www.sharelatex.com/learn/Page_size_and_margins) to learn how this package works.

## Recommended reading

- [The Beauty of LaTeX](http://nitens.org/taraborelli/latex) by Dario Taraborelli
- [Letterhead advices](http://practicaltypography.com/letterhead.html) from Butterick's Practical Typography 

## License

[MIT](https://opensource.org/licenses/MIT)
