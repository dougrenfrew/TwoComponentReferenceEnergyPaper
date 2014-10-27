# TwoComponentReferenceEnergyPaper

This is the LaTeX code for the paper entitled 'Two Component Reference Energy for the Design of Peptides and Foldamers'

## Building
To build the document run the following commands below. All of th packages should be available from the TeXLive ditrobution (MacTeX on Mac OS 10). The article is currently set up to use `biber` and `biblatex` for the bibliography. Both of those packages handle unicode characters (which `bibtex` does not) which ultimatly makes formattng the bibliography easier. 
```
pdflatex tcre
biber tcre
pdflatex tcre
pdflatex tcre
```
## Git Info
To produce the footer with the git resvision info provided by the `gitinfo2` package, you will need to create three git hooks. You will need to copy or sybolically link the sample git hook that came with the package in to your `.git/hooks` folder as a `post-checkout`, `post-commit`, and `post-merge` hook. The paths below might be different from your own. 

```
ln -s /usr/local/texlive/2014/texmf-dist/doc/latex/gitinfo2/post-xxx-sample.txt TwoComponentReferenceEnergyPaper/.git/hooks/post-checkout
ln -s /usr/local/texlive/2014/texmf-dist/doc/latex/gitinfo2/post-xxx-sample.txt TwoComponentReferenceEnergyPaper/.git/hooks/post-commit
ln -s /usr/local/texlive/2014/texmf-dist/doc/latex/gitinfo2/post-xxx-sample.txt TwoComponentReferenceEnergyPaper/.git/hooks/post-merge
```
