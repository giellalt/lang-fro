


















* Sets for POS sub-categories





* Sets for Semantic tags





* Sets for Morphosyntactic properties






































































































































































* Sets for verbs


- V is all readings with a V tag in them, REAL-V should
be the ones without an N tag following the V.  
The REAL-V set thus awaits a fix to the preprocess V ... N bug.



* The set COPULAS is for predicative constructions







* NP sets defined according to their morphosyntactic features







* The PRE-NP-HEAD family of sets

These sets model noun phrases (NPs). The idea is to first define whatever can
occur in front of the head of the NP, and thereafter negate that with the
expression **WORD - premodifiers**.












The set **NOT-NPMOD** is used to find barriers between NPs.
Typical usage: ... (*1 N BARRIER NPT-NPMOD) ...
meaning: Scan to the first noun, ignoring anything that can be
part of the noun phrase of that noun (i.e., "scan to the next NP head")






* Miscellaneous sets





















* Border sets and their complements













* Syntactic sets




These were the set types.



## HABITIVE MAPPING


* **hab1** 


* **hab2** 

* **hab3** (<hab> @ADVL>) for hab-actor and hab-case; if leat to the right, and Nom to the right of leat. Lots of restrictions.



* **habNomLeft** 


* **hab4** 	



* **hab6** 

* **hab7** 

* **hab8** This is not HAB
* **hab5**  This is not HAB



* **habDain** (<hab> @ADVL>) for (Pron Dem Pl Loc) if leat followed by Nom to the right




* **habGen** (<hab> @<ADVL) hab for Gen; if Gen is located in the end of the sentence and Nom is sentence initial










































































* **spred<obj** (@SPRED<OBJ) for Acc; the object of an SPRPED. Not to be mistaken with OPRED. If SPRED is to the left, and copulas is to the left of it. Nom or Hab are found sentence initially.


* **Hab<spred** (@<SPRED) for Nom; if copulas, goallut or jápmit is FMAINV and habitive or human Loc is found to the left. OR: if Ill or @Pron< followed by HAB are found to the left.

* **Hab>Advlcase<spred** (<ext> @<SUBJ) for Nom; it allows adverbials with Ill/Loc/Com/Ess to be found inbetween HAB and <ext>.

* **Nom>Advlcase<spred** (<ext> @<SUBJ) for Nom; it allows adverbials with Ill/Loc/Com/Ess to be found inbetween Nom and <ext> @<SUBJ.

* **<spred** (<ext> @<SUBJ) for Nom; if copulas to the left, and some kind of adverb, N Loc, time related word or Po to the left of it. OR: if Ill or @Pron< to the left, followed by copulas and the before mentioned to the left of copulas. 

* **<spred** (<ext> @<SUBJ) for Nom, but not for Pers. To the left boahtit or heaŋgát as MAINV, and futher to the left is some kind of place related word, or time related word


* **<spredQst1** (<ext> @<SUBJ) for Nom in a typically question sentence; if A) Hab, some kind of place word, Po or Nom to the left, and Qst followed by copulas to the left. B) same as a, only the Qst-pcle is attached to copulas. C) Qst to the left, with copulas to its left, but not if two Nom:s are found somewhere to the right. D) copulas to the left, and BOS to the left. E) Loc or Ill to the left, and Loc or Hab to the left of this, Qst and copulas to the left. F) Num @>N to the left, Hab, some kind of place word, Po or Nom to the left, and Qst followed by copulas to the left. NOTE) for all these rules; human, Loc or Sem/Plc not allowed to the right.

* **<spredQst2** (@<SPRED) for Nom; in a typically question sentence; differs from <spredQst1 by not beeing as restricted to the right. Though you are not allowed to be Pers or human.

* **Nom<spredQst** (@<SPRED) for Nom; in a typically question sentence. Differs from <spredQst2 by letting Nom be found between SPRED and copulas



* **<spred** (@<SPRED) for A Nom or N Nom if; the subject Nom is on the same side of copulas as you: on the right side of copulas

