This demonstrates footnotes being caught by the sphinxcontrib-spelling

I'm building this with 

```
sphinx-build -b html -b spelling source build
```

I see output like this:

```
Running Sphinx v5.0.2
Initializing Spelling Checker 7.5.1
loading pickled environment... done
Ignoring wiki words
Ignoring acronyms
Ignoring Python builtins
Ignoring importable module names
Ignoring contributor names
Looking for custom word list in C:\Projects\sphinx-test\source\spelling_wordlist.txt
Scanning contributors
myst v0.18.0: MdParserConfig(commonmark_only=False, gfm_only=False, enable_extensions=[], disable_syntax=[], all_links_external=False, url_schemes=('http', 'https', 'mailto', 'ftp'), ref_domains=None, highlight_code_blocks=True, number_code_blocks=[], title_to_header=False, heading_anchors=None, heading_slug_func=None, footnote_transition=True, words_per_minute=200, sub_delimiters=('{', '}'), linkify_fuzzy_links=True, dmath_allow_labels=True, dmath_allow_space=True, dmath_allow_digits=True, dmath_double_inline=False, update_mathjax=True, mathjax_classes='tex2jax_process|mathjax_process|math|output_area')
building [mo]: targets for 0 po files that are out of date
building [spelling]: all documents
updating environment: 0 added, 0 changed, 0 removed
looking for now-outdated files... none found
preparing documents... done
Writing C:\Projects\sphinx-test\build\example/markdown.spelling
Writing C:\Projects\sphinx-test\build\example/restructured.spelling
writing output... [100%] spelling_wordlist
WARNING: source\example\markdown.md:0: : Spell check: ovbiously: this is very ovbiously mispeled.
WARNING: source\example\markdown.md:0: : Spell check: mispeled: this is very ovbiously mispeled.
WARNING: source\example\markdown.md:0: : Spell check: https: https://github.com/microsoft/microsoft-ui-xaml.
WARNING: source\example\markdown.md:0: : Spell check: github: https://github.com/microsoft/microsoft-ui-xaml.
WARNING: source\example\markdown.md:0: : Spell check: microsoft: https://github.com/microsoft/microsoft-ui-xaml.
WARNING: source\example\markdown.md:0: : Spell check: microsoft: https://github.com/microsoft/microsoft-ui-xaml.
WARNING: source\example\markdown.md:0: : Spell check: ui: https://github.com/microsoft/microsoft-ui-xaml.
WARNING: source\example\markdown.md:0: : Spell check: xaml: https://github.com/microsoft/microsoft-ui-xaml.
WARNING: source\example\restructured.rst:5: : Spell check: ovbiously: this is very ovbiously mispeled.
WARNING: source\example\restructured.rst:5: : Spell check: mispeled: this is very ovbiously mispeled.
WARNING: Found 10 misspelled words
build succeeded, 11 warnings.
```