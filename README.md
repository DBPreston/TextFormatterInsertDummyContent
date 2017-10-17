# TextformatterInsertDummyContent

A Textformatter for ProcessWire CMS/CMF that aims to aid development by allowing the quick insertion of dummy text via shortcodes.

Usage is simple - just type for example **[dc3]** into a textarea with this textformatter applied (plain textarea or CKEditor) and it will be replaced at runtime by **3** paragraphs of dummy content. It can also be used to populate text fields (for headings etc) using e.g. **[dc4w]**. This will produce **4 w**ords (rather than paragraphs) at runtime.

## Tag Examples

- [dc3] - Show 3 paragraphs ([dc:3], [dc3p] & [dc:3p] all do the same).
- [dc3-6] - Show 3 to 6 paragraphs randomly per page load ([dc:3-6], [dc3-6p] & [dc:3-6p] all do the same).
- [dc3w] - Show 3 words ([dc:3w] does the same).
- [dc3-6w] - Show 3 to 6 words randomly per page load ([dc:3-6w] does the same).

The actual content comes from an included 'dummytext.txt' file containing 50 paragraphs of 'Lorem ipsum' from [lipsum.com](http://www.lipsum.com/). The 50 paragraphs is arbitrary - it could be 10 or 100 or anything in between, and the contents of that file can be changed for your own filler text if you wish.

## Upgrading From versions prior to 1.0.0

Prior to version 1.0.0 this module incorrectly capitalised the file and class name. In order to change this, you need to
follow this procedure...

- Remove TextFormatterInsertDummyContent from any fields that are using it
- Uninstall the original module
- Download the new version
- Refresh the modules list from the Processwire admin
- Select and install the TextformatterInsertDummyContent module
- Re-apply it as a formatter on each field you removed the original from.