* **<spredVeara** (@<SPRED) for veara + Nom; if genitive immediately to the right, and intransitive mainverb to the right of genitive

* **leftCop<spred** (@<SPRED) for Nom; if copulas is the main verb to the left, and there is no Ess found to the left of cop (note that Loc is allowed between target and cop). OR: if you are Coll or Sem/Group with copulas to your left. 

* **<spredLocEXPERIMENT** (@<SPRED) for material Loc; if you are to the right of copulas, and the Nom to the left of copulas is not a hab-actor


* **NumTime** (@<SPRED) for A Nom

* **<spredSg** (@<SPRED) for Sg Nom	

* **<spredPg** (@<SPRED) for Pl Nom	

* **<spred** (@<SPRED) for Nom; if copulas to the left, and Nom or sentence boundary to the left of copulas. First one to the right is EOS.

* **<spred** (@<SPRED) for N Ess

* **spredEss>** (@SPRED>) for N Ess; if copulas to the right of you, and if an NP with nom-case first one to your left.

* **HABSpredSg>** (@SPRED>) for Nom; if habitive first one to the left, followed by copulas.

* **GalleSpred>** (@SPRED>) for Num Nom; if sentence initial

* **spredSgMII>** (@SPRED>)

* **r492>** (@SPRED>) for Interr Gen; consisting only of negations. You are not allowed to be MII. You are not allowed to have an adjective or noun to yor right. You are not allowed to have a verb to your right; the exception beeing an aux.



* **AdjSpredSg>** (@SPRED>) for A Sg Nom; if copulas to the right, but not if A or @<SPRED are found to the right of copulas

* **SpredSg>Hab** (@SPRED>) for Nom; if you are sentence initial, copulas is located to the right, and there is a habitive to the right of copulas



* **Spred>SubjInf** (@SPRED>) for Nom; if copulas to the right, and the subject of copulas is an Inf to the right

* **spredCoord** (@<SPRED) coordination for Nom; only if there already is a SPRED to the left of CNP. Not if there is some kind of comparison involved.






* **subj>Sgnr1** (@SUBJ>) for Nom Sg, including Indef Nom if; VFIN + Sg3 or Pl3 to the right (VFIN not allowed to the left) 

* **subj>Du** (@SUBJ>) for dual nominatives, including Coll Nom. VFIN + Du3 to the right. 
* **subj>Pl** (@SUBJ>) for plural nominatives, including Coll and Sem/Group. VFIN + Pl3 to the right.

* **subj>Pl** (@SUBJ>) for plural nominatives


* **subj>Sgnr2** (@SUBJ>) for Nom Sg; if VFIN + Sg3 to the right.

* **<subjSg** (@<SUBJ) for Nom Sg; if VFIN Sg3 or Du2 to the left (no HAB allowed to the left).




















* **f<advl** (@-F<ADVL) for infinite adverbials

* **f<advl** (@-F<ADVL) for infinite adverbials



* **s-boundary=advl>** (@ADVL>) for ADVL that resemble s-booundaries. Mainverb to the right.




* **-fobj>** (@-FOBJ>) for Acc 

* **-fobj>** (@-FOBJ>) for Acc




* **advl>mainV** (@ADVL>) if; finite mainverb not found to the left, but the finite mainverb is found to the right.


* **<advl** (@<ADVL) if; finite mainverb found to the left. Not if a comma is found immediately to the left and a finite mainverb is located somewhere to the right of this comma.




* **<advlPoPr** (@<ADVL) if mainverb to the left.
* **advlPoPr>** (@<ADVL) if mainverb to the right.



* **advlEss>** (@<ADVL) for weather and time Ess, if FMAINV to the left.






* **advl>inbetween** (@ADVL>) for Adv; if inbetween two sentenceboundaries where no mainverb is present.

* **comma<advlEOS** (@<ADVL) if; comma found to the left and the finite mainverb to the left of comma. To the right is the end of the sentence.



