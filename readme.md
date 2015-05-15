This is an initial exploration of the Open Context site diaries found at

[http://opencontext.dainst.org/sets/.json?rows=2620&type=documents&start=1&response=uri][1] using David McClure's Textplot: 
[https://github.com/davidmcclure/textplot][2]

The materials from Open Context are CC-BY the original excavators.

My notes and files are at [Open Science Framework](https://osf.io) which I'll be making public in due course. For the time being, this repo hosts my explorations using Textplot, which I am contrasting with other forms of 'distant reading' this corpus of materials. I'm still getting to grips with the zooming interface, to make my images big enough to support the zoom. 

You can see my [latest attempt here](http://shawngraham.github.io/Open-Context-Site-Diaries/#oc-diaries/annotated/0.1936/0.8223/2.7378). The curly braces are my attempt at indicating - roughly - the 'dimension' or rough theme that seems to be structuring the discussion in that direction. Colour = modularity; node size = eigenvector centrality. I note that there are individuals' names that seem to happen only in particular modules, which is quite interesting. Some modules seem to go with that faux-objective clinical detachment (directing workmen, making decisions: archaeology is not revealed, but created! [text](http://shawngraham.github.io/Open-Context-Site-Diaries/#oc-diaries/annotated/0.3137/0.7567/8.1241)), while others hint at some of the passions, trials & tribulations of archaeology (for a poignant full example, see [this full-text](http://opencontext.dainst.org/documents/ACDA9FCB-9FC4-423F-BF6E-E6B7E278B3BD)).  Layout is force-directed, and so in itself x & y are meaningless, but given the way Textplot makes connections between words... well, I'll probably be changing these annotations before too long anyway!

-----

*Update* An updated version, w/o annotations because Inkscape is playing silly buggers with me, is [here](http://shawngraham.github.io/Open-Context-Site-Diaries/#13modules/13-modules/0.5000/0.5000/0.5871). Here, Textplot was set --bandwidth 100000, with no limits on number of terms etc. GML -> Gephi; Gephi found 13 extremely likely (per the algorithmn) modules, and so I recoloured accordingly. Sizing by eigenvector centrality.

Let's compare the structure uncovered by Textplot with the topics deduced by Mallet in R. Mallet is looking at the distribution of topics over the entire collection of site diaries rather than their ordering (as Textplot does). [In this document](http://rpubs.com/shawngraham/79365) I've fitted 13 topics, given how nicely those 13 modules emerged from the textplot graph.





  [1]: http://opencontext.dainst.org/sets/.json?rows=2620&type=documents&start=1&response=uri
  [2]: https://github.com/davidmcclure/textplot
