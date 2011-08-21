all: latex_part
	dvips -Ppdf -P cmz -Pdownload35 -j0 -G0 -t letter -o mram.ps mram.dvi
	ps2pdf14 -dPDFSETTINGS=/prepress -dEmbedAllFonts=true mram.ps
	chmod 777 *.*
latex_part:
	latex mram; bibtex mram; latex mram; latex mram;
mram.pdf:
	ps2pdf mram.ps mram.pdf
clean:
	rm -f mram.aux   mram.bbl   mram.blg  mram.brf   mram.dvi   mram.log  mram.ps  
