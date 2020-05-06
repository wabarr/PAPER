all: WAB_CV.pdf

WAB_CV.pdf: barrpubs.tex WAB_CV.tex
	pdflatex WAB_CV.tex
	pdflatex WAB_CV.tex
	open -a Preview ~/Documents/GitHub/PAPER-lab/assets/CV/WAB_CV.pdf
	git commit -m "update CV"
	git push
