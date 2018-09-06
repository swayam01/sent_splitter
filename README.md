###### sent_splitter optimized for biomedical texts, It reads a text and splits it into sentences by inserting line breaks.
 
 **Classification model rule based** <br />
sent_splitter detects candidate positions for splitting using selected delimiters: periods, commas, single/double quotation marks, right parentheses, etc. Then, it classifies whether each candidate really splits the sentence or not.

## Classifier Features <br />
*Delimiters of the candidate point <br />
*Previous/Next words <br />
*Previous/Next words deleted brackets, commas, etc. (word2) <br />
*Capitalization of first/other character(s) of the next word <br />
*Existence of capitals in the previous word <br />
*Existence of numbers in prev/next words <br />
*Existence of brackets/quotations in prev/next words <br />
*Existence of comma in prev/next words <br />
*Combination feature of previous word & delimiter <br />
*Combination feature of previous word2, delimiter & next word2 <br />

## How to use <br />
./sed_sentence_chunker
