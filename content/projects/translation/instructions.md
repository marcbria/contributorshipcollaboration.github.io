---
title: Instructions for Contributors
description: Guidelines for contributing to the translations.
order: 2
layout: "translation/single"
---


## Contributing to translations 

Anyone fluent in a language not already translated can help provide a new translation, or propose a change to an existing translation.

Before starting on a new translation:

* [Check the current status]() of translation for your language.
* Fill out [our Google Form](https://docs.google.com/forms/d/e/1FAIpQLSfdhqlnk4sw61MkkDuufZyqO1SKmnp--QE6vEG1_7qnP9MzJg/viewform?usp=sf_link) so we have a record of your interest and potentially to help match you with another translator or project contributor.
* Follow the instructions in the below [translation section](#-Creating-a-translation).

Contributors will be recognized in that their names will appear in the attribution for the translation they helped create. For example, see the [draft human-readable page for German](https://github.com/contributorshipcollaboration/credit-translation/blob/main/md_files/credit_translation_de.md).


## Contributing to other facets of the project (we'd love your help!)

* Code: check the Github issues or email us
* Outreach and implementation 
 * Contact scientific societies and scientific publishers who publish in these languages
* Help us organise a hackathon ad hoc or at a scientific conference

## Creating a translation

*  We have created a Google Sheet for entering your translation work and seeing how others did it. Contact us for access to the Google Sheet.
* First, one speaker fluent in both languages translates the English into the target language and enters that on the Google Sheet. 
* A second speaker, ideally one not familiar with CRediT, back-translates the translation into English.
* Feel free to use Google Translate to assist, just don't rely on it, for example don't use it for both the forward and back-translation.
* Discrepancies between the original English and the back-translated English can tip one off to parts of the translation that deserve attention, where one should consider alternative phrasings. So, the two speakers confer and resolve any discrepancies.
* To make your translation machine-readable, you must create a JSON file, following the format of the [schema](). See instructions below.
 * To see if a .json file already exists, look [here]() for a file with the [two-letter abbreviation](https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes) for your language.
  
### If a .json file for your language does NOT already exist:

Download one of the existing JSON files, such as [the German one]() and change all the German text to your target language. Then send it to us.

### If a .json for your language DOES already exist: 

* To edit the file, click on the pencil icon. Insert the content for your translation. See [the German one]() for an example.
* So that the Github repository gets updated, create a pull request by clicking on BLAH BLAH
* Don't forget to add information about how you did the translation in the "translationProcedure" string of the .json file, here is an example: "TL, CJ, and HH are all native speakers of German. A first version by TL existed for some time. CJ introduced an additional translation draft. TL and CJ merged the few differences between the two versions favoring broader (in the sense of suitability for as many disciplines and working environments as possible) translations. The final translation was then back-translated by HH, and finally approved by all parties." In this case, two forward translations were created, yielding discrepancies that surfaced parts to attend more to. As described in the above [Creating a translation](#-Creating-a-translation) section, however, another way to do that is to look at discrepancies highlighted by doing a back translation.
* Validate that your edits have not messed up the formatting by entering both the [schema]() and your file at [https://www.jsonschemavalidator.net/](https://www.jsonschemavalidator.net/). This checks for most formatting errors.
* Generate a pull request

### Validate your .json file

* Validate that your edits have not messed up the JSON file formatting by entering both the [schema]() and your file at [https://www.jsonschemavalidator.net/](https://www.jsonschemavalidator.net/).

### Send us your .json file, or upload it yourself

* If you're not familiar with Github, send us the .json file
* If you're familiar with Github,
 * Create the json file if it doesn't already exist
 * Create the pull request