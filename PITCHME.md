# Corpus Cleaning Workshop

http://github.com/tom-h/Corpus-Cleaning

https://gitpitch.com/tom-h/Corpus-Cleaning/master

---

# Topics

- Terminology
- Archiving
- Corpus building and cleaning

---

(time permitting)

- ELAN setup
- OpenRefine

---

# Terminology

- Archive
- Corpus
- Metadata

---

## What is an Archive?

- A record of work done, gathered while/once that work is being done |
- A place where that record is preserved by specialists |
- A place where researchers and other interested parties can reconstruct the work that you have done |

---

- Corpora are ideally built upon archived or published material, i.e., built upon citable sources

---

- Archiving is not publishing |
- (sort of...) |

- Archival sources are enduring and citeable |

---

## What is a corpus?

- A collection of textual material organised in a way that it aims to answer one or more specific research goals |
- The place to go to discover/check your assertions | 
- Potentially: a place to send other people to verify or extend upon your work |

---

- Training ASR is an extension of your work that requires a well organised and consistent corpus

---

- A corpus is not an archive |
- A corpus is more than a bundle of files |
- "Collection", "Bundle" and "Corpus" are all terms used to refer to archived files |

---

## What are tokens?

- Chunks of “primary” data |
- a term more conventionally used in computational linguistics |
- A way of thinking about how a computer sees language data |
- A way of thinking about at what levels annotations may apply |

---

## What are annotations?

- A type of “metadata”: an elaboration on data or metadata

---

- "Annotation" is used broadly in ELAN

---

## What is metadata?

- ...Data about data |
- data: observation |
- metadata: embues meaning |

---

Usually used to refer to classes of specific/standardised metadata created for a purpose, e.g.,:

- File Metadata: Date and times, Filename, File type, Permissions, etc...

---

## Archival metadata

- Descriptive metadata, Rights metadata, Provenance Metadata, Structural metadata, Content metadata
- etc

---

## Research metadata

- Specific categories of metadata that may overlap with archiving |
- Coding of categories that inform your research questions |
  - e.g., instances of a specific pattern not easily found by a search |
---

# Archiving

---

- Archives capture bundles of files that record the work that you have done |
- Ideally, this would capture change over time, not just “finished” materials |
- Any work that contextualises language material is suitable for archiving |

---

- Links to legacy materials, or further work based on legacy materials
  - Genealogies
  - Fieldnotes
  - Lexicons
  - Photos
  - etc...

---

- Archive early, archive incrementally |
- Get permissions, do the paperwork, create a collection |
- Understand the requirements of file-naming and directory structure |

---

### Archive new materials as they are created:

- Media files don't change once captured (usually) |
- Transcripts change between capturing, reviewing and corpus building |
- Consider archiving on a timetable to capture these changes, or archiving at the end of certain phases of work |

---

- Incremental changes can be extremely useful, and can be kept private if necessary |
- There is no limit on the number of times you can do this, or when you do this |
- Make a record of what you have done: |
  - Imagine someone trying to reverse engineer your work… imagine trying to do it yourself! |

---

### Use the benefits of early archiving:

  - Working/compressed versions of media files always available for download... the day after archiving |
  - A record of what changed when (very important as data is now born digital) |
  - Metadata folded into media |
  - Neatly organised file structure and metadata |
  - Citeable sources |  
---

**Note that there are expectations and guidelines for archiving for CoEDL Member/Affiliates:**

http://www.dynamicsoflanguage.edu.au/research/data-archives/expectations-of-coedl-members-and-affiliates/

You do not need to be an expert at this! The data manager, Julia Miller, is available for you to consult with at any time. If you haven’t talked to her yet, then make an appointment.

---

# Corpus building

---

- CoEDL has a goal to capture corpora of Australian and Pacific language materials

---

- after initial segmentation, transcription and translation

---

- gather together texts
  - own materials
  - legacy materials
  - other team members

---

- design may answer research question
- may need to control for variables

---

# Corpus Cleaning

---

## transcription
## annotation
## document grouping and/or metadata

