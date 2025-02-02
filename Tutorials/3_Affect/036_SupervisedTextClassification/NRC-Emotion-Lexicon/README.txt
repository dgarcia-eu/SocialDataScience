
THE NRC WORD-EMOTION ASSOCIATION LEXICON (aka NRC Emotion Lexicon, aka EmoLex)
------------------------------------------------------------------------------

Version:	0.92
Released: 	10 July 2011
Copyright: 	2011 National Research Council Canada (NRC)
Created By: Saif M. Mohammad (Senior Research Scientist, National Research Council Canada)
			Peter Turney

Readme Last Updated: August 2022
Automatic translations from English to 108 languages was last updated: August 2022

Home Page: 	http://saifmohammad.com/WebPages/NRC-Emotion-Lexicon.htm

Contact: 	Dr. Saif M. Mohammad 
		 	saif.mohammad@nrc-cnrc.gc.ca 
		 	uvgotsaif@gmail.com

TABLE OF CONTENTS

            I.    General Description
            II.   Papers And Citation
            III.  Python Code To Analyze Emotions In Text
            IV.   NRC Emotion Lexicon In Various Languages
            V.    Lemmatization And Other Techniques That May Be Beneficial
            VI.   Forms Of The Lexicon, Files, And Format
            VII.  Version Information And Change Log
            VIII. Other Emotion Lexicons
            IX.   Terms Of Use
            X.    Ethical Considerations


I. GENERAL DESCRIPTION
----------------------

The NRC Emotion Lexicon is a list of English words and their associations with eight emotions
(anger, fear, anticipation, trust, surprise, sadness, joy, and disgust) and two sentiments
(negative and positive). The annotations were manually done through crowdsourcing.

This work was approved by the NRC Research Ethics Board (NRC-REB) under protocol number
2009-94. REB review seeks to ensure that research projects involving humans as
participants meet Canadian standards of ethics.

Companion lexicons -- the NRC Emotion Intensity Lexicon and the NRC VAD Lexicon are available here:
http://saifmohammad.com/WebPages/lexicons.html

Applications: The lexicon has a broad range of applications in Computational Linguistics, Psychology,
Digital Humanities, Computational Social Sciences, and beyond. Notably it can be used to:
- study how people use words to convey emotions.
- study how emotions are conveyed through literature, stories, and characters.
- obtain features for machine learning systems in sentiment, emotion, and other affect-related tasks and
  to create emotion-aware word embeddings and emotion-aware sentence representations.
- evaluate automatic methods of determining emotion intensities (using lexicon entries as gold/reference scores).
- study psychological models of emotions.
- study the role of emotional words in emotional sentences, tweets, snippets from literature.


II. PAPERS AND CITATION 
-----------------------

- Saif Mohammad and Peter Turney. Crowdsourcing a Word-Emotion Association Lexicon.
Computational Intelligence, 29(3): 436-465, 2013. Wiley Blackwell Publishing Ltd.
 	 
- Saif Mohammad and Peter Turney. Emotions Evoked by Common Words and Phrases: Using
Mechanical Turk to Create an Emotion Lexicon. In Proceedings of the NAACL-HLT 2010
Workshop on Computational Approaches to Analysis and Generation of Emotion in Text, June
2010, LA, California.

If you use the lexicon in your work, then:

- Cite the papers:
		@article{Mohammad13,
			Author = {Mohammad, Saif M. and Turney, Peter D.},
			Journal = {Computational Intelligence},
			Number = {3},
			Pages = {436--465},
			Title = {Crowdsourcing a Word-Emotion Association Lexicon},
			Volume = {29},
			Year = {2013}
		}
		@inproceedings{mohammad-turney-2010-emotions,
    		title = "Emotions Evoked by Common Words and Phrases: Using {M}echanical {T}urk to Create an Emotion Lexicon", 
			author = "Mohammad, Saif  and Turney, Peter",
    		booktitle = "Proceedings of the {NAACL} {HLT} 2010 Workshop on Computational Approaches to Analysis and Generation of Emotion in Text",
    		year = "2010",
    		address = "Los Angeles, CA",
    		publisher = "Association for Computational Linguistics",
    		url = "https://aclanthology.org/W10-0204",
    		pages = "26--34",
		}

