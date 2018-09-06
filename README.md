###### sent_splitter optimized for biomedical texts, It reads a text and splits it into sentences by inserting line breaks.
 
 **Classification model**
sent_splitter detects candidate positions for splitting using selected delimiters: periods, commas, single/double quotation marks, right parentheses, etc. Then, it classifies whether each candidate really splits the sentence or not.

## Classifier Features
*Delimiters of the candidate point
*Previous/Next words
*Previous/Next words deleted brackets, commas, etc. (word2)
*Capitalization of first/other character(s) of the next word
*Existence of capitals in the previous word
*Existence of numbers in prev/next words
*Existence of brackets/quotations in prev/next words
*Existence of comma in prev/next words
*Combination feature of previous word & delimiter
*Combination feature of previous word2, delimiter & next word2

## How to use
./sed_sentence_chunker
