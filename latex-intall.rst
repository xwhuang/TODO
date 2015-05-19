1) get texlive install packet(installed from network)
   wget http://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz

2) uncompress install-tl-unx.tar.gz then 
   sh install-tl

3) set enviroment
   add "/usr/local/texlive/2014/bin/x86_64-linux" to PATH
   or edit /etc/enviroment or edit /etc/sudoers

4) update emcas's org-mode
   M-x packet-install RET org

5) edit .emacs file
   add follows:
   (setq org-latex-pdf-process '("xelatex -interaction nonstopmode %f"
                                "xelatex -interaction nonstopmode %f"))

6) install xecjk

7) add new fonts
   mv *.otf to /usr/share/fonts/truetype/adobe
   fc-cache -r -v 
   fc-list 

8) usepackage/xecjk
   \usepackage{xeCJK}
   \setCJKmainfont[BoldFont=Adobe Heiti Std,ItalicFont=Adobe Kaiti Std]{Adobe Song Std}
