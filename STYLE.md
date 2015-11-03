Style Manual
============
The site generally follows the Oxford style, with exceptions.

As with unit testing for code, a good habit is to add an entry for each problem you run into.

Oxford Style Examples
---------------------
An excerpt from some of the [examples][oed]:

 Right                | Wrong
:---------------------|:---------------------------------------------
 J R R Tolkien        | J.R.R., J. R. R., JRR
 Ampersands in names  | Ampersands anywhere else
 etc, ie, eg, vs      | etc., i.e., e.g., vs.
 UK, US               | U.K., U.S.
 Mr, Ms, Dr           | Mr., Ms., Mrs., Dr.
 ibid                 | ibid.
 90s, CDs, dos, donts | Plural apostrophes, except for disambiguation
 Jr, Sr (w/o comma)   | Jr., Sr. (w/ comma)

Formatting
----------
For purposes for retention and readability:

* Use `**strong**` for names, which improves retention
    - Consider using it for other larger concepts and entities
* Prioritize vertical lists over a comma-separated recital in a sentence
    - Do not capitalize one- or two-word list items
    - Do not end them in trailing commas
    - Only add a trailing period for longer sentences

These guidelines may seem weird to people from a print background, but should be sensible to people from a web background; remember the value of explicit, semantic web formatting to people with visual disabilities—some of whom rely screenshotreaders to read online articles.

The guidelines urge that you *prioritize* vertical lists; in the cases where you deem that an in-line (horizontal) list is sufficient, consider auxiliary enumeration like

> (1) apples, (2) oranges, (3) pineapples

This is not for accessibility, but readability retention.

Consider this [article on memorization][ndarville.github.io] and how the formatting contributes to the understanding and retention of the information.

### Links ###

Wrap links to accommodate web standards and people with screen readers. From [ndarville/style/html][]:

> In accordance with [HTML Techniques for Web Content Accessibility Guidelines 1.0, Section 6.1][link-text].
>
> **Do not** use `click here` as link text.
>
> **Do not** use call-to-action verbs like `go to our page`.
>
> Use the page or content your are linking to as the text instead.
>
> #### [Bad] ####
>
>> [Click here] to visit GitHub.
>
> #### [Also bad] ####
>
>> Click here to [visit GitHub].
>
> #### [Good] ####
>
>> Click here to visit [GitHub].

Feel free to phrase the link’s surrounding prose as you please.

It may feel like you have to change your writing style to adapt to writing for a digital publication. This is true, but it is important to remember that your articles will be read both as-is, as well as on screenreaders for those of your readers with disabilities who rely on them.

Adapting your prose to people with screenreaders differs little from making your visual media accessible to colour-blind readers, and your auditory media accessible to people hard of hearing.

### Important Distinctions ###

* “among” vs “between”
* “compare with” vs “compare to”

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

 Right              | Wrong
:-------------------|:--------------------
 Good job---I think | Good job --- I think, Good job--(...)

No eccentric diareses belong in this style guide, but do use hyphens for prefixes that cause ambiguity and poor readability (“pro-zoo”) or precede numbers and proper names (“pre-2000”, “pre-Orwell”).

#### Hyphenated Compound Modifiers ####

Only hyphenate [compound modifiers][] for disambiguation, not too dissimilarly to the Oxford Comma. Adverbs are rarely, if ever, cause for ambiguity—especialy those ending in -ly—so “wildly popular app” should go unhyphenated.

This generally applies to all hyphenation; “when in doubt, leave it out”.

#### Abbreviations ####

Refrain from abbreviations for common words and phrases (eg, ie, etc) as often as possible. Acronyms are of course acceptable for the most part, as long as the full name is commonly known (NATO, US, GOP).

Specificity
-----------
Reduce vagueness and passive voice as much as possible. This [McSweeney’s article][mcs] goes into more detail with examples.

