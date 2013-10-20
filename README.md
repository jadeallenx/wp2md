wp2md
=====
This is a simple script to convert Wordpress XML export into a set of 
Markdown formatted files.  Most likely you want to do this to move
your Wordpress content to some kind of static blog system.

Synopsis
--------
```bash
./wp2md ../path/to/wordpress/export/file.xml
```

By default, output is written into a directory called `../md` with a 
simple regex (i.e., replace all non-alphanumerics with '\_') to create
a filename.

Most of the "customization" must be done in the script itself. There are
no command line options at the moment beyond the input filename.

Dependencies
------------
There's a `cpanfile` in the root to fetch dependencies. You will probably 
need to pull HTML::FormatMarkdown from [my github repo](https://github.com/mrallen1/html-format)
until it's [merged upstream](https://github.com/nigelm/html-format/pull/1).

Support
-------
Feel free to open an issue on github if you encounter problems. There's quite
a few things in my output that are semi-specific to the kind of static blog
generator I am working on, so they may not be all that great for you.

License
-------
Copyright (C) 2013 Mark Allen

This is free software; you can redistribute it and/or modify it under 
the same terms as the Perl 5 programming language system itself.
