# Shell Scripting resources

## ShellCheck

Check your scripts with ShellCheck, a static analyzer that supports the popular
Bourne-style shells. This can be used online or installed on your computer, and
it is a useful and important tool for scripters of all skill levels. Any shell
script worth writing in the first place is probably worth checking with
ShellCheck. Shell scripting languages are interpreted, so without static
analysis you don&lsquo;t even have the benefit of seeing if your code will
compile.

- https://www.shellcheck.net/

## Wooledge

Several unofficial guides and FAQs for Bash and other Bourne-style shell
scripting languages are frequently recommended. But shell scripting is trickier
than people tend to think, even experienced people, even experienced people who
are trying to account for how tricky it is. Most unofficial guides, and even
many unofficial (yet reputably published) books, are bad. I recommend the
resources at Greg&lsquo;s wiki. There are no other unofficial FAQs, guides,
tutorials, or walkthroughs that I would recommend (but there are some other
resources, official and not, that I do recommend &ndash; see below). The
BashGuide is a possible place to start (but see below about the Bash reference
manual). Definitely also read (or skim) BashPitfalls.

- http://mywiki.wooledge.org/

## On subshells&hellip;

Subshells are an enormous point of confusion for novice shell scripters. A
subprocess (also known as a child process) that happens to be a shell is not
necessarily a subshell. In particular, if you run `bash` from a Bash prompt,
that child shell is a subprocess of the shell you used to run it, but it is not
a subshell. Subshells inherit and retain the full environment of their parent
shell, including shell variables that are not exported as environment
variables. Child processes that are not subshells, including child shells that
are not subshells, only get environment variables, i.e., exported variables. A
variable that is not inherited as an environment variable, and that is not
exported to make it one, is just a shell variable, and is not an environment
variable, and it does not appear in the environment of a non-subshell
subprocess. One factor that contributes to the confusion is that, when a shell
runs an external command, it may call fork() to create a subshell. However, the
environment of that subshell is sanitized of non-exported variables before an
exec()-family function is called to run the external command. Once the external
command is actually running, the subprocess is NOT a subshell anymore. I
don&lsquo;t know of any good way to explain this, really! This paragraph is a
somewhat technical explanation. Greg&lsquo;s wiki has a more accessible
explanation, with examples:

- https://mywiki.wooledge.org/SubShell

## GNU Bash Reference Manual

The Bash reference manual, an official resource, is remarkably good and fairly
accessible. Note that different versions of Bash do differ somewhat in their
features. Note also that this is NOT the same document as the manpage (`man
bash`), though that is also somewhat useful. I recommend anyone who writes Bash
scripts regularly, or any Bash scripts where quality is important, read this
all the way through at least once (in order or otherwise). If at first you
don&lsquo;t grok it, you may want to use sources on Greg&lsquo;s wiki first and
then return to it. But if you can read and understand it before anything else,
great! It is also valuable as a reference. To view the Bash reference manual in
a terminal, run `info bash` But you&lsquo;ll likely prefer it in HTML or PDF:

- https://www.gnu.org/software/bash/manual/

## POSIX - Shell Command Language

The &ldquo;Shell Command Language&rdquo; chapter in POSIX standardizes the
minimum requirements of POSIX-compatible shells. It is a somewhat difficult
read, but far less so than many language standards. I recommend reading or at
least skimming it, at some point. It is valuable as a reference when you need
to know specifically what features POSIX requires, but it&lsquo;s less
accessible (even as a reference) than the Bash reference manual.

- http://pubs.opengroup.org/onlinepubs/9699919799/utilities/V3_chap02.html

## Stack Exchange

Some Stack Exchange sites have good questions and answers about shell
scripting. The highest quality and greatest technical depth is usually on the
Unix & Linux Stack Exchange, with Ask Ubuntu and Stack Overflow as runners-up.
Check relevant tags (like the bash tag) as well as searching.

- https://unix.stackexchange.com/
- https://askubuntu.com/
- https://stackoverflow.com/

Stéphane Chazelas (whom you may know of as he discovered Bashdoor/Shellshock)
and Gilles are extraordinarily knowledgeable about shells (as well as Unix-like
operating system topics in general), even compared to other famous experts.
Chazelas, in particular, probably knows more about Bourne-style shells than
than anyone else ever has, or will, for generations. Unix & Linux Stack
Exchange has succeeded in part because it has attracted them and they have
written numerous good answers.

- https://unix.stackexchange.com/users/22565/st%C3%A9phane-chazelas
- https://unix.stackexchange.com/users/885/gilles

In that vein, you may want to start with &ldquo;Why is using a shell loop to
process text considered bad practice?&rdquo; by Stéphane Chazelas. This is very
useful because it explains the important ways shell scripting languages differ
from other programming languages in terms of how they work and should be used.

- https://unix.stackexchange.com/q/169716

## On how shell scripting languages are different&hellip;

Shell scripting languages are primarily glue languages and that is the way they
are best used. There may be an external command, like find or grep, that suits
a subtask that you might otherwise be tempted to code via loops or other raw
shell logic. If not, strongly consider using a domain-specific or general
scripting language to implement your subtask. Domain-specific languages that
come in handy include awk, sed, and (less frequently) bc. Those commands are
required by POSIX (though in practice bc is often not installed). General-
purpose scripting languages that come in handy include Python and Perl (which
aren&lsquo;t required by POSIX but are usually installed on Unix-like systems).
Mind the difference between Python 2 and Python 3. Even if you know your shell
and don&lsquo;t know a scripting language that would be good for your task if
you did know it, it&lsquo;s STILL often better to learn a bit of the scripting
language and use it. Although there&lsquo;s quite a bit that can be done in
&ldquo;pure shell,&rdquo; at least with feature-rich shells like Bash, this is
an unidiomatic and typically inferior way to write shell scripts.
&ldquo;Knowing&rsquo; shell scripting means knowing how to use common external
commands like those mentioned above, though for language interpreters that is
not necessarily the same as really knowing them as whole languages. In effect,
the &ldquo;standard library&rdquo; of the shell command language consists of
all the other utilities that POSIX requires to be present. The POSIX toolset is
big enough that it is easy to get dispirited about knowledge one doesn&lsquo;t
(or doesn&lsquo;t yet) possess, but remember that even partial proficiency goes
a long way. That shells are glue languages mandates familiarity with standard
external commands but also makes it far less important than it otherwise would
be to keep sharp on the arcane technicalities that plague the shells
themselves.

## HackerRank (for practice only)

I don&lsquo;t recommend HackerRank as an initial learning resource for shell
scripting, but once you have some familiarity, you can try doing all the
&ldquo;Linux Shell&rdquo; exercises. Also, many (perhaps all) of the Regex
exercises, in the Applications subdomain, can be used for Bash scripting
practice. (Remember that you can, and usually should, use external tools like
grep, sed, and awk.)

- https://www.hackerrank.com/domains/shell
- https://www.hackerrank.com/domains/regex

## Regex

Regular expressions come up a lot in shell scripting. They also have various
other applications in programming. If you don&lsquo;t know regex, I recommend
reading the grep manpage, followed by this site, which is also a good
reference:

- https://www.regular-expressions.info/