- Point to the lexicon homepage: 
		http://saifmohammad.com/WebPages/NRC-Emotion-Lexicon.htm

Other relevant papers:

- Practical and Ethical Considerations in the Effective use of Emotion and Sentiment Lexicons.
  Saif M. Mohammad. arXiv preprint arXiv:2011.03492. November 2020.

- Ethics Sheet for Automatic Emotion Recognition and Sentiment Analysis.
  Saif M. Mohammad. Computational Linguistics. 48 (2): 239–278. June 2022.


III. PYTHON CODE TO ANALYZE EMOTIONS IN TEXT
--------------------------------------------

There are many third party software packages that can be used in conjunction with the NRC
Emotion Lexicon to analyze emotion word use in text. We recommend Emotion Dynamics:

	https://github.com/Priya22/EmotionDynamics

It is the primary package that we use to analyze text using the NRC Emotion Lexicon and
the NRC VAD Lexicon.  It can be used to generate a csv file with a number of emotion
features pertaining to the text of interest, including metrics of utterance emotion
dynamics. 

See this paper for an example of the use of the lexicon to analyze emotions in text:

	Tweet Emotion Dynamics: Emotion Word Usage in Tweets from US and Canada. Krishnapriya
	Vishnubhotla and Saif M. Mohammad. In Proceedings of the 13th Language Resources and
	Evaluation Conference (LREC-2022), May 2022, Marseille, France.

	https://arxiv.org/pdf/2204.04862.pdf


IV. NRC EMOTION LEXICON IN VARIOUS LANGUAGES
--------------------------------------------

The NRC Emotion Lexicon has affect annotations for English words. Despite some cultural
differences, it has been shown that a majority of affective norms are stable across
languages. Thus, we provide versions of the lexicon in over 100 languages by translating
the English terms using Google Translate (August 2022).

The lexicon is thus available for English and these languages:

Afrikaans, Albanian, Amharic, Arabic, Armenian, Azerbaijani, Basque, Belarusian, Bengali,
Bosnian, Bulgarian, Burmese, Catalan, Cebuano, Chichewa, Corsican, Croatian, Czech,
Danish, Dutch, Esperanto, Estonian, Filipino, Finnish, French, Frisian, Gaelic, Galician,
Georgian, German, Greek, Gujarati, HaitianCreole, Hausa, Hawaiian, Hebrew, Hindi, Hmong,
Hungarian, Icelandic, Igbo, Indonesian, Irish, Italian, Japanese, Javanese, Kannada,
Kazakh, Khmer, Kinyarwanda, Korean, Kurmanji, Kyrgyz, Lao, Latin, Latvian, Lithuanian,
Luxembourgish, Macedonian, Malagasy, Malay, Malayalam, Maltese, Maori, Marathi, Mongolian,
Nepali, Norwegian, Odia, Pashto, Persian, Polish, Portuguese, Punjabi, Romanian, Russian,
Samoan, Sanskrit, Serbian, Sesotho, Shona, Simplified, Sindhi, Sinhala, Slovak, Slovenian,
Somali, Spanish, Sundanese, Swahili, Swedish, Tajik, Tamil, Tatar, Telugu, Thai,
Traditional, Turkish, Turkmen, Ukranian, Urdu, Uyghur, Uzbek, Vietnamese, Welsh, Xhosa,
Yiddish, Yoruba, Zulu

Note that an earlier version included translations obtained in 2017. The current 2022
translations are markedly better. That said, some of the translations may still be incorrect
or they may simply be transliterations of the original English terms.


V. LEMMATIZATION AND OTHER TECHNIQUES THAT MAY BE BENEFICIAL
------------------------------------------------------------

The lexicon file can be used as is, but occasionally certain additional techniques can be
applied to make the most of it for one's specific application context.

