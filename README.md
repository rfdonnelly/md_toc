# md_toc

Table of Contents generation for Markdown.  Add a TOC or maintain an existing TOC.

# Table of Contents

* [U: Usage](#u)
    * [U.notes: Notes](#u-notes)
    * [U.cli: Command Line Interface](#u-cli)
* [I: Inspiration](#i)

# <div id='u'/> U: Usage

md_toc requires a specific heading naming convention.  The heading requires a breadcrumb followed by a colon, a space, and the heading text.

Format:

    #[#[#...]] breadcrumb: heading_text

Example: Symbolic section identifiers

    # U: Usage

    ## U.notes: Notes

Example: Numeric section identifiers

    # 1: Usage

    ## 1.1: Notes

## <div id='u-notes'/> U.notes: Notes

* Files are edited in-place.
* Headings without a breadcrumb will not be added to the TOC.
* Headings without a breadcrumb that occur before any headings with breadcrumbs will be placed before the TOC.  In other words, TOC is placed just before first heading with breadcrumb.

## <div id='u-cli'/> U.cli: Command Line Interface

    md_toc <file.md>

# <div id='i'/> I: Inspiration

The [C++ Core Guidelines](https://github.com/isocpp/CppCoreGuidelines/blob/master/CppCoreGuidelines.md) was inspiration for the heading naming conventions used by md_toc.  After tediously adding and maintaining TOCs several times manually, md_toc was born.