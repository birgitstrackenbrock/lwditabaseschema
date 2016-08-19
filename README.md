# lwditabaseschema
Defines a DITA-OT plugin containing LW DITA XML schema's, generated with Oxygen from DTD's standing in the plugins\org.oasis.lwdita\dtd

## Installation

Checkout this repository in {DITA_OT_PATH}/plugins/lwditabaseschema
From {DITA_OT_PATH} run ant -f integrator.xml

## Author information
The lwditamarketing has been created by Birgit Strackenbrock (XStructuring).

## Extra

### Legal topic

This topic type is extra added to the base element and can be used to contain the legal information of a document.

* legaltopic - root element for a legal information topic (based on topic/topic)
  * legalbody - the body of a legal information topic (based on topic/body)
    * disclaimer - a special section for the disclaimer(based on topic/section)
    * legalsection - a special section for other legal information than the disclaimer e.g. copyright (based on topic/section)
      * copyright - container for the copyright information (based on topic/p)
       * copyrightyear - date since protection is active (based on topic/ph)
       * copyrightholder - holder of the copyright (based on topic/ph)

### Faq topic

This topic type is extra added to the base element and can be used to contain the frequently asked questions of a document.

* faqtopic - root element for a faq topic (based on topic/topic)
  * faqbody - the body of a faq topic, container for questionandanswer elements(based on topic/body)
    * questionandanswer - container of a question and answer pair(based on topic/ul)
      * question - contains the question (based on topic/li)
      * answer - contains the answer to the question above (based on topic/li)