---

## transcription

---

For ASR, and more generally, the principles behind the transcription need to be consistent.

- Is the transcription orthographic, phonemic, or phonetic?
- Does that apply for everything?
  - E.g., if there is code switching, do you switch between orthographies?

---

- If someone is switching between Kriol, English and another language, what is the phonemic equivalent of a numeral like “3”?

---

- Are there any shorthand forms like abbreviation?
  - “PNG”
  - “Hello? X5”

---

- Are meta- or para-linguistic events folded into the transcription?
- if so, do they disrupt the text, or occur in parallel

---

- What punctuation is used, and what does it mean?

---

- Is the same punctuation used for more than one purpose? |
  - “He walk-ed.” or "He walk -ed." (morpheme boundary) |
  - “He wal- … ran.” (false start) |
  - “He walked--no actually he ran.” (“rushed” prosody / parenthetical) |
  - "He wa----lked." (length)
  
---

Once separated, consider tokenising your text (or think about the consistency of your convention)

---

- What are spaces used for?|
  - what about compounds? "washing machine" |

---

## Annotation

- are comments folded into translation?
- are controlled vocabularies consistent?

---

## Tools

- Most transcription software has a built-in means of reviewing and changing the consistency of a corpus |
- sometimes a text editor is sufficient |
- regular expressions are awesome! |

---

#### regular expressions

Mosel, Ulrike 2012 "Advances in the accountability of grammatical analysis and description by using regular expressions" LD&C Special Publication 4

---

### In CLAN:

- CHAT is an extremely elaborate system of conventions coding very precise features. 

---

### In ELAN:

- Explode conventions into parallel tiers
- use tokensing features
- hide unused tiers
- use the ""

# ELAN setup

---

### Types and Tiers

- Types describe the nature of the data being captured
- Tiers are instantiations of those types 

---

## Types

"phonemic transcription", "english translation", "morphs", "commentary", "reported speech", "left hand shape"

---

## Types

*ideally, a type should describe the nature of the data, so that a user can interpret it*

---

## Types

"default", "default-lt", "tx", "ft", "symbolic subdivision", "included in"

---

## Types > Stereotypes

- describes the relationship between a tier and its parent
- code time-based or abstract relations between tiers

---

#### Types > Stereotypes > Time-based

### "none"
### Included-in
### Time-subdivision

---

#### Types > Stereotypes > Time-based 

### "none"

- no parent tier
- spans of time that describe something close to the original recording
  - a class of transcription (e.g., utterances, hand guestures, mouthing)

---

#### Types > Stereotypes > Time-based

### Included-in

- one or more spans of time within a larger span
  - a distinct event within a larger one
  - a raised eyebrow
  - a cough

---

#### Types > Stereotypes > Time-based

### Time sub-division

- One or more time based subevents that entirely overlap with the parent span (no gaps!)
  - words in an utterance
  - +/- raised eyebrow
  
---

#### Types > Stereotypes > Time-based

### Time sub-division

- exact time boundaries are optionally encoded
- i.e., you can indicate that the data is time-based, but that such detail is not (yet) coded

---

#### Types > Stereotypes > Abstract relations

### Symbolic sub-division
### Symbolic association

---

#### Types > Stereotypes > Abstract relations

- codes abstract relations
- one-to-one or one-to-many (in order)

---

#### Types > Stereotypes > Abstract relations

### Symbolic sub-division

- one-to-many
- sentence and words
- words and segments (especially for digraphs)

---

#### Types > Stereotypes > Abstract relations

### Symbolic association

- one-to-one
- word/morph and gloss
- transcription and translation

---

## Tiers

- label
- type
- speaker

---

- label = type x speaker
- use a delimiter
- shorter labels usually considered okay

---

### Toolbox:

"type@speaker"

---

## Templates

- one per speaker
- common tiers can be included

---

## Consistency

- use 'File' > 'Multiple File Processing' > 'edit multiple files'

---

# demonstration in ELAN

---

# OpenRefine

---

# Thanks