1. LEMMATIZATION: The lexicon largely includes the base forms or lemmas of words. For
example, it may include an entry for 'attack', but not for 'attacks' or 'attacking'. In
many cases, such morphological variants are expected to have similar emotion scores. So
one can first apply a third-party lemmatizer on the target text to determine the base forms
before applying the lexicon. Note that lemmatization must be applied with care; for
example, while it it good to go from 'helplessness' to 'helpless' (they are expected to
have similar emotional connotations), 'helplessness' should not be lemmatized to 'help'
(they are expected to have markedly different emotional connotations). Further, various
factors such as tense and 'differing predominant senses for different morphological forms'
can impact emotionality. So benefits of lemmatization are limited, especially when
analyzing large pieces of text.

2. OTHER: Other techniques such discarding highly ambiguous terms (terms with many
meanings), or identifying most common terms in one's text and inspecting emotion entries
in the lexicon for those terms (and correcting entries where appropriate), etc. are also
good practice.


VI. FORMS OF THE LEXICON, FILES, AND FORMAT 
-------------------------------------------

1. NRC-Emotion-Lexicon-Wordlevel-v0.92.txt: Has annotations at WORD LEVEL. This is the
primary lexicon file used by the vast majority of users. The word-level lexicon was
created by taking the union of emotions associated with all the senses of a word (see form
4). This is the primary form of the lexicon, and is used by the vast majority of users.

Each line has the following format:
<term><tab><AffectCategory><tab><AssociationFlag>

<term> is a word for which emotion associations are provided;

<AffectCategory> is one of eight emotions (anger, fear, anticipation, trust, surprise,
sadness, joy, or disgust) or one of two polarities (negative or positive);

<AssociationFlag> has one of two possible values: 0 or 1. 0 indicates that the target word
has no association with affect category, whereas 1 indicates an association.


2a.  NRC-Emotion-Lexicon-ForVariousLanguages.txt: This file has the same first eleven
columns as the NRC-Emotion-Lexicon-Wordlevel-v0.92.txt.  Additionally, it has columns
pertaining to over 100 languages. Each of these columns lists the translations of the
English words into the corresponding language. For example, the column Japanese contains
the Japanese translations of the English words.  The translations were obtained using
Google Translate in August 2022.


2b. OneFilePerLanguage: This directory has the same information as in
NRC-Emotion-Lexicon-ForVariousLanguages.txt, but in multiple files -- one for each
language.  Each of these files has twelve columns. The first eleven columns are the same
as in NRC-Emotion-Lexicon-ForVariousLanguages.txt. Additionally, it has  a column for the
translation of the English words to a different language -- the language corresponding to
the file name.  So if one is interested only in the Japanese version of the lexicon, then
they can simply use Japanese-NRC-EmoLex.txt.


3. NRC-Emotion-Lexicon-Senselevel-v0.92.txt: Has annotations at WORD-SENSE LEVEL.  This is
the original form of data annotation. The information from this file was aggregated to
create the word-level lexicon (described in bullet 1).

Each line has the following format:
<term>--<NearSynonyms><tab><AffectCategory><tab><AssociationFlag>

<term> is a word for which emotion associations are provided;

<NearSynonyms> is a set of one to three comma-separated words that indicate the sense of
the <term>. The affect annotations are for this sense of the term.

<AffectCategory> is one of eight emotions (anger, fear, anticipation, trust, surprise,
sadness, joy, or disgust) or one of two polarities (negative or positive);

<AssociationFlag> has one of two possible values: 0 or 1. 0 indicates that the target word
has no association with affect category, whereas 1 indicates an association.

4. ListOfLanguages-For-Which-Lexicon-Availabale.txt: Lists the languages for which the
lexicon is available.

5. Paper1_NRC_Emotion_Lexicon.pdf and Paper2_NRC_Emotion_Lexicon.pdf: The research papers describing the NRC Emotion Lexicon.