Gendered Terminology
--------------------
Avoid compounds with “man” as much as possible. One example comes from [NASA's style guide][nasa]:

> **Manned Space Program vs. Human Space Program:**
>
> All references referring to the space program should be non-gender specific (e.g. human, piloted, un-piloted, robotic). The exception to the rule is when referring to the Manned Spacecraft Center, the predecessor to the Johnson Space Center in Houston, or any other official program name or title that included "manned" (e.g. Associate Administrator for Manned Spaceflight).

Generally, positions of leadership tend to be gendered with “-man”. In those cases, use “-person” or, at least, “-woman” depending on whether the former sounds off. For instance, use either “chairwoman” or just “chair” instead of “chairman”, when the position is held by a woman.

Markdown
--------
 Right                | Wrong
:---------------------|:---------------
 `### Header 1 ###`   | `### Header 1`, `## Header 1 ##`, `# Header 1 #`
 `#### Header 2 ####` | `#### Header 2`
 `* List item`        | `-`, `+`
 `- Sublist item`     | `*`, `+`

General
-------
 Right                 | Wrong
:----------------------|:--------------------
 -ize, -yze, -ization  | -ise, -yse, -isation
 -eable                | -able
 10:00, 10 AM/PM       | 10 am/pm, 10AM/PM
 ceasefire             | cease-fire
 comprise              | comprised of
 e-mail                | email
 front page            | frontpage
 Hafnia Times          | The Hafnia Times
 invitation            | invite
 Islamic State, IS(IS) | ISIL, Daesh
 Koran                 | Quran, Qu’ran
 learn/-ed/-t          | /-ed/-ed, /-t/-t
 median income         | middle income
 NATO                  | Nato
 no one                | no-one
 revise                | revize
 sex worker            | prostitute, hooker
 sharing economy       | on-demand industry
 slaveholder           | slave owner
 use                   | usage

### Danish Stuff ###

 Right       | Wrong
:------------|:-----
 LEGO        | Lego
 LEGO bricks | LEGOs

### Male and Female ###

* “female” is only to be used as an adjective
    - same for “male”
* “woman” is only to be used as a substantive

When the gender is unknown, use the pronoun “they”—not “s/he”.

Do not use “Mrs” and “missus”.

### Donts ###

Don’t use these words in general:

* problematic
* racial profiling
* tragedy

#### Specious Geography ####

There is no consensus around the meaning of these geographical terms, so try not to use them:

* Eastern Europe and Eastern-Europeans
* the international community
* the East
* the West(ern World)

You might also reconsider the specificity of such geographies as

* Africa
* Arabic countries
* Asia
* the Middle East

### Nerdy Terms ###

Don’t use these terms without explaining them in context:

* G3, G7, etc
* P5+1

British vs American
-------------------
The differences not supported by this style manual have been omitted.

### Endings ###

 UK    | US  | Examples
:------|:----|:--------------------
 -our  | -or | colour, behaviour
 -re   | -er | centre, theatre
 -ll   | -l  | traveller, cancelled
 -ogue | -og | dialogue, analogue

### Words ###

 UK noun      | UK verb      | US noun      | US verb
:-------------|:-------------|:-------------|:-------------
 defen**c**e  | -d           | defen**s**e  | -d
 licen**c**e  | licen**s**e  | licen**s**e  | licen**s**e
 offen**c**e  | -d           | offen**s**e  | -d
 practi**c**e | practi**s**e | practi**s**e | practi**s**e
 preten**c**e | -d           | preten**s**e | -d

### Others Words ###

* aeroplane vs airplane
* judgement vs judgment (except for legal cases)
* whom vs who

Quotations
----------
Use an ellipsis wrapped in parentheses, `(...)`, when sections of an excerpt are removed.

Any modification to the original quote (short of quote marks and dashes) must be denoted with square brackes, `[]`.

Numbers
-------
 Right                         | Wrong
:------------------------------|:-----------------------------------
 1,000,000                     | 1000000
 10,000 Danish kroner ($1,702) | 10,000 kr., 10,000 crowns, 10,000,-
 $1,702                        | 1,702 US dollars
 100M                          | 100m, 100mn, 100 M
 100B                          | 100b, 100bn, 100 B
 two                           | 2
 nine, ten, 11, 12             | 9, 10, eleven, twelve
 second                        | 2nd
 ninth, tenth, 11th, 12th      | 9th, 10th, eleventh, twelfth
 100 cm, 1 m                   | 100cm, 1m
 100 h, 10 m, 1 s              | 100h, 10m, 1s
 10%                           | 10 %, 10 per cent, 10 percent
 10-year-old                   | 10yo

When listing prices and valuations, use the shortform, i.e. $1,500 and 1,500 Danish kroner. Shorten large numbers with M and B, but not k.

Time and Date
-------------
Use a 24-hour format by default, and only use the 12-hour format when required by verbatim transcriptions and the like.

 Right    | Wrong
:---------|:-----------------------
 April 10 | 10 April, 10th of April
 15:00    | 3:00 PM
 2010–15  | 2010–2015, 2010–5

Media
-----
 Right              | Wrong
:-------------------|:-------------------------------
 BBC                | British Broadcasting
 Berlingske Tidende | Berlingske
 BuzzFeed           | Buzzfeed
 DR                 | Danish Radio, Denmark’s Radio
 Jyllands-Posten    | Jyllands Posten, JyllandsPosten
 Radio24syv         | Radio24Syv, radio24syv
 TV 2               | TV2
 Weekendavisen      | WeekendAvisen

Parties
-------
 Right                                | Shorthand            | Wrong
:-------------------------------------|:---------------------|:-----
 [The Danish Social Democrats][a]     | The Social Democrats | -The
 [The Danish Social-Liberal Party][b] | The Social Liberals  | -The
  Socialist People’s Party            | -                    | +The
  The Conservative People’s Party     | The Conservatives    | -The
  Liberal Alliance                    | -                    | +The
 [Danish People’s Party][o]           | DPP                  | +The
 [Venstre][v], the Liberal Party      | -                    | “Venstre, Liberal Party of Denmark”
 [The Red-Green Alliance][ø]          | The Red-Greens       | -The
  Alternativet                        | The Alternative      | +The

Politicians
-----------
### Danish ###

 Right                   | Shorthand        | Wrong
:------------------------|:-----------------|:------------------
 Helle Thorning-Schmidt  | Thorning-Schmidt | (Unhyphenated)
 Kristian Thulesen Dahl  | Dahl             | (Hyphenated)
 Margrethe Vestager      | Vestager         |  Magrethe Vestager
 Pia Olsen Dyhr          | Dyhr             | (Hyphenated)
 Johanne Schmidt-Nielsen | Schmidt-Nielsen  | (Unhyphenated)
 Pia Kjærsgaard          | Kjærsgaard       |  Pia Kærsgaard
 Lars Løkke Rasmussen    | Rasmussen        | (Hyphenated)

### International ###

 Right            | Shorthand | Wrong
:-----------------|:----------|:-----------------------
 Hillary Clinton  | Clinton   | Hilary Clinton, Hillary

Technology
----------
 Right                      | Wrong
:---------------------------|:------------
 ride-booking, ride-hailing | ride-sharing

* **Broadband** is a minimum speed of 25 Mb/s download and 3 Mb/s upload as [defined by the FCC][broadband].

Capitalization
--------------
 Right                        | Wrong
:-----------------------------|:-----------
 Prime Minister such-and-such | (Lowercase)
 The prime minister           | (Uppercase)
 President such-and-such      | (Lowercase)
 The president                | (Uppercase)
 Pope such-and-such           | (Lowercase)
 The pope                     | (Uppercase)
 Democrat(ic), Republican, Conservative | (Lowercase)
 Muslim, Jew(ish), Christian  | (Lowercase)
 secretary general            | (Uppercase)

Monolithic concepts like “Internet” and “Technology” are capitalized, partly as a deterrent to using them as big, fluffy concepts.

Tweets
------
Tweets for and about a Hafnia Times article should read:

>"Article Title" link [optional Twitter-uploaded image]

Do not use a colon to point towards the link.

Finance
-------
 Right          | Wrong
:---------------|:-----
 Nationalbanken, Denmark’s Nationalbank | The Danish (...), The Central Bank of Denmark
 Riksbanken, Sweden’s Riksbank          | The Swedish (...), The Central Bank of Sweden
 (the) ECB | The European Central Bank, Europe’s Central Bank

Currency
--------
All currencies are uncapitalized.

 Right                     | Wrong
:--------------------------|:------------------------------------
 (Danish) krone(r), DKK    | (Danish) kroners
 (Norwegian) krone(r), NOK | (Danish) kroners
 (Swedish) krona/-or, SEK  | (Swedish) kroner, (Swedish), kronors
 (Swiss) franc(s), CHF     |
  euro                     |  euros
 (US) dollar(s)            | (US) Dollar(s)

Using the currency symbols is preferable; “$1,500”, “1,500 kr.” vs “1,500 US dollars”, “1,500 Danisk kroner”.

Use the unabbreviated currency the first time, and the abbreviation for repeat uses.

Tricky Spellings
----------------
* accommodation
* artis**a**nal
* boycott
* cemet**e**ry
* commission
* committee
* competitive
* embarrass
* graffiti
* ha**r**ass
* millennium
* publicly
* refe**rr**al, -ed, -er
* resuscitate

Typo-prone Words
----------------
* appar**e**ntly
* cumulative
* defin**ite**ly
* occasion
* privilege
* sep**a**rate
* tomorrow
* weird

Common Misconceptions
---------------------
 Right             | Wrong
:------------------|:--------------
 same-sex marriage | gay marriage\*

### Learn the Difference ###

* -ly vs -ally
* amoral, disinterested vs immoral, uninterested
* assure vs ensure vs insure
* awhile vs a while
* accuracy vs prediction
* born, aid, breath vs borne, aide, breathe
* classic vs classical
* complementary vs complimentary
* counsellor vs councillor
* disk vs disc
* effect vs affect
* everyone vs every one
* fiancé vs fiancée
* historic vs historical
* phase vs faze
* seize vs cease
* surveillance vs wiretapping (vs dragnet)
* you and I vs you and me

A lot of people

\* Except when referring to homosexual couples specifically

Acronyms/Abbreviations
----------------------
Use Markdown’s [abbreviation syntax][] in the following cases:

 Shorthand  | Full Word
:-----------|:----------------------------------
 MEPs       | members of the European Parliament
 MPs        | members of parliament

Definitions
-----------
* [Genocide][]
* [Torture][]

Immigrant vs Expatriot
----------------------
Use **immigrants** in general and avoid **expatriots**.

You can use **expatriots** to draw an explicit distinction between immigrants who intend permanent residence to a expatriots whose future residency plans are significantly more ambiguous.

Reporting on Politics
---------------------
Be sure to distinguish between:

* Majorities of votes (ie a majority of the popular vote)
* Majorities of seats in parliament (ie an electoral majority)

Refrain from using “supermajority” and “absolute majority”, when you are in fact just describing a basic majority of seats.

In Britain, parties can gain a majority of seats without a majority of votes. Do not call this majority of seats an absolute majority; absolute majorities and supermajorities are for circumstances that require more than 50% of seats in parliament.

### US Politics ###

Be wary of sentences akin to “Congress does `X`”. In many cases, it is actually only one of the two chambers, the Senate and the House that block or pass measures in the news, meaning that the bill has in fact neither been passed or blocked.

Furthermore, only write that “the Senate/House does `X`”, when both parties vote across partisan lines with a similar ratio of Aye/Nay votes. Otherwise, write that “Republicans/Democrats do `X` in the Senate/House”.

Terrorism
---------
If a US attack meets the [18 U.S.C. § 2331 definition of terrorism][us-terrorism], describe the perpetrator(s) as a (domestic) terrorist. Do not use vague terms like ”shooter“ or ”gun(wo)man“.

Different, legal, definitions of terorism may apply in other countries.

Essentialism
------------
Avoid nouns defining people by traits, and generally nounified adjectives:

 Preferred                           | Not Preferred
:------------------------------------|:-----------------
 black and Asian people              | blacks and Asians
 gay and lesbian people              | gays and lesbians
 homo-, bi-, and heterosexual people | homo-, bi-, and heterosexuals
 illegal( immigrant)s                | people living [somewhere] illegally
 men, women                          | males, females

Be particularly careful with referring to people “victims”.

By using an adjective rather than a noun for your description, you describe a trait instead of defining an identity.

### Disabilities ###

When referring to medical conditions and disabilities, it is preferred to use the construction “people (diagnosed) with `condition`”:

 Preferred                             | Not Preferred
:--------------------------------------|:-------------
 people (diagnosed) with schizophrenia | schizophrenic people, schizophrenics
 people (diagnosed) with diabetes      | diabetics
 people with disabilities              | disabled people, special-needs people

#### Abusing Technical Terms ####

Technical terms are not slurs, eg:

* lame
* schizophrenic/-a

### Nationality, Race, and Hyphenation ###

Hyphenated nationalities like “Native-Americans” and “African-Americans” are likewise discouraged. In order of preference, use

* “Native American people”, “Native Americans” (capitalized)
* “black people/Americans”, “African-American people”

It’s hardly always easy to figure out the appropriate, consistent terminology, but running into these situations is always cause for consulting available guides and manuals, as well as amending any existing ones, such as this.

#### Other Dos and Donts ####

 Preferred              | Not Preferred
:-----------------------|:----------------------
 biracial, multiracial  | mixed race, mulatto(!)

Do not use the following words as descriptors:

Media Guidelines
----------------
If we believe journalism has power to affect hearts and minds, it has power to afflict them as well.

Here is a selection of guidelines for ensuring that your writing has a positive effect:

* [GLAAD Media Reference Guide on Transgender Issues][transgender]
* [Prevent copycats by using guidelines for reporting on suicide][copycat]

### Self-Harm ###

* [“Samaritans’ Media Guidelines for Reporting Suicide”][suicide]
* [reportingonsuicide.com](http://reportingonsuicide.org/)
* [“Reporting on Suicide: Recommendations for the Media”][suicide-2] (.pdf)

Corrections
-----------
Some good pointers from BuzzFeed:

> ### How BuzzFeed Does Corrections ###
>
> * A correction should include the accurate information. It should explain the error, and it may restate the error when it’s necessary to clarify what it was or to debunk a claim. See sample corrections at the end of this doc.
> * Corrections should be made for errors of fact — not misspellings or typos or broken links. Do issue a correction, however, if someone’s name is misspelled throughout a story.
> * Corrections should be in plain English, not in the somewhat formal corrections style traditional among news organizations.
> * Be very thorough and careful. The absolute worst thing is to have to correct your correction. If the correction is about a person, it’s often a good move to read the correction on the phone to its subject before printing it.
> * Try to mention the correction on all channels the story went out on—if you tweeted it, tweet the correction, etc.
>
> ### Corrections vs. Updates ###
>
> Updates should be used to reflect important new information or clarifications; corrections are for mistakes.
>
> ### Process ###
>
> * Writers should draft corrections, but run them by their editor, team leader, or the after-hours list for approval/editing before putting them in.
>
> #### [Example:] Newsy, simple correction ####
>
> Twitter increased the value of its IPO shares to between $23 and $25. An earlier version of this post misstated the value range. [Include previous figure in correction, ed.]
>
> #### Example:] Newsy, restating the error ####
>
> Twitter’s CEO could not be reached for comment. An earlier version of this post said Twitter’s CFO could not be reached for comment.
>
> (^ This is also an example of when what was maybe just a typo warrants a correction rather than just a quick fix.)

### Diffs and Changelogs ###

Show the specific changes (before and after), ie “diffs”, with either an archive of the old version or by employing the `<del>` and `<ins>` tags:

> Evil Corp posted <del>$15B</del> <ins>$35B</ins> in profits.

[NewsDiffs][] is instructive on the importance of transparent diffs.

### Tweets ###

Delete the erroneous tweet—or reply to it with your corrective. Consider including an annotated screenshot of the old tweet in the new tweet.

### Markup ###

The correction text is placed a the bottom, but readers shouldn’t see them only when they’ve finished reading an article, as it will retroactively call the article into question. Place a notice at the top of an article alerting the reader to the existence of a correction or update at the bottom. Provide an internal link to navigate to the text from the notice.

#### Corrections as Paragraphs vs Lists ####

For corrections involving several errors, format the corrections as a list instead of a paragraph of multiple corrections; to use [a real correction example][nyt-correction]:

##### Bad #####

> An article last Sunday about new lodging options in Africa misstated the Canadian region where the winemaker Norman Hardie is based. It is Prince Edward County, Ontario, not the Niagara region. And the price for the trip offered with Mr. Hardie was given in the incorrect currency. The price is 6,975 Canadian, not U.S., dollars.

##### Good #####

> * An article last Sunday about new lodging options in Africa misstated the Canadian region where the winemaker Norman Hardie is based. It is Prince Edward County, Ontario, not the Niagara region.
> * The price for the trip offered with Mr. Hardie was given in the incorrect currency. The price is 6,975 Canadian, not U.S., dollars.

Other Resources
---------------
* [Common Errors in English Usage][ceeu]

TODO
----
- [ ] Settle **Foreign spellings** section of OED.
- [ ] Settle **Plurals** section of OED.
- [ ] Link to media guide for disabilities and neurodiversity.


[oed]: http://www.ox.ac.uk/public-affairs/style-guide
[ndarville.github.io]: https://ndarville.github.io/blog/2013/12/15/naming-the-thirteen-dwarves-in-the-hobbit.html
[ndarville/style/html]: https://github.com/ndarville/style/blob/master/html/README.md
[link-text]: http://www.w3.org/QA/Tips/noClickHere
[compound modifiers]: https://en.wikipedia.org/wiki/English_compound#Hyphenated_compound_modifiers
[mcs]: http://www.mcsweeneys.net/articles/an-interactive-guide-to-ambiguous-grammar
[nasa]: http://history.nasa.gov/printFriendly/styleguide.html

[a]: http://socialdemokraterne.dk/default.aspx?site=english
[b]: http://www.radikale.dk/english
[o]: http://www.danskfolkeparti.dk/The_Party_Program_of_the_Danish_Peoples_Party
[v]: http://www.venstre.dk/servicemenu/english/facts-about-venstre/
[ø]: http://enhedslisten.dk/content/red-green-alliance

[broadband]: http://www.fcc.gov/reports/2015-broadband-progress-report
[genocide]: http://www.ohchr.org/EN/ProfessionalInterest/Pages/CrimeOfGenocide.aspx
[torture]: http://www.hrweb.org/legal/cat.html#Article%201.1
[abbreviation syntax]: https://michelf.ca/projects/php-markdown/extra/#abbr
[us-terrorism]: https://www.fbi.gov/about-us/investigate/terrorism/terrorism-definition
[transgender]: http://www.glaad.org/reference/transgender
[copycat]: http://www.theatlantic.com/national/archive/2012/12/the-media-needs-to-stop-inspiring-copycat-murders-heres-how/266439/
[suicide]: http://www.samaritans.org/media-centre/media-guidelines-reporting-suicide
[suicide-2]: http://www.sprc.org/sites/sprc.org/files/library/sreporting.pdf
[NewsDiffs]: http://newsdiffs.org
[nyt-correction]: http://www.nytimes.com/2015/11/01/pageoneplus/corrections-november-1-2015.html
[ceeu]: http://public.wsu.edu/~brians/errors/
