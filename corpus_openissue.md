# Open issue:

## Individual list

- 10024470:  subsequent reduction by NADPH (Does it really happen by enzyme?)
- PMID-10601247: All "PLS-DSD" should turn into complex.
- PMID-10762278: Tn5 intersection need more curation. D-galactarate, D-glucarate systems shouldn not be metabolite.
- PMID-10769117:  propionyl CoA:succinate CoA transferase <- should be single entity instead.
- PMID-10933791: ES complex <- this is annotated as metabolite
- PMID-1095572: Leucine transport, Leucine-specific.  Should I remove "chmemical" annotation from leucine?
- PMID-11168365: "biosynthesis of the vitamins thiamine and pyridoxal"  Take a look at  vitamin.
- PMID-11396917: "orthovanadate (VO(3-)(4))-bound enzymes has also revealed the common molecular mechanism of the transfer reaction catalyzed by sulfotransferses"
- PMID-11676470: "oxidized nucleotides", why it is a metabolite? can I mark it as "small molecules" Escherichia coli should be delete out of protein entity
- PMID-11698387: Gm2251 is a part of 23 rRNA
- PMID-11737206: 
  - "fungal alanine racemase", should I remove fungal?
  - "vitamin B6-dependent enzymes" <- it is to ambiguous?
  - SHMT shows a broad range of reaction specificity, being able to catalyse at appreciable rates retroaldol cleavage, racemase, aminotransferase and decarboxylase reactions.
  - aldolase from E. coli and alanine racemase from Cochliobolus carbonum
  - "SHMT crystal structure" and "tetrahydrofolate binding site", should I split them?
- PMID-11790762
  - Zn(II) uptake system  does not tag. (go with pmid-1095572 problem)
- PMID-11932438:  
  - "that S-adenosylhomocysteine (SAH) or 5'-methylthioadenosine (MTA) serves as a substrate for AI-2 production. Cell-free extracts of Escherichia coli MG1655, but not DH5alpha (which carries a luxS frame-shift mutation) were capable of generating AI-2 activity upon addition of SAH," <- This whole thing may need some review.
  - "RH"-supplemented cell-free extracts of Pseudomonas aeruginosa
- PMID-11967075
  - "polytopic membrane proteins" should be delete out.
  - "nitrite ex-cretion"

- PMID-12107134: yegMNOB (mdtABCD) transporter gene cluster


Stop at 12399477:



Some open issue from reviewer.
==============================
Overall, he argue that we should annotate using biologically relevant and disregard about linguistic feature 


------------

14.	"In the second phase of the reaction, various 2-keto acids can compete for this intermediate to form the respective acetohydroxy acids." While there clearly is a metabolic reaction of the form "2-keto acids" # "acetohydroxy acids" going on, there is no enzyme in the sentence to associate the metabolites. At the very least, the authors need to acknowledge this shortcoming in their paper. Other than that, this shows that while sometimes strings like "amino acids" were annotated as metabolites, there are relevant entities not annotated in the corpus.

--------------


6. The annotated entities and triggers need to be described and the boundaries of what constitutes a valid or invalid entity detailed (see corpus issues, too). Furthermore, what a "correct span" of those entities represents has to be specified. Also, a specification of what a valid trigger word is (and/or what not) is required. Even GREC only has a short section on Reagents (p. 17 of their guidelines), and this does not cover all the issues encountered when detecting chemical entities, as recent community challenges (BioCreative) have shown. For example, there are obvious inconsistencies of the offsets/spans of entities in PMID 2007556 ("ilvGMEDA operon *of E. coli*"). Another example: "*major* G3P dehydrogenase" (9696782:19). In that same article, why is the noun phrase head "mutants" part of a gene entity (:25)? All these and many more, similar entity boundaries issues in the corpus have to be fixed and specified in the guidelines.


## Missing?

## What specificity
(Maybe I should have another class for them, entity?)
Amino acid,
one-carbon metabolism (e.g. nucleic acid synthesis)


## Event
Just how vivid it should be, mechanical description is obious choice
Anaphora?  
Gene and proteins

## Edges case
"First, tktA tktB double mutants, which lack transketolase activity and cannot synthesize"


## Upgrade my corpus

Preposition (IN). Several preposition seems to reinforce and change event type.
http://128.199.144.116:8083/#/annotator_agreement/corpus/PMID-10024470 (by, and to change "reduction" event)
/annotator_agreement/corpus/PMID-10074354 (IN "from")

## Annotator agreement
PMID-10091662 <- enediol structure is being to broad., hydroxyl O1 sounds like a part
PMID-10671448 <- "Only phosphoserine could be detected after acid hydrolysis of the labeled protein, and site-directed mutagenesis of serine residues located in or near the active site identifies the serine residue at position 102 as the site of autophosphorylation o" <- about serine part.
PMID-12896971 <- "PdxA catalyzes a stepwise oxidative decarboxylation of the substrate HTP.".
PMID-12896974-INTRODUCTION <- What about EDTA? <- not count
                           <- maybe I should not include bound.
PMID-13405870 <- "Wood and Gunsalus enzyme" 
PMID-355220 <- Show that event can reach very far.
PMID-378964 <- Don't consider a separate amino sequence.
PMID-3884731 <- Anticapsin
PMID-9537380-INTRODUCTION <- Event --> --> From

### need to emphasize on