6. Paper-Practical-Ethical-Considerations-Lexicons.pdf: Practical and Ethical Considerations in the
Effective use of Emotion and Sentiment Lexicons

7. Paper-Ethics-Sheet-Emotion-Recognition.pdf: Ethics Sheet for Automatic Emotion Recognition and Sentiment Analysis.


ENCODING: The lexicon files were created using UTF-8 encoding. You can view the lexicon files using
most text editors, Microsoft Excel, etc. You might have to make sure that the viewer
supports characters from various languages, i.e., set the encoding option in the viewer to
UTF-8, etc.  For example, to view in excel, follow these steps:

- open excel
- click on File -> Import
- select file type as 'Text file'
- select the lexicon file to import in the dialog box that opens up
- select 'File Origin' type as 'Unicode (UTF-8)'
- click 'Finish'


VII. VERSION INFORMATION AND CHANGE LOG
----------------------------------------

- Version 0.92 is the latest version (Released July 2011).  
- The automatic translations generated using Google Translate are updated every few years.  
  They were last obtained in August 2022. 
- The README was last updated in August 2022. 


VIII. OTHER EMOTION LEXICONS
----------------------------

- The NRC Emotion Intensity Lexicon is a list of English words (taken from the NRC Emotion
Lexicon and other sources) with real-valued scores of intensity for eight discrete emotions
(anger, anticipation, disgust, fear, joy, sadness, surprise, and trust). 

	Word Affect Intensities. Saif M. Mohammad. In Proceedings of the 11th Edition of the Language 
    Resources and Evaluation Conference (LREC-2018), May 2018, Miyazaki, Japan.
    
    http://saifmohammad.com/WebPages/AffectIntensity.htm

- The NRC Valence, Arousal, and Dominance (VAD) Lexicon includes a list of more than 20,000 English words and
their valence, arousal, and dominance scores.  For a given word and a dimension (V/A/D), the scores range from
0 (lowest V/A/D) to 1 (highest V/A/D).

    Obtaining Reliable Human Ratings of Valence, Arousal, and Dominance for 20,000 English Words.  Saif M.
    Mohammad. In Proceedings of the 56th Annual Meeting of the Association for Computational Linguistics,
    Melbourne, Australia, July 2018.

	http://saifmohammad.com/WebPages/nrc-vad.html

Various other emotion lexicons can be found here:
http://saifmohammad.com/WebPages/lexicons.html

You may also be interested in some of the other resources and work we have done on the
analysis of emotions in text:

http://saifmohammad.com/WebPages/ResearchAreas.html
http://saifmohammad.com/WebPages/ResearchInterests.html#EmotionAnalysis


IX. TERMS OF USE 
----------------

1. Research Use: The lexicon mentioned in this page can be used freely for non-commercial
research and educational purposes.

2. Citation: Cite the papers associated with the lexicon in your research papers and
articles that make use of them. 

3. Media Mentions: In news articles and online posts on work using the lexicon, cite the
lexicon. For example: "We make use of the <resource name>, created by <author(s)> at the
National Research Council Canada." We would appreciate a hyperlink to the lexicon home
page and an email to the contact author (saif.mohammad@nrc-cnrc.gc.ca).  (Authors and
homepage information provided at the top of the README.)

4. Credit: If you use the lexicon in a product or application, then acknowledge this in
the 'About' page and other relevant documentation of the application by stating the name
of the resource, the authors, and NRC. For example: "This application/product/tool makes
use of the <resource name>, created by <author(s)> at the National Research Council
Canada." We would appreciate a hyperlink to the lexicon home page and an email to the
contact author (saif.mohammad@nrc-cnrc.gc.ca).

5. No Redistribution: Do not redistribute the data. Direct interested parties to the
lexicon home page.  You may not rent or license the use of the lexicon nor otherwise
permit third parties to use it. 

6. Proprietary Notice: You will ensure that any copyright notices, trademarks or other
proprietary right notices placed by NRC on the lexicon remains in evidence.

