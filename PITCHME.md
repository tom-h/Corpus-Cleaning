# Corpus Cleaning Workshop

http://github.com/tom-h/Corpus-Cleaning

---

# Terminology

- Archive
- Corpus
- Metadata

---

## What is archiving?

- A record of work done, gathered while that work is being done
- A place where that record is preserved by specialists
- A place where researchers and other interested parties can reconstruct the work that you have done

*Corpora are ideally built upon archived or published material, i.e., built upon citable sources*

---

## What is a corpus?

- A collection of textual material coded in a way that it aims to answer one or more specific research goals
- The place to go to discover/check your assertions
- Potentially: a place to send other people to verify or extend upon your work

*Training ASR is an extension of your work that requires a well organised and consistent corpus.*

---

## What is a “clean” corpus?

- One where categories of annotation/metadata are clearly distinguishable to other researchers (and to computers…)
- One where tokens are consistently delimited in a principled and consistent fashion
- Ideally, one where each category of annotation/metadata is distinguished in parallel but separate streams.

---

- More likely: a collection of conventions that are well documented and consistently applied

*Cleaning a corpus is the process of reviewing the categories that you have coded, documenting conventions, or better moving away from convention to explicit, consistent and verbose coding of categories of annotations such that a non-expert can understand what you have done*

---

## What are tokens?

- Chunks of “primary” data
- a term more conventionally used in computational linguistics
- A way of thinking about how a computer sees language data
- A way of thinking about at what levels annotations may apply

---

## What is metadata?

- ...Data about data: ...but, that’s almost everything
- Usually used to refer to classes of specific metadata created for a purpose, e.g.,:
  - File Metadata:
  - Date and times
  - Filename
  - File type
  - Permissions
  - etc...

---

## Archival metadata

- Descriptive metadata
- Rights metadata
- Provenance Metadata
- Structural metadata
- ...

---

## Research metadata

- Specific categories of metadata that may overlap with archiving
- Coding of categories that inform your research questions
- What are annotations?
- A type of “metadata”: an elaboration on data or metadata

---

# Workflow

### Where does archiving fit relative to my research goals?
### Where does corpus building fit relative to my research goals?
### How does principled corpus building and archiving help me achieve my research goals?

---

## Data Gathering

- Junk-in junk-out
- It all starts with the best possible data
- Gathering good primary data
- Noise free audio
- Metadata best practice

---

## Legacy materials

- Careful treatment of legacy materials
- Tracking original metadata to capture context in a recoverable fashion
- Close association between original data and enriched forms
E.g., new annotations reference page numbers of source, filename for image of source, etc

---

# Archiving

---

- Archives capture bundles of files that record the work that you have done
- Ideally, this would capture change over time, not just “finished” materials
- Work that contextualises language material is suitable for archiving

---

- Links to legacy materials, or further work based on legacy materials
- Genealogies
- Fieldnotes
- etc...

---

- Archive early, archive incrementally
- Get permissions, do the paperwork, create a collection
- Understand the requirements of file-naming and directory structure

---

### Archive new materials as they are created
  - Media generally doesn’t change once captured, and so it can and should be archived immediately
  - Transcripts change between capturing, reviewing and corpus building
  - Consider archiving on a timetable to capture these changes, or archiving at the end of certain phases of work

---

- Incremental changes can be extremely useful, and can be kept private if necessary
- There is no limit on the number of times you can do this, or when you do this
- Make a record of what you have done:
  - Imagine someone trying to reverse engineer your work… imagine trying to do it yourself!

---

### Use the benefits of early archiving:

  - Working/compressed versions of media files always available for download... the day after archiving
  - A record of what changed when (very important as data is now born digital)
  - Metadata folded into media
  - Neatly organised file structure and metadata
  
---

**Note that there are expectations and guidelines for archiving for CoEDL Member/Affiliates:**

http://www.dynamicsoflanguage.edu.au/research/data-archives/expectations-of-coedl-members-and-affiliates/

You do not need to be an expert at this! The data manager, Julia Miller, is available for you to consult with at any time. If you haven’t talked to her yet, then make an appointment.

