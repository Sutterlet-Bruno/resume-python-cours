commande de génération du rapport :
```bash
pandoc resume.md -o resume.pdf --pdf-engine=pdflatex --from markdown --template ./eisvogel.latex --listings
```

Paquet à installer pour la génération du rapport :
+ texlive (attention, il est très lourd)
+ pandoc (pour la génération du pdf)

Note :
I started with the heig.latex template that seems to be an update/improvement of the eisvogel.latex template. But I had some issues with the heig.latex template, so I switched to the eisvogel.latex template.
It seems the '@' character is not supported in the heig.latex template due to the use of it for pandoc functions. I tried to fix the problem but did not succeded. So I switched to the eisvogel.latex template and it worked.