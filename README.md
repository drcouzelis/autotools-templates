# Template files for GNU Autotools

These files provide a template for configuring your software project to use GNU Autotools. Using GNU Autotools will provide you with the standard "./configure && make && make install" installation procedure, used by on various operating systems.

## Usage

Copy the files into the top-level directory of your software project. Edit the examples in the files to match your project (for example, "myappname"), file / directory structure, and libraries used.

Then, run:

    autoreconf --install

to generate the "configure" script.

You are now ready to build your software using GNU Autotools!