* **advlBOS>** (@ADVL>) if; you are N Ill and found sentnece initially. First one to your right is a clause.


* **<advlPoEOS** (@<ADVL) for Po; if you are found at the very end of a sentence. A mainverb is needed to the right though.



* **cleanupILL<advl** (@<ADVL) for N Ill if; there are no boundarysymbols to your left, if you arent already @N< OR @APP-N<, and no mainverb is to yor left.











* **<opredAAcc** (@<OPRED) for A Acc; if an other accusative to the left, and a transtive verb to the left of it. OR: if a transitive verb to the left, and an accusative to the left of it.


### sma object









* **<advlEss** (@<ADVL) for ESS-ADVL if; FMAINV to the left
* **<spredEss** (@<SPRED) for N Ess if; FMAINV to the left is intransitive or bargat





## SUBJ MAPPING - leftovers

## OBJ MAPPING - leftovers


## HNOUN MAPPING
















* * *
<small>This (part of) documentation was generated from [../src/cg3/functions.cg3](http://github.com/giellalt/lang-fro/blob/main/../src/cg3/functions.cg3)</small>=================================== !
The Old French morphophonological/twolc rules file !
=================================== !
















{T}+s and s{T}+s become z



p, f, c, b, and v disappear before inflectional -s
FIXME: change to labials + c





NASAL ALTERATIONS












Silent t and d




Palatalized vowels











Ordinals















































* * *
<small>This (part of) documentation was generated from [../src/fst/phonology.twolc](http://github.com/giellalt/lang-fro/blob/main/../src/fst/phonology.twolc)</small>
General features

Noun Features

Verb Features

Article Features

Pronoun Features

Adverb Features

Adjective Features

Conjunction Features


Numeral Features

Interjection Features

Archiphonemes


* * *
<small>This (part of) documentation was generated from [../src/fst/root.lexc](http://github.com/giellalt/lang-fro/blob/main/../src/fst/root.lexc)</small>Verb Inflection





































































































































































































































































*-er_verbs examples:*
* *durer:* `durer+V+Inf`
* *dur:* `durer+V+1s+Pres+Ind`
* *durat:* `durer+V+3s+Perf+Ind`
* *dura:* `durer+V+3s+Perf+Ind`
* *durerons:* `durer+V+1p+Fut+Ind`
* *dure:* `durer+V+2s+Pres+Imp`


*-ier_verbs examples:*
* *aidier:* `aidier+V+Inf`
* *aidastes:* `aidier+V+2p+Perf+Ind`
* *aidoit:* `aidier+V+3s+Ipfv+Ind`
* *aideit:* `aidier+V+3s+Ipfv+Ind`
* *aida:* `aidier+V+3s+Perf+Ind`
* *aidat:* `aidier+V+3s+Perf+Ind`
* *aidierons:* `aidier+V+1p+Fut+Ind`
* *aidieront:* `aidier+V+3p+Fut+Ind`
* *aidasse:* `aidier+V+1s+Ipfv+Sbjv`


*-ir_verbs examples:*
* *choisir:* `choisir+V+Inf`
* *choisis:* `choisir+V+1s+Pres+Ind`
* *choisis:* `choisir+V+2s+Pres+Ind`
* *choisis:* `choisir+V+2s+Perf+Ind`
* *choisirez:* `choisir+V+2p+Fut+Ind`
* *choisireiz:* `choisir+V+2p+Fut+Ind`
* *choisiroiz:* `choisir+V+2p+Fut+Ind`
* *choisireie:* `choisir+V+1s+Pres+Cond`
* *choisiroie:* `choisir+V+1s+Pres+Cond`
* *choisist:* `choisir+V+3s+Ipfv+Sbjv`
* *choisist:* `choisir+V+3s+Pres+Ind`


*-re_verbs examples:*
* *perdre:* `perdre+V+Inf`
* *perds:* `perdre+V+2s+Pres+Ind`
* *perdrons:* `perdre+V+1p+Fut+Ind`
* *perdreie:* `perdre+V+1s+Pres+Cond`
* *perdroie:* `perdre+V+1s+Pres+Cond`
* *perdu:* `perdre+V+Part+Past+Masc+Obl+Sg`
* *perdu:* `perdre+V+Part+Past+Masc+Nom+Pl`
* *perdust:* `perdre+V+3s+Ipfv+Sbjv`
* *perduxt:* `perdre+V+3s+Ipfv+Sbjv`
* *perdxt:* `perdre+V+3s+Ipfv+Sbjv`
* *perdu:* `perdre+V+3s+Perf+Ind`
* *perdut:* `perdre+V+3s+Perf+Ind`


*misc_verbs examples:*
* *aveir:* `avoir+V+Inf`
* *avoir:* `avoir+V+Inf`
* *escrivant:* `escrire+V+Part+Pres+Masc+Obl+Sg`
* *escrivant:* `escrire+V+Part+Pres+Masc+Nom+Pl`
* *escrivant:* `escrire+V+Part+Pres+Fem+Nom+Sg`
* *escrivant:* `escrire+V+Part+Pres+Fem+Obl+Sg`
* *escrivans:* `escrire+V+Part+Pres+Fem+Nom+Sg`
* *escrivanz:* `escrire+V+Part+Pres+Fem+Nom+Sg`

* * *
<small>This (part of) documentation was generated from [../src/fst/affixes/verbs.lexc](http://github.com/giellalt/lang-fro/blob/main/../src/fst/affixes/verbs.lexc)</small>Noun inflection
The Old French language nouns inflect in cases.































*nouns examples:*
* *fille:* `fille+N+Fem+Nom+Sg`
* *file:* `fille+N+Fem+Nom+Sg`
* *fille:* `fille+N+Fem+Obl+Sg`
* *file:* `fille+N+Fem+Obl+Sg`
* *filles:* `fille+N+Fem+Nom+Pl`
* *files:* `fille+N+Fem+Nom+Pl`
* *filles:* `fille+N+Fem+Obl+Pl`
* *files:* `fille+N+Fem+Obl+Pl`
* *Alemaigne:* `Alemaigne+N+Prop+Fem+Nom+Sg`
* *Alemaigne:* `Alemaigne+N+Prop+Fem+Obl+Sg`
* *Alemaigne:* `Alemaigne+N+Prop+Fem+Nom+Pl`
* *Alemaigne:* `Alemaigne+N+Prop+Fem+Obl+Pl`
* *Alamaigne:* `Alemaigne+N+Prop+Fem+Nom+Sg`
* *Alamaigne:* `Alemaigne+N+Prop+Fem+Obl+Sg`
* *Alamaigne:* `Alemaigne+N+Prop+Fem+Nom+Pl`
* *Alamaigne:* `Alemaigne+N+Prop+Fem+Obl+Pl`
* *Gieffroy:* `Gieffroy+N+Prop+Masc+Nom+Sg`
* *Gieffroy:* `Gieffroy+N+Prop+Masc+Obl+Sg`
* *Gieffroy:* `Gieffroy+N+Prop+Masc+Nom+Pl`
* *Gieffroy:* `Gieffroy+N+Prop+Masc+Obl+Pl`
* *lei:* `lei+N+Fem+Nom+Sg`
* *lei:* `lei+N+Fem+Obl+Sg`
* *ley:* `lei+N+Fem+Nom+Sg`
* *ley:* `lei+N+Fem+Obl+Sg`
* *leis:* `lei+N+Fem+Nom+Pl`
* *leis:* `lei+N+Fem+Obl+Pl`
* *loi:* `lei+N+Fem+Nom+Sg`
* *loi:* `lei+N+Fem+Obl+Sg`
* *loy:* `lei+N+Fem+Nom+Sg`
* *loy:* `lei+N+Fem+Obl+Sg`
* *lois:* `lei+N+Fem+Nom+Pl`
* *lois:* `lei+N+Fem+Obl+Pl`
* *termes:* `terme+N+Masc+Nom+Sg`
* *terme:* `terme+N+Masc+Obl+Sg`
* *terme:* `terme+N+Masc+Nom+Pl`
* *termes:* `terme+N+Masc+Obl+Pl`
* *vespre:* `vespre+N+Masc+Nom+Sg`
* *vespre:* `vespre+N+Masc+Obl+Sg`
* *vespre:* `vespre+N+Masc+Nom+Pl`
* *vespres:* `vespre+N+Masc+Obl+Pl`
* *ancestre:* `ancessor+N+Masc+Nom+Sg`
* *ancessor:* `ancessor+N+Masc+Obl+Sg`
* *ancessor:* `ancessor+N+Masc+Nom+Pl`
* *ancessors:* `ancessor+N+Masc+Obl+Pl`
* *bers:* `bers+N+Masc+Nom+Sg`
* *bers:* `bers+N+Masc+Obl+Sg`
* *bers:* `bers+N+Masc+Nom+Pl`
* *bers:* `bers+N+Masc+Obl+Pl`
* *cortiers:* `cort+N+Agent+Masc+Nom+Sg`
* *corteor:* `cort+N+Agent+Masc+Obl+Sg`
* *courteor:* `cort+N+Agent+Masc+Obl+Sg`
* *courtiers:* `cort+N+Agent+Masc+Nom+Sg`
* *corteors:* `cort+N+Agent+Masc+Obl+Pl`
* *courteors:* `cort+N+Agent+Masc+Obl+Pl`
* *cortière:* `cort+N+Agent+Fem+Nom+Sg`
* *cortière:* `cort+N+Agent+Fem+Obl+Sg`
* *cortiere:* `cort+N+Agent+Fem+Nom+Sg`
* *cortiere:* `cort+N+Agent+Fem+Obl+Sg`
* *courtière:* `cort+N+Agent+Fem+Nom+Sg`
* *courtière:* `cort+N+Agent+Fem+Obl+Sg`
* *courtiere:* `cort+N+Agent+Fem+Nom+Sg`
* *courtiere:* `cort+N+Agent+Fem+Obl+Sg`


* * *
<small>This (part of) documentation was generated from [../src/fst/affixes/nouns.lexc](http://github.com/giellalt/lang-fro/blob/main/../src/fst/affixes/nouns.lexc)</small>Verbs










































Add: doloir, rire, trover, asseoir
conduire, criembre, tordre
* * *
<small>This (part of) documentation was generated from [../src/fst/stems/verbs.lexc](http://github.com/giellalt/lang-fro/blob/main/../src/fst/stems/verbs.lexc)</small>Nouns












































* * *
<small>This (part of) documentation was generated from [../src/fst/stems/nouns.lexc](http://github.com/giellalt/lang-fro/blob/main/../src/fst/stems/nouns.lexc)</small>


We describe here how abbreviations are in Old French are read out, e.g.
for text-to-speech systems.

For example:

* s.:syntynyt # ;  
* os.:omaa% sukua # ;  
* v.:vuosi # ;  
* v.:vuonna # ;  
* esim.:esimerkki # ; 
* esim.:esimerkiksi # ; 


* * *
<small>This (part of) documentation was generated from [../src/transcriptions/transcriptor-abbrevs2text.lexc](http://github.com/giellalt/lang-fro/blob/main/../src/transcriptions/transcriptor-abbrevs2text.lexc)</small>















































% komma% :,      Root ;
% tjuohkkis% :%. Root ;
% kolon% :%:     Root ;
% sárggis% :%-   Root ; 
% násti% :%*     Root ; 

* * *
<small>This (part of) documentation was generated from [../src/transcriptions/transcriptor-numbers-digit2text.lexc](http://github.com/giellalt/lang-fro/blob/main/../src/transcriptions/transcriptor-numbers-digit2text.lexc)</small>