# lintpre

A simple package to lint typescript files with eslint and format all sorts of source files with prettier.

I haven't put much time to this yet, but it's a start.

I'm testing out, on a really low-endd computer, different types of coding setups and not all the text editors have builtin language support,

So I figured out I'd put together something local that I can run from the cli regardlesss of the editor.

I bet vi(m) and emacs have this stuff figured out but I am not that hardcore. Gotta point and click occcasionally
to keep the mouse hand warm :).

#### Notes
Intriguing why config file options don't seem to work. I want tabs instead of spaces so had to add --use-tabs switch
to the prettier script lines.

While I did get the eslint to work previously, it's now popping up warning `warning  File ignored because outside of base path
` :). I worked around this by symlinking the file to the lintpre directory. This is of course rather not good. putting 
..-notation path as a parameter to it doesn't work either.

Mounting the sshfs directory under this directory works too and is enough for my usage. Sort of suboptimal solution, but it'll
do until something I can figure out something better :).
