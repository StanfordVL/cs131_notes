# CS131 Computer Vision:  Foundations and Applications

## Instructions for creating class notes

### Signup to write the notes for a particular lecture.

[Here is the link](https://docs.google.com/spreadsheets/d/1-2PAMFgZ7m2AYlgrzsbynwlGULUp_DdlX3N6h5S9n78/edit#gid=0). Try and choose lectures that have no students signed up yet.

### Overall workflow
1. Fork this repository by clicking the "Fork" button on the top right of [this
page](https://github.com/StanfordVL/cs131_notes).

2. Next, clone your forked repository into your local machine:
```
git clone github.com/YOUR_GITHUB_ACCOUNT/cs131_notes.git
```
3. Give others permission to commit to your forked repository by clicking on
"Settings" and then "Collaborators".
3. Write up the class notes.
4. Push your changes to your forked repository.
5. Send a pull request to the official
[repository](https://github.com/StanfordVL/cs131_notes).

### Downloading the software and testing the repository.
1. Download [pdfltex](https://www.tug.org/applications/pdftex/) so that you can
compile the tex documents. You can also use [Overleaf](overleaf.com) or
[Sharelatex](sharelatex.com) to compile your tex documents.

2. Go into the template folder and compile the format and template files:
```
cd template

pdflatex format.tex
bibtex format
pdflatex format.tex

pdflatex template.tex
bibtex template
pdflatex template.tex
```

3. Make sure that template.pdf and format.pdf have been generated and are correctly
displayed. Read format.pdf to understand how we expect the class notes to be
formatted.

### Writing class notes for a given lecture
1. Create a folder called `LectureXX` where `XX` is `01` for the first lecture
or `18` for the eighteenth lecture.

2. Copy over template.tex and bibliography.bib to your folder.
```
cp template/template.tex lectureXX/lectureXX.tex
cp template/bibliography.bib lectureXX/bibliography.bib
```

3. Write the lecture notes. Make sure to include pictures, references and
tables. If you add images, make sure to give credit to the source of those
images.

4. Compile your lecture template to make sure that it formats correctly.
```
cd lectureXX
pdflatex lectureXX.tex
bibtex lectureXX
pdflatex lectureXX.tex
```

5. Submit a pull request to have your lecture notes merged.
