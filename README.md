# IITP CSE PhD thesis template

IIT Patna PhD Thesis template for CSE department. Sample thesis can be found [here](thesis.pdf).

> NOTE: Please read the comments in the tex file before delete anything.

### Directory structure

```
.
├── Appendix
│   ├── Appen1.tex
├── Chapter1 				# Contribution Chapter 1
│   ├── chapter1.tex
│   └── Images
├── HeadTail
│   ├── abstract.tex			# Thesis abstract
│   ├── ack.tex				# Acknowledgement
│   ├── Appen1.tex
│   ├── biodata.tex
│   ├── Certificate_of_approval_DC.tex	# Approval from DC
│   ├── cert.tex			# Declaration by supervisor
│   ├── coverpage.tex
│   ├── Declaration.tex			# Declaration by scholar
│   ├── dedication.tex			# Dedication
│   ├── iitplogo.eps			# Institute logo
│   ├── publication.tex			# Publication list
│   └── title.tex			# Thesis title
├── latexmkrc				# Overleaf file
├── README.md
├── References
│   ├── references.tex			# References file
│   └── ThesisBib.bib			# BibTex file
├── Symbol
│   ├── abbreviation.tex		# Abbreviation list
│   └── listofsymbol.tex		# Symbol list
├── thesis.pdf
└── thesis.tex				# Main Thesis file

```

### Added your details

Given your details at YOUR DETAILS in `thesis.tex` preamble like below: 

```
%% YOUR DETAILS
\newcommand{\thesistitle}{Thesis Title}
\newcommand{\authorname}{My Name}
\newcommand{\authorrollno}{XX21CSXX}
\newcommand{\supervisorname}{Dr. X}
```

### How to add new chapter?

If you want to add more chapters, which might be needed for showing another/more contributory chapters, make a copy of `Chapter1` folder and rename it and include new chapter before the thesis conclusion. 

```
\include{Chapter1/chapter1} 
\include{Chapter2/chapter2} % new chapter
```

### Lists

List of Figures and Tables will be generated automatically but List of Notations should be mannually added.

### How to add reference?

Here we use BibTex  to describe and process lists of references. Your bib file can be found at `References/ThesisBib.bib`. Add all your BibTex in this bib file.

### Work offline and with Overleaf

A `latexmkrc` file is a configuration / initialization (RC) file for the Latexmk package. Latexmk is used by Overleaf to control the compilation of your source LaTeX document into the final typeset PDF file. By using a customized configuration file called Latexmk you can override the default compilation commands to [allow Overleaf to compile](https://www.overleaf.com/learn/latex/Articles/How_to_use_latexmkrc_with_Overleaf:_examples_and_techniques) your document in a special way. Please do not delete this file.
