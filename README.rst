#####################################
Types and Programming Languages in F#
#####################################

Code and Examples from Benjamin Pierce's "`Types and Programming Languages`_".

.. _`Types and Programming Languages`: http://www.cis.upenn.edu/~bcpierce/tapl/


Overview
========

"`Types and Programming Languages`_" provides a comprehensive introduction to type systems and programming language theory. The code which accompanies the book is written in OCaml; this repository contains an F# port of that code.

**NOTE:** The ported F# code is not a fresh implementation -- it is the *original* OCaml code with some trivial modifications which allow it to compile with F#. The output of each of the F# projects has been verified to match the `output of the original OCaml programs`_.
**NOTE/2:** This is just a review of the original F# to make it compile with VS2017, latest F# and required packages_.

.. _`Types and Programming Languages`: http://www.cis.upenn.edu/~bcpierce/tapl/
.. _`output of the original OCaml programs`: fsharp-tapl/blob/master/expected-output.rst

Prerequisites
=============

- F# compiler

  - Windows

    - Visual Studio 2017

  - Mac OS X / FreeBSD / Linux

    - `fsharp 4.4.3.0`_
  
- NuGet_ is used to manage external packages. The easiest way to `install NuGet`_ is by downloading it (for free) from the `Visual Studio Extension Gallery`_. If you do not have NuGet, or are running a version prior to 2.5, you *must* install it (or upgrade) before you will be able to build the projects.

  The solution uses the *Package Restore* feature of NuGet to automatically download any missing packages when the project is built. This requires that you have the `Allow NuGet to download missing packages during build`_ setting enabled; in Visual Studio, you can find the setting under ``Options -> Package Manager -> General``.

  Once NuGet is installed and configured, you should be able to build the solution.
