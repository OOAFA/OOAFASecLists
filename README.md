# OOAFASecLists

A collection of useful lists in various translations.

## Discovery - DNS

DNSLeak_ru_zone.txt - DNS Research reference: [RussiaDNSLeak](https://github.com/mandatoryprogrammer/RussiaDNSLeak).

ru_sublazerwlst: [sublazerwlst](https://github.com/sharsi1/sublazerwlst).

Russian and Cyrillic Domains on nic.ru: [nic.ru domains](https://www.nic.ru/en/catalog/domains/russian-and-cyrillic/).

## Discovery - Web-Content

How we translated the wordlists:

1. Used an AI model from huggingface.co called "glazzova/ml_translation_model1".  This model was fine tuned from another model from Helsinki.  
2. Batched up the english text into comma separated batches of data around 460 chars in length.  Think of them as word lists.
3. Translated each word list into RU through the AI model application on a GPU enabled machine.
4. FOR EACH word in the resulting list....
4.1 If the word did not translate into RU, or there was a space in the end result, the translation was rejected. I used a latin-1 encoder to determine if the word was pure latin chars or NOT.. if NOT latin chars, I consider it to be RU.
4.2 Checked if the word was in the "already translated" list.  If not, wrote the new word to disk as a translated entity.

## Usernames

xx_shodan_squeegee_usernames.txt - Country specific shodan RDP scraping results.

## Passwords

xato converted.

Coming soon .. Russian per-TLD Public Data Breach Lists