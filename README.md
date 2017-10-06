# TextFormatterInsertDummyContent

A TextFormatter for ProcessWire CMS/CMF that aims to aid development by allowing the quick insertion of dummy text via shortcodes.

Usage is simple - just type for example **[dc3]** into a textarea with this textformatter applied (plain textarea or CKEditor) and it will be replaced at runtime by **3** paragraphs of dummy content. It can also be used to populate text fields (for headings etc) using e.g. **[dc4w]**. This will produce **4 w**ords (rather than paragraphs) at runtime.

The actual content comes from an included 'dummytext.txt' file containing 50 paragraphs of 'Lorem ipsum' from [lipsum.com](http://www.lipsum.com/). The 50 paragraphs is arbitrary - it could be 10 or 100 or anything in between, and the contents of that file can be changed for your own filler text if you wish.
