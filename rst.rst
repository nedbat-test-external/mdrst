##########################
ReStructured Text Examples
##########################

Basic Stuff
***********

Emphasis
========

.. note: RST only allows asterisks for emphasis

This word is *italicized*.

Strong emphasis
===============

.. note: RST only allows asterisks for strong emphasis

This word is **bold**.

Code inline
===========

Call the ``function_name`` function.

Code blocks
===========
Look at this output::

   $ ls /usr/
   bin        lib        libexec    local      sbin       share

Look at this code:

.. code-block:: python

    def fib(n):
        if n <= 2:
            return 1
        else:
            return fib(n-1) + fib(n-2)

Blockquotes
===========

Lincoln said:

   Four-score and seven years ago, our fathers
   brought forth on this continent a new nation,
   conceived in Liberty, and dedicated to the
   proposition that all men are created equal.


Lists
*****

Numbered
========

#. First ordered list item
#. Another item
#. Use hash marks for numbers

Bullets
=======

* First unordered list item
* Another item
* And another item

Nested
======

.. note: RST needs blank lines around the inner list.

#. First outer

   * First inner
   * Second inner

#. Second outer
#. Third outer

Links
*****

URLs
====

URLs make links: http://python.org.

Inline
======

`Inline link <http://python.org>`__
for brevity.

Indirect
========

`Indirect link`_
for readability.

.. _Indirect link: http://python.org


Headers
*******

Headers
=======

.. parse-headers-off

.. note: The overlines and characters are flexible in RST as long as they are consistent.  RST requires strict nesting; even after the hierarchy is established, you can't use, say, a third-tier header right under a first-tier whereas MD allows this.

############
First Header
############

Second Header
*************

Third Header
============

Fourth Header
-------------

.. parse-headers-on


Images
******

Images
======

.. image:: xsy_150.png
   :alt: Image of Xsy


Notes etc
*********

Notes
=====

.. note::
   This is the text of a note.

.. note: GitHub's RST rendering doesn't make this stand out much.

Warnings
========

.. warning::
   This is the text of a warning.

.. note: GitHub's RST rendering doesn't make this stand out much.
