# SPACY 
## 1.POS Tagging

	Text: The originalword text.
	Lemma: The base form of the word.
	POS: The simple part-of-speech tag.
	Tag: The detailed part-of-speech tag.
	Dep: Syntactic dependency, i.e. the relation between tokens.
	Shape: The word shape - capitalisation, punctuation, digits.
	is_alpha: Is the token an alpha character?
	is_stop: Is the token part of a stop list, i.e. the most common words of the language.

## 2.Dependency Parse
This parser powers the sentence boundary detection, and lets you iterate over base noun phrases or chunks.

## 3.Noun chunks
Noun chunks are base noun phrases, that have a noun as their head.Noun chunks can be described as nounplus the words describing the noun.

	Text: The Original noun chunk text.
	Root text: The original text of the word connecting the nounchunk to the rest of the parse.
	Root dep: Dependency relation connecting the root to its head.
	Root head text: The text of the root tokens head

## 4.Navigating the parse tree 
Head and child terms are used to describe the words connected by a single arc in the dependency tree.

	Text: The original token text.
	Dep: The syntactic relation connecting child to head.
	Head text: The original text of the token head.
	Head POS: The part-of-speech tag of the token head.
	Children: The immediate syntactic dependents of the token. 

## 5.Named Entity Recognition 
A named entity is a real-world object thats assigned a name.

	Text: The original entity text.
	Start: Index of start of entity in the Doc.
	End: Index of end of entity in the Doc.
	Label: Entity label, i.e. type.


## 6.Tokenization 
Tokenization is the task of splitting a text into meaningful segments called tokens.
	
	Text: The original token text.

## 7.Sentence Segmentation 
It is used to determine sentence boundaries.

	Text: The original sentence text.

## 8.Rule-based matching
This operates over tokens, similar to regular expressions.The rules can refer to token annotations and flags.