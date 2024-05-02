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
3. A translated word was rejected if it was a zero length string, contained a space character, was not translated (English), or was a duplicate of a previously translated word.
* Note: for performance improvements, the translation was executed on a Nvidia/Cuda enabled RTX-3070 GPU card.

## Usernames

xx_shodan_squeegee_usernames.txt - Country specific shodan RDP scraping results.

## Passwords

xato converted.

Coming soon .. per-TLD and language public data breach lists
