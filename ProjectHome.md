My project provides a mechanism, developed by this author for his own use and enjoyment, to compile and install both Image::Magick (PerlMagick) and the base ImageMagick® compiled code to a non-standard location which does not interfere with any existing PerlMagick or ImageMagick® installation on the system.

_PerlMagick_ is the unconforming name given to the Image::Magick portion of ImageMagick®, the C image display, analysis and manipulation library and tools (http://www.imagemagick.org/script/index.php). It is **uncomforming** in the sense that it is not a package name that Perl users expect - the predictable name would be _Image-Magick_.  Image::Magick/PerlMagick means 'a Perl extension for interfacing to the C library provided by ImageMagick®'. See http://www.imagemagick.org/script/perl-magick.php.

The starting point for using _magickdperl_ is to `apt-get source imagemagick`.

Once this is done, you will add the single GNUmakefile which my project provides, to the top of the source tree, which apt will have created under **.** (your current directory). This source tree top dir should be named _imagemagick-6.3.7.9.dfsg1/_. At the time of starting my project, that is the latest **.deb** available (it is available as a _backport_ as well as for current Debian releases).