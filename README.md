# Thaanaepub3
Thaana epub3 template 

Basic template for Thaana epub3 files (works with google playbooks & apple ibooks)

After you are done editing the file and before publishing validate the epub using epubcheck or an online epub validatoe like http://validator.idpf.org/

To manually create the epub after editing do the following: 

$ zip -X0 Alhuganduge_Dhuvahu_Foiy.zip mimetype
$ zip -rDX9 Alhuganduge_Dhuvahu_Foiy.zip * -x "*.DS_Store" -x mimetype
$ mv Alhuganduge_Dhuvahu_Foiy.zip Alhuganduge_Dhuvahu_Foiy.epub


To check using epubcheck do the following:

$ epubcheck Alhuganduge_Dhuvahu_Foiy.epub 
Validating against EPUB version 3.0 - custom validation
WARNING(HTM-015): Alhuganduge_Dhuvahu_Foiy.epub/Text/titlepage.xhtml(-1,-1): HTML4 DOCTYPE definition within ePub v3.
Validating using EPUB version 3.0 rules.
ERROR(HTM-004): Alhuganduge_Dhuvahu_Foiy.epub/OEBPS/Text/titlepage.xhtml(0,0): Irregular DOCTYPE: found '-//W3C//DTD XHTML 1.1//EN', expected '<!DOCTYPE html>'.

Check finished with errors

epubcheck completed

If there are errors it will display them. If no errors you should get an output like below

$ epubcheck Alhuganduge_Dhuvahu_Foiy.epub 
Validating against EPUB version 3.0 - custom validation
Validating using EPUB version 3.0 rules.
No errors or warnings detected.
epubcheck completed

 
