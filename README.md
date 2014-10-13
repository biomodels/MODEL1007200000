

This is the model described in the article:  
**In silico experimentation with a model of hepatic mitochondrial folate metabolism.**   
H. Frederik Nijhout, Michael C Reed, Shi-Ling Lam, Barry Shane, Jesse F
Gregory and Cornelia M Ulrich, _Theor Biol Med Model_ 2006,3:40; PubmedID:
[17150100](http://www.ncbi.nlm.nih.gov/pubmed/17150100) ; DOI:
[10.1186/1742-4682-3-40](http://dx.doi.org/10.1186/1742-4682-3-40) ;  
Abstract:  
BACKGROUND: In eukaryotes, folate metabolism is compartmentalized and occurs
in both the cytosol and the mitochondria. The function of this
compartmentalization and the great changes that occur in the mitochondrial
compartment during embryonic development and in rapidly growing cancer cells
are gradually becoming understood, though many aspects remain puzzling and
controversial.  
APPROACH: We explore the properties of cytosolic and mitochondrial folate
metabolism by experimenting with a mathematical model of hepatic one-carbon
metabolism. The model is based on known biochemical properties of
mitochondrial and cytosolic enzymes. We use the model to study questions about
the relative roles of the cytosolic and mitochondrial folate cycles posed in
the experimental literature. We investigate: the control of the direction of
the mitochondrial and cytosolic serine hydroxymethyltransferase (SHMT)
reactions, the role of the mitochondrial bifunctional enzyme, the role of the
glycine cleavage system, the effects of variations in serine and glycine
inputs, and the effects of methionine and protein loading.  
CONCLUSION: The model reproduces many experimental findings and gives new
insights into the underlying properties of mitochondrial folate metabolism.
Particularly interesting is the remarkable stability of formate production in
the mitochondria in the face of large changes in serine and glycine input. The
model shows that in the presence of the bifunctional enzyme (as in embryonic
tissues and cancer cells), the mitochondria primarily support cytosolic purine
and pyrimidine synthesis via the export of formate, while in adult tissues the
mitochondria produce serine for gluconeogenesis.

This model does not reproduce the results in the article completely, but most
steady state concentrations are in a range of 10% around the published values.
Also parameterscans give nearly identical results as shown in the article.

In the SBML version model the volumes of the mitochondrion, the cytoplasm and
the cell were all set to one to obtain the same equations as described in the
supplemental materials of the article. The total folate is equally split
between the cytosol and the mitochondrion and divided by 3/4 for the cytosol
and 1/4 for the mitochondrion, respectively. To obtain an SBML model in which
the volumes of the compartments, _cytosol_ and _mito_ , are used, the model
needs to be altered as follows:  
for the initial distribution of folate the terms 3/4 and 1/4 have to be
replaced by volumes of cytosol and mitochondria respectively  
in the transport reactions between mitochondrion and cytosol the stoichiometry
of the mitochondrial reactants has to be set from 3 to 1 and in the first part
of the according rate laws the factor _mito/3_ should simply be replaced with
_mito_ .  
the stoichiometries of _src_ and _dmg_ have to be changed to _cell/mito_ for
mitchondrial and _cell/cytosol_ for cytosolic reactions involving these two
species.  
While the concentrations stay the same after these alteration, the reaction
fluxes change by a factor of _cytosol_ and _mito_ for cytosolic and
mitchondrial reactions, respectively.

Originally created by libAntimony v1.3 (using libSBML 3.4.1)

This model originates from BioModels Database: A Database of Annotated
Published Models (http://www.ebi.ac.uk/biomodels/). It is copyright (c)
2005-2011 The BioModels.net Team.  
To the extent possible under law, all copyright and related or neighbouring
rights to this encoded model have been dedicated to the public domain
worldwide. Please refer to [CC0 Public Domain
Dedication](http://creativecommons.org/publicdomain/zero/1.0/) for more
information.

In summary, you are entitled to use this encoded model in absolutely any
manner you deem suitable, verbatim, or with modification, alone or embedded it
in a larger context, redistribute it, commercially or not, in a restricted way
or not..  
  
To cite BioModels Database, please use: [Li C, Donizelli M, Rodriguez N,
Dharuri H, Endler L, Chelliah V, Li L, He E, Henry A, Stefan MI, Snoep JL,
Hucka M, Le Novère N, Laibe C (2010) BioModels Database: An enhanced, curated
and annotated resource for published quantitative kinetic models. BMC Syst
Biol., 4:92.](http://www.ncbi.nlm.nih.gov/pubmed/20587024)