---

# Corpus building

---

Many linguistics projects start with the gathering of language data into a collection called a “corpus”

- The corpus may be a subset of archived materials, and may incorporate work produced by others. Ideally, it is built on citable sources.

---

- CoEDL has a separate project to capture corpora of Australian and Pacific language materials
The primary object in a textual corpus is the text, while annotations contextualise this text
- This inverts the relationship between the notion of the audio as the primary source. An audio segment instead contextualises the text!

---

A corpus aggregates individual transcripts/sessions into a larger “document” or database

- This means that structure and coding of comparable categories needs to be equivalent across individual documents

---

## Design

- Design limits/shapes potential uses
- What kinds of questions can be asked?
- What structure best communicates categories of information?

---

- Historical conventions are driven by a need to save space on a printed page, and the need to save time when typing it all in
- Humans are terrible at being consistent!
- Good design will broaden the possible uses of your work
- Planning to change your mind will help

---

## Tools

- Most transcription software has a built-in means of reviewing and changing the consistency of a corpus

### In CLAN:

- CHAT is an extremely elaborate system of conventions coding very precise features. 

### In ELAN:

- Explode conventions into parallel tiers

### In General:

- Search for punctuation, sequences of capital letters, ...

---

## Mixed categories

- Many linguists work with, at a minimum, chunks of transcription, and possibly corresponding translation. While these may seem straightforward categories of data, in reality they are often a jumble of mixed categories.
- Inline meta-annotation, often by a set of loose and expanding conventions, is useful way of speeding up transcription. 

*It is a good idea to review, separate and expand these conventions once the corpus is of a reasonable size. Working on a corpus of a reasonable size will allow you to clean more quickly, without repeating work.*

---

## Transcription

For ASR, and more generally, the principles behind the transcription need to be consistent.

- Is the transcription orthographic, phonemic, or phonetic?
- Does that apply for everything?
  - E.g., if there is code switching, do you switch between orthographies?

---

- If someone is switching between Kriol, English and another language, what is the phonemic equivalent of a numeral like “1”?

---

- Are there any shorthand forms like abbreviation?
  - “PNG”
  - “Hello? X5”

---

- Are meta- or para-linguistic events folded into the transcription?

---

- What punctuation is used, and what does it mean?

---

- Is the same punctuation used for more than one purpose?
  - “He walk-ed.” (morpheme boundary)
  - “He wal- … ran.” (false start)
  - “He walked- no actually he ran.” (“rushed” prosody)
  
---

- What are spaces used for?|
  - what about compounds?

---

# ELAN setup

---

### Types and Tiers

- Types describes the nature of the data being captured
- Tiers are instantiations of those types 

---

## Types

"transcription", "translation", "morphs", "words", "commentary", "custom coding"

*ideally, a type should describe the nature of the data, so that a user can interpret it*

"default", "default-lt", "tx", "ft", "symbolic subdivision", "included in"

---

# Types > Stereotypes

- describes the relationship between a parent tier
- code time-based or abstract relations between tiers

---

#### Types > Stereotypes > Time-based

### "no stereotype"
### Included-in
### Time-subdivision

---

#### Types > Stereotypes > Time-based 

### "no stereotype"

- no parent tier
- spans of time that describe something close to the original recording
  - an utterance
  - a distinct physical event, guesture, hand shape

---

#### Types > Stereotypes > Time-based

### Included-in

- one or more spans of time within a larger span
  - a distinct event within a larger one
  - a raised eyebrow

---

#### Types > Stereotypes > Time-based

### Time sub-division

- One or more subevents that entirely overlap with the parent span (no gaps!)
  - words in an utterance
  - +/- raised eyebrow
  
---

#### Types > Stereotypes > Time-based

### Time sub-division

- exact time boundaries are optionally encoded
- i.e., you can indicate that the data is time-based, but that such detail is not (yet) coded

---

#### Types > Stereotypes > Abstract relations

### Symbolic Sub-division
### Symbolic Association

---

#### Types > Stereotypes > Abstract relations

- codes abstract relations