7. Title: All intellectual property rights in and to the lexicon shall remain the property
of NRC. All proprietary interests, rights, unencumbered titles, copyrights, or other
Intellectual Property Rights in the lexicon and all copies thereof remain at all times
with NRC.

8. Commercial License: If interested in commercial use of the lexicon, contact the author:
saif.mohammad@nrc-cnrc.gc.ca

9. Disclaimer: National Research Council Canada (NRC) disclaims any responsibility for the
use of the lexicon and does not provide technical support. NRC makes no representation and
gives no warranty of any kind with respect to the accuracy, usefulness, novelty,
validity, scope, or completeness of the lexicon and expressly disclaims any implied
warranty of merchantability or fitness for a particular purpose of the lexicon.  That
said, the contact listed above welcomes queries and clarifications.

10 Limitation of Liability: You will not make claims of any kind whatsoever upon or
against NRC or the creators of the lexicon, either on your own account or on behalf of any
third party, arising directly or indirectly out of your use of the lexicon. In no event
will NRC or the creators be liable on any theory of liability, whether in an action of
contract or strict liability (including negligence or otherwise), for any losses or
damages incurred by you, whether direct, indirect, incidental, special, exemplary or
consequential, including lost or anticipated profits, savings, interruption to business,
loss of business opportunities, loss of business information, the cost of recovering such
lost information, the cost of substitute intellectual property or any other pecuniary loss
arising from the use of, or the inability to use, the lexicon regardless of whether you
have advised NRC or NRC has advised you of the possibility of such damages. 


We will be happy to hear from you. For example,:
- telling us what you are using the lexicon for
- providing feedback regarding the lexicon;
- if you are interested in having us analyze your data for sentiment, emotion, and other affectual information;
- if you are interested in a collaborative research project. We regularly collaborate with graduate students,
post-docs, faculty, and research professional from Computer Science, Psychology, Digital Humanities,
Linguistics, Social Science, etc.

Email: Dr. Saif M. Mohammad (saif.mohammad@nrc-cnrc.gc.ca, uvgotsaif@gmail.com)


X. ETHICAL CONSIDERATIONS
-------------------------

Please see the papers below (included with the download) for ethical considerations
involved in automatic emotion detection and the use of emotion lexicons. (These also act
as the Ethics and Data Statements for the lexicon.)

- Ethics Sheet for Automatic Emotion Recognition and Sentiment Analysis.
Saif M. Mohammad. Computational Linguistics. 48 (2): 239–278. June 2022.

- Practical and Ethical Considerations in the Effective use of Emotion and Sentiment Lexicons.
Saif M. Mohammad. arXiv preprint arXiv:2011.03492. December 2020.

Note that the labels for words are *associations* (and not denotations). As noted in the
paper above, they are limited by when the dataset was annotated, by the people that
annotated them, historical perceptions, and biases. (See bullets c through h in the
paper). It is especially worth noting that identity terms, such as those referring to
groups of people may be particularly prone to inappropriate biases. Further, marginalized
groups have historically faced more negative perceptions. Thus some terms that are
associated with marginalized groups may be marked as having associations with negative
emotions by the annotators. For example, group X marked as being associated with negative
emotions could imply that they have historically faced negative emotions or that some
people have negative associations with group X, or there is some other reason for the
negative association. The exact relationship is not listed in the lexicon. In order to
avoid misinterpretation and misuse, and as recommended generally in the ethical
considerations paper, we have removed entries for a small number of terms (about 25) that
are associated with identity groups. For the vast majority of sentiment and emotion
analysis requirements this removal will likely have no impact or will be beneficial.

The list of identity terms used is taken from this list developed in 2019 on an offensive
language project (abusive language is often directed at some identity groups):

https://github.com/hadarishav/Ruddit/blob/main/Dataset/identityterms_group.txt

Only some of these terms occurred in our lexicon. This is not an exhaustive list; users
may choose to filter out additional terms for their particular task. We also welcome
requests for removal of additional terms from the list. Simply email us with the term or
terms and reason for removal.
 
