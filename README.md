# Books3Info
Intended for data and information related to the Books3 dataset included as part of The Pile, and used to train Meta's LLaMA among others. Right now there are two files included here: 

-  **Books2_ISBNs.txt**, and
-  **filenames.txt**

### Books2_ISBNS
This is a list of some 125,000 ISBN-13s extracted from the 197,500 txt files contained in the Books3 dataset, consistingly of (mostly) pirated ebooks. The ISBN list may include both print- and e-book ISBNs of the same title, depending on the policy of publishers of including ISBNs in their ebook files. ISBNs are presented as extracted, and not always in canonical form with hyphens included (in the right places). They are presented exactly as they appeared in the txt files that were part of Books3, with no further processing.

Why such a difference between number of books and number of ISBN-13s? 
- my parsing may have failed to pick them up. I used the following regex to search - '([0-9][0-9-X ]{10,16})' - I am sure this can be improved upon
- some books may include only ISBN-10s which I did not try to parse
- some books do not incude ISBNs in the relevant file. Some may be self-published titles that made their way into the Bibliotik torrent. In other cases ISBNs may have been stripped by some other process. By way of example, a few such titles include:
- - C. A. Gray - Intangible.epub, a Smashwords edition (does that mean it is duplicated in the BooksCorpus dataset which is around 11,000 novels from Smashwords?)
- - 5 Minutes to Stress Relief How to Release Fear, Worry, and Doubt Instantly - Lauren Miller.epub, self-published
- - C_Pocket_Reference.epub, a 2009 O'Reilly Media, Inc publication with no ISBN included
- - Cajun Greats_ 175 Delicious Cajun Recipes - Jo Franks.epub - self-published
- - and etc

Note that even the self-published titles without ISBN usually contain a copyright statement reserving all rights. 

### filenames

This is just one big list of the names of the text files that make up the Books3 database, as originally organised in the Books3 dataset. The pirates didn't follow a naming convention, so this is a little chaotic. The most common pattern is "Author Name - Title" but it is far from consistent. Sometimes the file name also includes language and date of publication, even publisher name. Still, this may be helpful.

If you would like more information on copyright questions around the Large Language Models you are welcome to the compiler's newsletter at https://aicopyright.substack.com.
