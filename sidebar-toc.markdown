---
layout: page
title: Sidebar
permalink: /sidebar-toc/
---

* TOC
{:toc}

This example puts the Table of Contents in the Sidebar.  Just
paste the following in your page.


<button class="favorite styled" type="button">
  <a href="https://github.com/jwrr/minima-sidebar">Clone It</a>
</button>


```
* TOC
{:toc}
```

And create assets/main.scss with the following content.

```
---
---

@import "minima";

div.post-content > #markdown-toc {float:right;width:30%;max-width:320px;margin-top:-100px;}
div.post-content > #markdown-toc {list-style:none;padding-left:0;margin-left:0;}
div.wrapper {max-width:960px;margin-left:5%;}
div.post-content > p {width:65%;max-width:640;}
table,hr,p,div.highlight {width:65%;max-width:640;}
```

Examples
--------
Check out [Sidebar](/sidebar-toc), [Sidebar2](/sidebar-toc2) and [Sidebar Fixed](/sidebar-fixed) for more 
examples.

Jekyll Serve
------------

You can view this repo locally with the following command (I'm assuming you've
already installed [jekyll](https://jekyllrb.com/docs/) and cloned this repo.

```
jekyll serve --trace
```

You may get an error similar to the following:

```
/usr/lib/ruby/2.7.0/bundler/runtime.rb:312:in `check_for_activated_spec!': You 
have already activated rouge 3.20.0, but your Gemfile requires rouge 3.19.0. 
Prepending `bundle exec` to your command may solve this. (Gem::LoadError)
```

This means the `gem.lock` file is out of date.  To fix run the following 
command.  You may have to iterate multiple times if more than one gem is 
out of date.

```
bundle update rouge
```

Please send me a pull request with your fix.


Lorem Ipsum
-----------

You can ignore the following documentation.  I'm using the
[Lued Text Editor](https://jwrr.github.io/lued/)
documentation as Lorem Ipsum.


<hr>


Enter Magic
-------------------

First a little magic.  You enter an edit command, such as <kbd>alt+xw</kbd> to 
delete one word to the right.  Now you want to delete many words.  You
can keep pressing <kbd>alt+xw</kbd>... but it's a little annoying.  And here
enters the magic.  Press the <kbd>Enter</kbd> key instead. It repeats the
last <kbd>alt+??</kbd> command. This is a nice time saver, and may help keep the
carpal away.  Note, as soon as you enter another command, such as a <kbd>ctrl+?</kbd>
command or an arrow-key command, the <kbd>Enter</kbd> key reverts back to
being just a regular ole <kbd>Enter</kbd> key.

More Repeat Magic
-----------------
The above <kbd>Enter</kbd> repeats just the last <kbd>Alt</kbd> command.  Say
you just performed a sequence of commands that you want to repeat. <kbd>Ctrl+R</kbd>,
R for Repeat, shows a list of the most recent commands.  You enter the number of
commands you want to repeat and it is done.  Say you want to repeat it again.
Press <kbd>alt+rr</kbd> to repeat again.  Now if you to keep repeating, press
<kbd>Enter</kbd> repeatedly (or hold it down if you have alot of repeats).


Tab Magic
-----------------


Basic Control Key Commands
--------------------------

File Tab Commands
-----

Select Commands
-----

Movement Commands
-----

Ctags / Exuberant Tags
-----

Delete, Cut, Copy and Paste Commands
-----

Find and Replace Commands
-----

Line Swap Commands
-----

Indent and Align Commands
-----

Center Cursor Commands
-----

Comment Commands
-----

Upper / Lower Case Commands
-----

Mark Commands
-----

Insert Line Before / After Commands
-----

Page Up / Down Commands
-----

Remove Tabs and Spaces
-----

Configuration Commands
-----

Misc Commands
-----


Repeat Magic
-----------


Moving Around
-----------


Terminal/Console Limitations
--------------------

### Control Keys are Case Insensitive

The terminal maps upper and lower case <kbd>Ctrl</kbd>
key combinations to the same value.  So Lued can't
tell the difference.  For example, <kbd>Ctrl+d</kbd> (used by
Sublime to select a word) and <kbd>Shift+Ctrl+D</kbd>
(used by Sublime to duplicate a line) look the same to Lued.

Note, the <kbd>Alt</kbd> key combinations **are** case sensitive.


<hr style="margin-top:4em;">







