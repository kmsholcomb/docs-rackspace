# Contributor guidelines

These guidelines provide the general process for maintaining source code that
builds the Rackspace Cloud Files developer documentation.

- [Project description](#project-description)
- [Updating and adding content](#updating-and-adding-content)
- [General style guidelines](#general-style-guidelines)
- [Submitting your content](#submitting-changes)
- [Previewing changes](#previewing-changes)

## Project description
<!-- Provide as little or as much information about architecture as needed to
help contributors figure out which file to update.-->

This project is developed and built by using the
[Python Sphinx documentation generator](http://sphinx-doc.org/).
Content is written in [reStructuredText](http://sphinx-doc.org/rest.html),
which is the markup syntax and parser component of
[Python Docutils](http://docutils.sourceforge.net/index.html).

Source files for the Sphinx documentation project are in the ``api-docs``
directory. Following are the key files that define project and content
architecture:

```eval_rst
.. list-table::
   :widths: 50 50
   :header-rows: 1

   * - Cont
     - File   * - ent
     -
   * - Inde
     - `ind   * - x
     - ex.r   * - page
     - st <   * - for
     - http   * - the
     - s://   * - main
     - gith   * - cont
     - ub.c   * - ent
     - om/r   * - stru
     - acke   * - ctur
     - rlab   * - e
     - s/do   * - 
     - cs-c   * - 
     - loud   * - 
     - -fil   * - 
     - es/b   * - 
     - lob/   * - 
     - mast   * - 
     - er/a   * - 
     - pi-d   * - 
     - ocs/   * - 
     - inde   * - 
     - x.rs   * - 
     - t>`_   * - 
     - _
   * - Abou
     - `ove   * - t
     - rvie   * - the
     - w/in   * - API
     - dex.   * - inde
     - rst   * - x
     - <htt   * - 
     - ps:/   * - 
     - /git   * - 
     - hub.   * - 
     - com/   * - 
     - rack   * - 
     - erla   * - 
     - bs/d   * - 
     - ocs-   * - 
     - clou   * - 
     - d-fi   * - 
     - les/   * - 
     - blob   * - 
     - /mas   * - 
     - ter/   * - 
     - api-   * - 
     - docs   * - 
     - /ove   * - 
     - rvie   * - 
     - w/in   * - 
     - dex.   * - 
     - rst>   * - 
     - `__
   * - Gett
     - `get   * - ing
     - ting   * - Star
     - -sta   * - ted
     - rted   * - intr
     - .rst   * - oduc
     - <ht   * - tion
     - tps:   * - 
     - //gi   * - 
     - thub   * - 
     - .com   * - 
     - /rac   * - 
     - kerl   * - 
     - abs/   * - 
     - docs   * - 
     - -clo   * - 
     - ud-f   * - 
     - iles   * - 
     - /blo   * - 
     - b/ma   * - 
     - ster   * - 
     - /api   * - 
     - -doc   * - 
     - s/ge   * - 
     - ttin   * - 
     - g-st   * - 
     - arte   * - 
     - d.rs   * - 
     - t>`_   * - 
     - _
   * - Gett
     - `get   * - ing
     - ting   * - Star
     - -sta   * - ted
     - rted   * - inde
     - /ind   * - x
     - ex.r   * - 
     - st <   * - 
     - http   * - 
     - s://   * - 
     - gith   * - 
     - ub.c   * - 
     - om/r   * - 
     - acke   * - 
     - rlab   * - 
     - s/do   * - 
     - cs-c   * - 
     - loud   * - 
     - -fil   * - 
     - es/b   * - 
     - lob/   * - 
     - mast   * - 
     - er/a   * - 
     - pi-d   * - 
     - ocs/   * - 
     - gett   * - 
     - ing-   * - 
     - star   * - 
     - ted/   * - 
     - inde   * - 
     - x.rs   * - 
     - t>`_   * - 
     - _
   * - Deve
     - `dev   * - lope
     - elop   * - r
     - er-g   * - Guid
     - uide   * - e
     - .rst   * - intr
     - <ht   * - oduc
     - tps:   * - tion
     - //gi   * - 
     - thub   * - 
     - .com   * - 
     - /rac   * - 
     - kerl   * - 
     - abs/   * - 
     - docs   * - 
     - -clo   * - 
     - ud-f   * - 
     - iles   * - 
     - /blo   * - 
     - b/ma   * - 
     - ster   * - 
     - /api   * - 
     - -doc   * - 
     - s/de   * - 
     - velo   * - 
     - per-   * - 
     - guid   * - 
     - e.rs   * - 
     - t>`_   * - 
     - _
   * - Conc
     - `con   * - epts
     - cept   * - sect
     - s.rs   * - ion
     - t <h   * - 
     - ttps   * - 
     - ://g   * - 
     - ithu   * - 
     - b.co   * - 
     - m/ra   * - 
     - cker   * - 
     - labs   * - 
     - /doc   * - 
     - s-cl   * - 
     - oud-   * - 
     - file   * - 
     - s/bl   * - 
     - ob/m   * - 
     - aste   * - 
     - r/ap   * - 
     - i-do   * - 
     - cs/c   * - 
     - once   * - 
     - pts.   * - 
     - rst>   * - 
     - `__
   * - Gene
     - `gen   * - ral
     - eral   * - API
     - -api   * - info
     - -inf   * - rmat
     - o/in   * - ion
     - dex.   * - inde
     - rst   * - x
     - <htt   * - 
     - ps:/   * - 
     - /git   * - 
     - hub.   * - 
     - com/   * - 
     - rack   * - 
     - erla   * - 
     - bs/d   * - 
     - ocs-   * - 
     - clou   * - 
     - d-fi   * - 
     - les/   * - 
     - blob   * - 
     - /mas   * - 
     - ter/   * - 
     - api-   * - 
     - docs   * - 
     - /gen   * - 
     - eral   * - 
     - -api   * - 
     - -inf   * - 
     - o/in   * - 
     - dex.   * - 
     - rst>   * - 
     - `__
   * - API
     - `api   * - Refe
     - -ref   * - renc
     - eren   * - e
     - ce.r   * - intr
     - st <   * - oduc
     - http   * - tion
     - s://   * - 
     - gith   * - 
     - ub.c   * - 
     - om/r   * - 
     - acke   * - 
     - rlab   * - 
     - s/do   * - 
     - cs-c   * - 
     - loud   * - 
     - -fil   * - 
     - es/b   * - 
     - lob/   * - 
     - mast   * - 
     - er/a   * - 
     - pi-d   * - 
     - ocs/   * - 
     - api-   * - 
     - refe   * - 
     - renc   * - 
     - e.rs   * - 
     - t>`_   * - 
     - _
   * - API
     - `sto   * - Refe
     - rage   * - renc
     - -api   * - e
     - -ope   * - inde
     - rati   * - x
     - ons/   * - for
     - inde   * - stor
     - x.re   * - age
     - st <   * - oper
     - http   * - atio
     - s://   * - ns
     - gith   * - 
     - ub.c   * - 
     - om/r   * - 
     - acke   * - 
     - rlab   * - 
     - s/do   * - 
     - cs-c   * - 
     - loud   * - 
     - -fil   * - 
     - es/b   * - 
     - lob/   * - 
     - mast   * - 
     - er/a   * - 
     - pi-d   * - 
     - ocs/   * - 
     - stor   * - 
     - age-   * - 
     - api-   * - 
     - oper   * - 
     - atio   * - 
     - ns/i   * - 
     - ndex   * - 
     - .rst   * - 
     - >`__
   * - API
     - `cdn   * - Refe
     - -api   * - renc
     - -ope   * - e
     - rati   * - inde
     - ons/   * - x
     - inde   * - for
     - x.rs   * - CDN
     - t <h   * - oper
     - ttps   * - atio
     - ://g   * - ns
     - ithu   * - 
     - b.co   * - 
     - m/ra   * - 
     - cker   * - 
     - labs   * - 
     - /doc   * - 
     - s-cl   * - 
     - oud-   * - 
     - file   * - 
     - s/bl   * - 
     - ob/m   * - 
     - aste   * - 
     - r/ap   * - 
     - i-do   * - 
     - cs/c   * - 
     - dn-a   * - 
     - pi-o   * - 
     - pera   * - 
     - tion   * - 
     - s/in   * - 
     - dex.   * - 
     - rst>   * - 
     - `__
   * - API
     - `sto   * - oper
     - rage   * - atio
     - -api   * - ns
     - -ope   * - meth
     - rati   * - ods
     - ons/   * - for
     - meth   * - stor
     - ods   * - age,
     - <htt   * - incl
     - ps:/   * - udin
     - /git   * - g
     - hub.   * - code
     - com/   * - samp
     - rack   * - les
     - erla   * - 
     - bs/d   * - 
     - ocs-   * - 
     - clou   * - 
     - d-fi   * - 
     - les/   * - 
     - tree   * - 
     - /mas   * - 
     - ter/   * - 
     - api-   * - 
     - docs   * - 
     - /sto   * - 
     - rage   * - 
     - -api   * - 
     - -ope   * - 
     - rati   * - 
     - ons/   * - 
     - meth   * - 
     - ods>   * - 
     - `__
   * - API
     - `cdn   * - oper
     - -api   * - atio
     - -ope   * - ns
     - rati   * - meth
     - ons/   * - ods
     - meth   * - for
     - ods   * - CDN,
     - <htt   * - incl
     - ps:/   * - udin
     - /git   * - g
     - hub.   * - code
     - com/   * - samp
     - rack   * - les
     - erla   * - 
     - bs/d   * - 
     - ocs-   * - 
     - clou   * - 
     - d-fi   * - 
     - les/   * - 
     - tree   * - 
     - /mas   * - 
     - ter/   * - 
     - api-   * - 
     - docs   * - 
     - /cdn   * - 
     - -api   * - 
     - -ope   * - 
     - rati   * - 
     - ons/   * - 
     - meth   * - 
     - ods>   * - 
     - `__
   * - Spec
     - `use   * - ial
     - -cas   * - Use
     - es-i   * - Case
     - nfor   * - s
     - mati   * - intr
     - on.r   * - oduc
     - st <   * - tion
     - http   * - 
     - s://   * - 
     - gith   * - 
     - ub.c   * - 
     - om/r   * - 
     - acke   * - 
     - rlab   * - 
     - s/do   * - 
     - cs-c   * - 
     - loud   * - 
     - -fil   * - 
     - es/b   * - 
     - lob/   * - 
     - mast   * - 
     - er/a   * - 
     - pi-d   * - 
     - ocs/   * - 
     - use-   * - 
     - case   * - 
     - s-in   * - 
     - form   * - 
     - atio   * - 
     - n.rs   * - 
     - t>`_   * - 
     - _
   * - Stat
     - `sta   * - ic
     - tic-   * - webs
     - webs   * - ites
     - ites   * - usin
     - -usi   * - g
     - ng-c   * - CDN-
     - dn-e   * - enab
     - nabl   * - led
     - ed-c   * - cont
     - onta   * - aine
     - iner   * - rs
     - s/in   * - 
     - dex.   * - 
     - rst   * - 
     - <htt   * - 
     - ps:/   * - 
     - /git   * - 
     - hub.   * - 
     - com/   * - 
     - rack   * - 
     - erla   * - 
     - bs/d   * - 
     - ocs-   * - 
     - clou   * - 
     - d-fi   * - 
     - les/   * - 
     - blob   * - 
     - /mas   * - 
     - ter/   * - 
     - api-   * - 
     - docs   * - 
     - /sta   * - 
     - tic-   * - 
     - webs   * - 
     - ites   * - 
     - -usi   * - 
     - ng-c   * - 
     - dn-e   * - 
     - nabl   * - 
     - ed-c   * - 
     - onta   * - 
     - iner   * - 
     - s/in   * - 
     - dex.   * - 
     - rst>   * - 
     - `__
   * - Bulk
     - `bul   * - oper
     - k-op   * - atio
     - erat   * - ns
     - ions   * - 
     - /ind   * - 
     - ex.r   * - 
     - st <   * - 
     - http   * - 
     - s://   * - 
     - gith   * - 
     - ub.c   * - 
     - om/r   * - 
     - acke   * - 
     - rlab   * - 
     - s/do   * - 
     - cs-c   * - 
     - loud   * - 
     - -fil   * - 
     - es/b   * - 
     - lob/   * - 
     - mast   * - 
     - er/a   * - 
     - pi-d   * - 
     - ocs/   * - 
     - bulk   * - 
     - -ope   * - 
     - rati   * - 
     - ons/   * - 
     - inde   * - 
     - x.rs   * - 
     - t>`_   * - 
     - _
   * - Publ
     - `pub   * - ic
     - lic-   * - acce
     - acce   * - ss
     - ss-t   * - to
     - o-yo   * - your
     - ur-c   * - Clou
     - loud   * - d
     - -fil   * - File
     - es-a   * - s
     - ccou   * - acco
     - nt/i   * - unt
     - ndex   * - 
     - .rst   * - 
     - <ht   * - 
     - tps:   * - 
     - //gi   * - 
     - thub   * - 
     - .com   * - 
     - /rac   * - 
     - kerl   * - 
     - abs/   * - 
     - docs   * - 
     - -clo   * - 
     - ud-f   * - 
     - iles   * - 
     - /blo   * - 
     - b/ma   * - 
     - ster   * - 
     - /api   * - 
     - -doc   * - 
     - s/pu   * - 
     - blic   * - 
     - -acc   * - 
     - ess-   * - 
     - to-y   * - 
     - our-   * - 
     - clou   * - 
     - d-fi   * - 
     - les-   * - 
     - acco   * - 
     - unt/   * - 
     - inde   * - 
     - x.rs   * - 
     - t>`_   * - 
     - _
   * - Rele
     - `rel   * - ase
     - ease   * - note
     - -not   * - s
     - es.r   * - 
     - st <   * - 
     - http   * - 
     - s://   * - 
     - gith   * - 
     - ub.c   * - 
     - om/r   * - 
     - acke   * - 
     - rlab   * - 
     - s/do   * - 
     - cs-c   * - 
     - loud   * - 
     - -fil   * - 
     - es/b   * - 
     - lob/   * - 
     - mast   * - 
     - er/a   * - 
     - pi-d   * - 
     - ocs/   * - 
     - rele   * - 
     - ase-   * - 
     - note   * - 
     - s.rs   * - 
     - t>`_   * - 
     - _
   * - Sphi
     - `con   * - nx
     - f.py   * - docu
     - <ht   * - ment
     - tps:   * - atio
     - //gi   * - n
     - thub   * - conf
     - .com   * - igur
     - /rac   * - atio
     - kerl   * - n
     - abs/   * - file
     - docs   * - 
     - -clo   * - 
     - ud-f   * - 
     - iles   * - 
     - /blo   * - 
     - b/ma   * - 
     - ster   * - 
     - /api   * - 
     - -doc   * - 
     - s/co   * - 
     - nf.p   * - 
     - y>`_   * - 
     - _   * - 
     - (Typ   * - 
     - ical   * - 
     - ly,   * - 
     - this   * - 
     - file   * - 
     - does   * - 
     - not   * - 
     - requ   * - 
     - ire   * - 
     - chan   * - 
     - ges.   * - 
     - )
   * - Linu
     - ``Ma   * - x
     - kefi   * - and
     - le``   * - OS X
     -   * - buil
     -   * - d
     -   * - scri
     -   * - pt
     -
   * - Wind
     - ``ma   * - ows
     - ke.b   * - buil
     - at``   * - d
     -   * - scri
     -   * - pt
     -

```

## Updating and adding content

Contributions are submitted, reviewed, and accepted by using GitHub
pull requests, following the [GitHub workflow](GITHUBING.md) for this
repository.

To update existing source files or add new ones, follow the
[GitHub workflow](GITHUBING.md) for this repository.

* Update source files by using the GitHub editor or any plain text editor.
* Format source files with
  [reStructuredText syntax](http://www.sphinx-doc.org/en/stable/rest.html).
* For quick syntax checking, try the
[Online reStructuredText editor](http://rst.ninjs.org/).

## General style guidelines

When you add or update content, use the following general style guidelines,
which are described in detail in [Style guidelines for technical content](https://github.com/rackerlabs/docs-rackspace/blob/master/doc/style-guide/README.md):

- Use [sentence-style capitalization](https://github.com/rackerlabs/docs-rackspace/blob/master/doc/style-guide/a-l-style-guidelines.md#guidelines-for-sentence-style-capitalization) for titles and headings
- Use consistent [text formatting](https://github.com/rackerlabs/docs-rackspace/blob/master/doc/style-guide/m-z-style-guidelines.md#text-formatting)
- Write clear and consistent [code examples](https://github.com/rackerlabs/docs-rackspace/blob/master/doc/style-guide/a-l-style-guidelines.md#code-examples)
- Use [active voice](https://github.com/rackerlabs/docs-rackspace/blob/master/doc/style-guide/basic-writing-guidelines.md#use-active-voice)
- Use [present tense](https://github.com/rackerlabs/docs-rackspace/blob/master/doc/style-guide/basic-writing-guidelines.md#use-present-tense)
- Write to the user by using [second person and imperative mood](https://github.com/rackerlabs/docs-rackspace/blob/master/doc/style-guide/basic-writing-guidelines.md#write-to-the-user-by-using-second-person-and-imperative-mood)
- Use numbered lists for instructions, and write clear [step text](https://github.com/rackerlabs/docs-rackspace/blob/master/doc/style-guide/m-z-style-guidelines.md#procedural-steps)
- Clarify [pronouns](https://github.com/rackerlabs/docs-rackspace/blob/master/doc/style-guide/basic-writing-guidelines.md#clarify-pronouns) such as *it*, *this*, *there*, and *that*
- Clarify [gerunds and participles](https://github.com/rackerlabs/docs-rackspace/blob/master/doc/style-guide/basic-writing-guidelines.md#clarify-gerunds-and-participles)
- Use [consistent terminology](https://github.com/rackerlabs/docs-rackspace/blob/master/doc/style-guide/basic-writing-guidelines.md#use-consistent-terminology)

<!-- Adding build from source guidelines until we can provide a link to
automated gh-pages output, or to the staging URL that Ash is working on. -->

## Submitting changes

When you've completed your changes, submit a pull request. Someone on the
Information Development team will review your PR.

- Minor updates and corrections get a quick review to ensure that content is
  error-free and doesn't introduce other issues.
- More complex changes or additions require both technical and editorial
  review.

Depending on the review feedback, you might be asked to make additional
changes.

After content has been reviewed and approved, the updates can be merged to the
master branch. The merge triggers the build and deploy process. Typically, new
content is available on developer.rackspace.com within a minute or two after it
is merged. Larger updates might take a bit longer.

## Previewing changes

When you submit a pull request, the Strider build process creates
a preview of your changes in a staging environment. After the build
process completes, the following message displays in the pull request
comments with a link to the content: ``Your content preview is now ready.``

You can also build the project locally using the
[Sphinx documentation generator](http://sphinx-doc.org/). For details, see
[Building from source](https://github.com/rackerlabs/docs-rackspace/blob/master/doc/tools/build-from-source.rst).
