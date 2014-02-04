LobLib
========

#### The Lobster Library ####

LobLib is a LaTeX package for creating lobster themed documents and make inserting a wide range of lobster images into papers.

[Examples](https://github.com/bae43/LobLib/tree/master/documentation/examples) —
[Documentation](https://github.com/bae43/LobLib/tree/master/documentation) —


### Usage ###

Download the style and object folder and place them in tex/tempf. Refresh the File System Database as per guidlines of installing custom packages ([More Info](http://www.math.uiuc.edu/~hildebr/tex/tips-customstyles.html)). LobLib requires [TikZ & PGF](http://www.ctan.org/pkg/pgf) and [PGF Ornament](http://altermundus.com/pages/downloads/packages/pgfornament/ornaments.pdf).

### Features ###


Intended for use of problem sets, a title constructor creates a lobster themed title when filling in the following fields
```latex
\renewcommand{\coursename}{ Algorithms  }
\renewcommand{\coursenumber}{ CS 4820 }
\renewcommand{\name}{ Bryce Evans  }
\renewcommand{\netid}{bae43}
\renewcommand{\today}{September 12, 2013}
\renewcommand{\hwnum}{1}
\renewcommand{\hwtitle}{NP-Completeness }
\makelobtitle
```

Use \lob for adding in any of the lobsters numbered in the documentation. Current Version has 92 Lobsters and counting. Add any options supported by TikZ for customization of any image. All symbols and images are vectorized for scalability.
```latex
\lob{1}
\lob{2}
\lob{3}
% ...
\lob[size=3, color=blue]{92}
```

Watermarks can be added as well
```latex
\BgThisPage
```

Other misc. additions include section breaks, claw tombstones for proofs, 
```latex
\lobsectionbreak
\clawtomb

```


