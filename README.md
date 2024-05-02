# OOAFASecLists

A collection of useful lists in various translations.

## Discovery - DNS

DNSLeak_ru_zone.txt - DNS Research reference: [RussiaDNSLeak](https://github.com/mandatoryprogrammer/RussiaDNSLeak).

ru_sublazerwlst: [sublazerwlst](https://github.com/sharsi1/sublazerwlst).

Russian and Cyrillic Domains on nic.ru: [nic.ru domains](https://www.nic.ru/en/catalog/domains/russian-and-cyrillic/).

## Discovery - Web-Content

How we translated the wordlists:

1. Using Hugging Face, we located several different models for language translation. Some examples as follows:
* Helsinki-NLP/opus-mt-en-uk: english to ukranian
* Helsinki-NLP/opus-mt-en-zh: english to chinese
* Helsinki-NLP/opus-mt-en-ar: english to arabic
2. Each word from fed in batches to the translator pipeline after initializing the pre-trained model.
3. For each translated word, if there was no specific translation, or a space existed then the word was rejected.
4. For each translated word, if the result was only in the "latin" alphabet, then it was rejected as "not translated".
5. The translated word was then written to disk.
* Note: for performance improvements, the translation was executed on a Nvidia/Cuda enabled RTX-3070 GPU card.

## Usernames

xx_shodan_squeegee_usernames.txt - Country specific shodan RDP scraping results.

## Passwords

xato converted.

Coming soon .. per-TLD and language public data breach lists
