Style Manual
============
The site generally follows the Oxford style, with exceptions.

As with unit testing for code, a good habit is to add an entry for each problem you run into.

Oxford Style Examples
---------------------
An excerpt from some of the [examples][oed]:

 Right                | Wrong
:---------------------|:---------------------------------------------
 J R R Tolkien        | J.R.R. Tolkien, J. R. R. Tolkien
 Ampersands in names  | Ampersands anywhere else
 etc, ie, eg          | etc., i.e., e.g.
 ibid                 | ibid.
 90s, CDs, dos, donts | Plural apostrophes, except for disambiguation

Characters
----------
 Right   | Wrong
:--------|:-------------------------
 æ       | ae
 ø       | oe, o
 å       | aa
 “Quote” | ”Quote”, ‘Quote’, «Quote»

### Dashes ###

Em dashes, —, are denoted by three dashes in markup, `---`, and are used without empty space around them.

En dashes, –, are for number and date ranges and denoted by two dashes, `--`.

Right               | Wrong
:-------------------|:--------------------
 Good job---I think | Good job --- I think, Good job-- (...)

No eccentric diareses belong in this style guide, but do use hyphens for prefixes that cause ambiguity and poor readability (“pro-zoo”) or precede numbers and proper names (“pre-2000”, “pre-Orwell”).

Markdown
--------
 Right               | Wrong
:--------------------|:---------------
`### Header 1 ###`   | `### Header 1`, `## Header 1 ##`, `# Header 1 #`
`#### Header 2 ####` | `#### Header 2`

General
-------
 Right               | Wrong
:--------------------|:----------------
 Hafnia Times        | The Hafnia Times
 Front page          | Frontpage

Quotations
----------
Use an ellipsis wrapped in parentheses, `(...)`, when sections of an excerpt are removed.

Any modification to the original quote (short of quote marks and dashes) must be denoted with square brackes, `[]`.

Numbers
-------
 Right                         | Wrong
:------------------------------|:------------------
 1,000,000                     | 1000000
 10,000 Danish kroner ($1,702) | 10,000 kr., 10,000 crowns, 10,000,-
 $1,702                        | 1.702 U.S. dollars
 100M                          | 100m, 100mn, 100 M
 100B                          | 100b, 100bn, 100 B
 two                           | 2
 nine, ten, 11, 12             | nine, ten, eleven, twelve
 second                        | 2nd
 ninth, tenth, 11th, 12th      | 9th, 10th, 11th, 12th
 100 cm, 1 m                   | 100cm, 1m
 10%                           | 10 %, 10 per cent, 10 percent

When listing prices and valuations, use the shortform, i.e. $1,500 and 1,500 Danish kroner. Shorten large numbers with M and B, but not k.

Time and Date
-------------
 Right    | Wrong
:---------|:----------------
 April 10 | 10 April, 10th of April
 15:00    | 3:00 PM
 2010–15  | 2010–2015, 2010–5

Media
-----
 Right           | Wrong
:----------------|:-------------------------------
 TV 2            | TV2
 DR              | Danish Radio, Denmark’s Radio
 Berlingske Tidende | Berlingske
 Weekendavisen   | WeekendAvisen
 BuzzFeed        | Buzzfeed
 Radio24syv      | Radio24Syv, radio24syv
 Jyllands-Posten | Jyllands Posten, JyllandsPosten

Parties
-------
 Right                                | Shorthand            | Wrong
:-------------------------------------|:---------------------|:---------------------------------
 [The Danish Social Democrats][a]     | The Social Democrats | (Without definite article)
 [The Danish Social-Liberal Party][b] | The Social Liberals  | (Without definite article)
  Socialist People’s Party            | -                    | (With definite article)
  The Conservative People’s Party     | The Conservatives    | (Without definite article)
  Liberal Alliance                    | -                    | (With definite article)
 [Danish People’s Party][o]           | DPP                  | (With definite article)
 [Venstre][v]                         | -                    | Venstre, Liberal Party of Denmark
 [The Red-Green Alliance][ø]          | The Red-Greens       | (Without definite article)

Politicians
-----------
 Right                   | Shorthand        | Wrong
:------------------------|:-----------------|:-----------------------
 Helle Thorning-Schmidt  | Thorning-Schmidt | Helle Thorning Schmidt
 Kristian Thulesen Dahl  | Dahl             | Kristian Thulesen-Dahl
 Margrethe Vestager      | Vestager         | Magrethe Vestager
 Pia Olsen Dyhr          | Dyhr             | Pia Olsen-Dyhr
 Johanne Schmidt-Nielsen | Schmidt-Nielsen  | Johanne Schmidt Nielsen
 Pia Kjærsgaard          | Kjærsgaard       | Pia Kærsgaard
 Lars Løkke Rasmussen    | Rasmussen        | Lars Løkke-Rasmussen

Technology
----------
 Right                      | Wrong
:---------------------------|:------------
 ride-booking, ride-hailing | ride-sharing

Capitalization
--------------
 Right                        | Wrong
:-----------------------------|:---------------------
 Prime Minister such-and-such | (Lowercase)
 The prime minister           | (Uppercase)
 President such-and-such      | (Lowercase)
 The president                | (Uppercase)
 Pope such-and-such           | (Lowercase)
 The pope                     | (Uppercase)
 Democrat(ic), Republican, Conservative | (Lowercase)
 Muslim, Jew(ish), Christian  | (Lowercase)
 secretary general | (Uppercase)

Companies
---------
 Right | Wrong
:------|:-----
 LEGO  | Lego

Finance
-------
 Right          | Wrong
:---------------|:-----
 Nationalbanken, Denmark’s Nationalbank | The Danish (...), The Central Bank of Denmark
 Riksbanken, Sweden’s Riksbank          | The Swedish (...), The Central Bank of Sweden
 ECB | The European Central Bank, Europe’s Central Bank

Currency
--------
All currencies are uncapitalized.

 Right                     | Wrong
:--------------------------|:-----
 (Danish) krone(r), DKK    | (Danish) kroners
 (Norwegian) krone(r), NOK | (Danish) kroners
 (Swedish) krona/-or, SEK  | (Swedish) kroner, (Swedish), kronors
 (Swiss) franc(s), CHF     |
 euro           | euros
 (U.S.) dollars | (U.S.) Dollars

Using the currency symbols is preferable; “$1,500”, “1,500 kr.” vs. “1,500 U.S. dollars”, “1,500 Danisk kroner”.

Use the unabbreviated currency the first time, and the abbreviation for repeat uses.

Acronyms/Abbreviations
----------------------
Use Markdown’s [abbreviation syntax][abbr] in the following cases:

 Shorthand  | Full Word
:-----------|:------------------------------------
 MEP        | Member(s) of the European Parliament
 MP         | Member(s) of parliament

Links
------
- [GLAAD Media Reference Guide on Transgender Issues][transgender]


[oed]:  http://www.ox.ac.uk/public-affairs/style-guide
[abbr]: https://michelf.ca/projects/php-markdown/extra/#abbr

[a]: http://socialdemokraterne.dk/default.aspx?site=english
[b]: http://www.radikale.dk/english
[o]: http://www.danskfolkeparti.dk/The_Party_Program_of_the_Danish_Peoples_Party
[v]: http://www.venstre.dk/servicemenu/english/facts-about-venstre/
[ø]: http://enhedslisten.dk/content/red-green-alliance

[transgender]: http://www.glaad.org/reference/transgender
