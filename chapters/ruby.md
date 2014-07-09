# I was going to write a post about Softcover but decided that before I do I need to cover some of the dependencies that are required for it.  

## The post about Softcover will be coming shortly.

The first and major dependency is to have Ruby and Rubygems installed on your system.

If you already have them then you can skip the rest of this post.  If you do not yet have them, then continue reading and I will show you where to get them and how to install them.

What is Ruby?

First let me tell you what Ruby is not.  In this case it is not the red gemstone that is made into jewellery.  It is an interpreted  programming language, but don't let this scare you as you will not have to do any programming to use Softcover.  But, you can if you want to.

Where can I get Ruby?

The program is available at https://www.ruby-lang.org/en/downloads/ . On this page are versions for various operating systems including Linux, Mac and Windows.  I have heard that there are problems with loading it on Windows but it works fine on the other systems.  I use only Linux so I will give you instructions on how to use Ruby in the Linux environment.  If you are also using Linux then select the "latest stable version".  At the time of this writing it is 2.1.1.

Once you have it downloaded you will need to extract it as the download is a compressed archived file.  You should have an extractor program already installed on your system.  Then "cd /directory where it is extracted" that is, from a terminal window change to the directory where the extracted files are located.  As this is where the Ruby source code is located you will need to issue 3 commands to install it.

    Enter "./configure" minus the quotes.  This will print a lot of stuff to your screen and then bring you back to your command prompt.
    Enter "make" again without the quotes when you get your prompt back.  This will also print a lot of stuff to your screen.
    Finally enter "sudo make install" or just "make install" depending on your operating system.  This command will actually install Ruby  on your system.

For Mac or Windows systems see https://www.ruby-lang.org/en/installation/  for these systems as I do not use either.

Once you have Ruby installed enter the command "ruby -v" again without the quotes.  This should come back with "2.1.1" or whatever is the version number when you install it.

 

Now on to Rubygems.

These are add-ons that have been developed by third parties to increase the usability of Ruby.  Softcover is one.  You can get Rubygems at http://rubygems.org/ Just click on the link "Install Rubygems 2.2.2" at the time of this writing.  You will be given 4 choices of file to download:

    TGZ which is Linux compressed file.
    Zip which is a Windows and maybe a Mac compressed file.
    GEM which is an upgrade file if you have a previous version installed.
    GIT will take you to GITHUB where the source code is located.  You will only need this if you plan to contribute to the project.

I would recommend that you select either 1 or 2 from that page.  You will have to extract these files to another directory.  Change to the directory  where the files are located.  To install the application just enter "ruby setup.rb" again without the quotes.  This is the Ruby source file for installing the Rubygems application.  Most files having a ".rb" extension are Ruby source files.

To add gems to your system enter the command "sudo gem install name-of-gem" or "gem install name-of-gem" depending on your system.

Congratulations:

You are now up and running with Ruby and Rubygems.

If you have any comments, questions or suggestions feel free to fill out the COMMENT box below.

If enough readers leave comments about learning how to program in Ruby, I can cover that in a future post.

Better than that, I found a site presenting a FREE 7 day course in Ruby programming at http://howtoprogrambetter.com/start-programming-now-free-7-day-online-course/
