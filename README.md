This is a pair of scripts that, together, automatically compile a
.scss file as soon that .scss file is updated.

Dart Sass already does this, but Dart Sass isn't available in Debian's
repositories, which is why I made these scripts.

`update-sass` compiles a .scss file if it's newer than a given .css
file.

`monitor-sass` keeps all files in a directory updated by continually
calling `update-sass` on every file in the directory.

I know that's not the most efficient or scalabe method of doing this,
but this script set was just meant to help me when developing small
projects on Debian, or other platforms on which I'm not using a Sass
implementation with the `--watch` flag.  :)