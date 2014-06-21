Softcover part 2.

In my previous post I was not able to list all of the features of Softcover so will use this post to put the finishing touches on.
One thing that I forgot in the previous post.

In the previous post I mentioned Markdown. Softcover uses a special version of Markdown to create your books from the files you generate. This version has additional features not offered by the general version of Markdown.
Tables.

There are 2 ways to create tables in Softcover. The first uses pipes (|), dashes (-) and equal signs (=).

An example is: | Cell 1 | Cell 2|

| Cell 3 | Cell 4|

This will produce a table that looks like the following.

 

    Cell 1  Cell 2
    Cell 3  Cell 4

However this will NOT create the horizontal lines after the first 2 rows. Dashes can be used to create a header row and equal signs can create a footer row.

The second method and the one that I used to create tables is using LaTeX tables via the tabular environment. An example of this is as follows:

\begin {tabular} { | r|l|c| } This will create a table with 3 cells wide, the first will be flush right, the second will be flush left and the third will have center alignment. The rows will be created by the following: Cell 1 & Cell 2 & Cell 3 \\ The double slashes at the end are required to define the end of the row. \hline will insert a horizontal line in the table. \multicolumn{3}{|c|}{\textsc{Centered over 3 columns}}\\ will create a row that is “Centered over 3 columns”. A caption for the table can be created by entering \caption{Some text used for the caption. \label{table:caption}}
Figures/pictures.

Figures/pictures can also be inserted into your books using a format similar to links. I have not yet tried this feature.
sc clean.

This is another command that I forgot to mention in the previous post. If you start getting errors that you don't know how to fix, try running the command “sc clean”. This will clean out old files that might no longer be compatible with the current version of your book.
Other commands.

There are numerous other commands that I have not yet used. These can be subjects for future posts.
The second part of the Softcover platform.

The second part of the Softcover platform is the on-line platform for publishing, marketing and selling ebooks and other digital products. This platform is located at https://www.softcover.io Once here you will need to create an account by clicking on the “Sign Up” link at the top right of the page. You need to enter an email, password and password confirmation and click on the “SIGN UP” button.

From your books directory enter the command “sc login”. It will ask for your email and password. You can then publish your book to the live site by entering the command “sc deploy”. This will build all versions of your book and publish it to the live site. The first time you do this it might take a little time but each subsequent time will take less time as it only uploads files that have changed.

If you want to make changes to the book formats that are uploaded and published you can edit the .softcover-deploy file.
Official Information.

For the official information check out the “softcover a manual, guide and reference” book by the developer of Softcover, Michael Hartl. This is located at https://www.softcover.io/browse
As usual use the comment box below to submit any and all comments, questions or suggestions or to sign up for our newsletter.

[mc4wp_form]
