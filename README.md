## Command line instruction to webpage

Github-pages documentation: [GitHub Pages Documentation - GitHub Docs](https://docs.github.com/en/pages)

Jekyll documentation: [Quickstart | Jekyll • Simple, blog-aware, static sites](https://jekyllrb.com/docs/)

#### Compile webpage locally

Compile the webpage locally **before** commiting changes to git ! To do so:

- Be sure to use the correct version of ruby:
  
  ```
  rvm 3.2.3
  ```

- (optional) if not compiled for some time:
  
  ```
  bundle update
  ```

- Then to create local link:
  
  ```
  bundle install
  bundle exec jekyll serve
  ```

#### Compile webpage on internet

If everything is as wanted, just commit and push changes. Compilation is automatic 

#### Modify CV with bibliography

CV uses biblatex with biber backend to include bibliography. To modify the .pdf output it must be compiled twice:

```
pdflatex CV_english_RBarboni.tex
biber CV_english_RBarboni
pdflatex CV_english_RBarboni.tex
```

More info available here: http://randyklabacka.com/2020/07/02/LaTeX_CreateModernCV.html
