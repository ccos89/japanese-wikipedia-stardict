# Japanese Wikipedia Stardict for Ereaders

A dictionary converting Japanese Wikipedia's short abstracts of articles as consolidated by [DBPedia](https://dbpedia.org/) in the Stardict format. For use by KOReader and other eReaders or by [GoldenDict](https://github.com/goldendict/goldendict) on PC.

Inspired by [Wikipedia For Yomitan/Yomichan](https://github.com/MarvNC/wikipedia-yomitan) where MarvNC has made a much prettier version of a Japanese Wikipedia dictionary but which does not work with eReaders.  Contrary to their version, I have stripped out the URLs for the articles as following the links does not make sense in the context of most ereaders.  

&#11088; Although KOreader supports Wikipedia lookups natively and other eReaders may do the same, that information would typically be difficult or impossible to export to a flash card/vocab builder tool.  With this dictionary the Wikipedia abstract can be saved as a "definition" on an Anki card through the excellent [anki.koplugin](https://github.com/Ajatt-Tools/anki.koplugin) or a comparable program for another eReader.

&#128269; The dictionary is searchable by both the kanji/katakana/stylized version of the word and the hiragana reading.  The definition it displays is the abstract (the short text summary at the top of the Wikipedia article before it goes into detailed information) which is usually a sentence to a single paragraph long.  

&#x1F4D6; There are about 1.2 million entries in the dictionary so it is quite large but I have had no issues running it on a Kobo Forma which has quite modest processing power and where I am also running about 20 other Stardicts, so I would guess this should work on any relatively modern eReader that supports the format.

## Download/Install

Clone or download the repo from Github.  Move the whole "JaWikiStar" folder or just all the files within to the directory where you can install custom dictionaries in your ereader/Stardict compatible desktop program.  

For example, on KOReader, move the whole folder to \koreader\data\dict.  

To uninstall, simply delete the folder from where you put it.

&#x1F4CC; Please note, I have only tested the dictionary on GoldenDict and KOReader as those are the programs that are relevant to me to use. YMMV with other eReaders, although I don't see why it wouldn't work.

## Usage Notes

Because the article names (i.e., the dictionary headwords) are often long and for the lookup to work correctly the whole string of kanji or kana characters needs to be selected, if you are not getting the results you want you should try tweaking the string lookup length for the Japanese language support in KOReader or manually select the whole string you are trying to look up if the ereader is only selecting a single word or portion of the string.

If you want to change the name of the dictionary as it appears in your eReader, you can edit the .ifo file to change bookname= to the desired name for the dictionary (default: Japanese Wikipedia Abstracts).

## Updates

I will try to update this project periodically to incorporate new edits to Wikipedia as they are collected by DBPedia.  I don't have a set timeline on when that will occur.

**LAST UPDATED: 1-24-2024**

## Screenshots

GoldenDict on PC
![Dictionary Lookup on GoldenDict](https://github.com/ccos89/japanese-wikipedia-stardict/assets/133320139/cc4ed121-7a62-4d95-803c-8bb04dd2191c)

KOReader on Kobo Forma
![Dictionary Lookup on Kobo Forma](https://github.com/ccos89/japanese-wikipedia-stardict/assets/133320139/21260754-84f9-486d-b52f-4e78ccbc865c)

## Info and Licensing

This dictionary was built using [PyGlossary](https://github.com/ilius/pyglossary) and uses data from [Wikipedia.jp](https://wikipedia.jp) which is owned by the [Wikimedia Foundation](https://wikimediafoundation.org/) and which was scraped and compiled by [DBPedia](https://dbpedia.org/).

This data is distributed under the CC0-1.0 license.
