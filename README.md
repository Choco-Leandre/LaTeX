## Bienvenue sur mes fichiers LaTeX
Ici je partage des exemples de documents LaTeX que j'ai pu faire et mon package pour réaliser mes compositions.
### - Utiliser `lcpackage`
- Téléchargez le fichier `lcpackage.sty`

Vous utilisez **TeXLive** (Windows):
- Mettez le fichier `.sty` dans `C:\texlive\texmf-local\tex\latex\local\`
- Dans l'invite de commande à l'emplacement du fichier, tapez la commande `texhash`
- Attendez qu'il y ai de marqué `Done.`

Vous utilisez **MikTeX**
- Allez dans `C:\Users\NOM\AppData\Local\MiKTeX\`
> Veuillez changer votre NOM par celui de votre nom d'utilisateur Windows
- Naviguez vers `tex\latex\`
> A créer si les dossiers n'existent pas
- Mettre le fichier `.sty`
- Sur MikTeX Console, dans `Tasks`, cliquez sur `Refresh file name database` ou `Refresh FNDB`

Ensuite:
- Sur TeXMaker ou autre, utilisez la commande suivante:
> Sauf Overleaf, vous devez mettre le fichier `.sty` dans la racine avant de compiler
```latex
\documentclass{article}
\usepackage{lcpackage}
% Vous pouvez ajouter d'autres commandes ou packages si besoin

\begin{document}
\pagestyle{fancy} 
\fancyhf{}
\fancyhead[L]{{\fontfamily{phv}\selectfont Matière}}
\fancyhead[C]{{\fontfamily{phv}\selectfont $\cdots$ Titre - Nom $\cdots$}}
\fancyhead[R]{{\fontfamily{phv}\selectfont Page \thepage /\pageref{LastPage}}}
{\fontfamily{phv}\selectfont
\begin{center}
\Huge{Titre}
\end{center}

\end{document}
```
- Compilez, et ça devrait être tout bon!
