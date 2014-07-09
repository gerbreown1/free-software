# What is Softcover you might be asking.

## Well, I won't keep you waiting any longer, after the past two posts where I talked about dependencies for Softcover.

You might have guessed from some of the dependencies that Softcover has to do with e-books. You would be correct, it does have something to do with e-books.

But, it does a lot more as it also is a publishing platform for authors[^Hartl].

It consists of two main parts: a state-of-the-art-open-source ebook typesetting system and an online platform for publishing, marketing, and selling ebooks and other digital goods such as screencasts.
This post will focus on the first part.

The following information will focus on the first part – the ebook typesetting system.

## How do I install it?

###This is the very easy part after you have Ruby and Rubygems installed. 
Softcover is used from the command line in the terminal mode for your system. From the terminal command line just enter the command “gem install softcover” without the quotes. 

On some system you might need to have the word “sudo” at the front. Once it does its thing you will be up and running with Softcover by using the command “softcover xxxxx” or just “sc xxxxx”.
###The first command you should use.

Enter “sc check”, I use “sc” because I'm too lazy to type out the whole word. This “check” command will verify that you have all of the required dependencies installed as per the two previous posts. The second command you could use could be “sc help”. This will give you a list of all available commands.

##Creating your first e-book with Softcover.

Change to the directory where you want to create your book. Then enter the command “sc new *name-of-book* ”. This will create a bunch (technical term) of directories and files for you with the name of the main directory being *name-of-book*. You should then change to this directory. A lot of the files that are created can be removed after you inspect them to get an idea of what they files should look like.
###Files that you should change.

These files are located in the root directory of your book.

+    Book.txt. This will be a list of the files that will make up your book so you should delete all of the sample files that are listed there.

+    .softcover-build. Note the period at the beginning of the file name. If it does not show up it is because it is a hidden files. You need to tell your file manager to “*show hidden files*”.

In my *.softcover-build* I have the following entries:

+ softcover build:html
+ softcover build:pdf
+ softcover build:mobi 

*.softcover-deploy* has similar entries as the .softcover-build with the addition of “softcover publish”

###The next files that need to be changed are located in the “config” directory of your book. They are:

+ *book.yml*. In this file you will need to enter:
    + Title, Subtitle (if any or leave blank if none)
    + Description (or leave blank)
    + Author.
    + The other entries should NOT be changed.

+ *marketing.yml*. See the examples and make changes as you see fit. The main change should be to the authors:name. The “hide_custom_domain_footer” should be set to “false”

##After making these changes you are ready to start writing your famous novel as an ebook.

Each chapter will be a separate file with an extension of “.md”. These files need to be listed in the Book.txt file in the order that you want them to appear in the book, i.e. file 1 will be chapter 1, etc.


These files need to be created with TEXT Editor program NOT Word-processor program such as M$ Word or LibreOffice Writer. These programs can be used provided the output is saved as a text file. My current favorite text editor is called “Geany”, which I will report on in a future post.

## Markdown.

These files will contain “Markdown” code that will specify the output of your book. An example is double asterisks  before and after the text that you want to make **BOLD**. An underscore or a single asterisk  before and after a section of text will make it _ITALICS_.

###Foot notes and Links

Foot notes are created as such [^Text] and then at the bottom of the file you would enter [^Text]: Some text for the foot note. I was having problems until I discovered that the “:” is required.

Links are also very easy to create: Just enter the following, [Text that will be shown in the link](the URL that you want to link to). Note there is NO space between the ] and (.
### Headings

For headings just use the “#” = H1 or multiples of this for each heading, “##” = H2, “###” = H3, etc. If a line return is included in the sentence the text after the line return will not be included in the sentence. These headings are used to create the Table of Contents for your book.

##The following link lists the codes that are used for Markdown Markdown-Cheatsheet

###Math formulas.

You can also enter math formulas into your book if it is a Technical book. I have not yet used this feature so am not sure how it works.

###Source code.

If your book is about a programming language there are features that can be used in the Markdown file. This is another feature that I have not yet used.

##Lists.

This **IS** something I have used and it is very slick. Just enter “1.” at the beginning of the line for each item in the list and Softcover will automatically renumber them for you. You can enter an item in the middle of the list and the other items will be renumbered for you.

If you don't want to have numbers in your list just use “*”, “-” or “+” as the first character of your list item.

## Building your book.

When you have all of your chapters or parts of your chapters and are ready to create your book just enter the command “sc build:all” and Softcover will build a HTML, EPUB, MOBI and PDF file for your book. You can also build each individual file by replacing the “all” in the above command with the extension that you want to produce.

[^Hartl]: From the Softcover manual, guide and reference by Michael Hartl
