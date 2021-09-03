<center><a href="https://summerofcode.withgoogle.com/projects/#5342773319827456"><img src="https://developers.google.com/open-source/gsoc/resources/downloads/GSoC-logo-horizontal.svg" alt="gsoc" height="50"/></a></center>

# Google Summer of Code | Final Work Submission Report

- **Name:** Gavish Poddar
- **Organisation:** Python Software Foundation
- **Sub-Organisation:** Zyte
- **Project:** [`dateparser`](https://github.com/scrapinghub/dateparser)
 Better language detection & reimplementing `search_dates` 
- **Proposal:** [dateparser - better language detection](https://blogs.python-gsoc.org/media/proposals/Dateparser_Better_Language_Detection_1.pdf)

Hello Everyone! My name is Gavish Poddar and I'm excited to tell you about my GSoC journey. For the past couple of months, I have been working on an awesome project `dateparser`. The dateparser aims to parse `datetime` from a string.

My GSoC journey would not have been successful without the guidance of my mentors [Marc Hernández](https://github.com/noviluni), [Konstantin Lopuhin](https://github.com/lopuhin) and [Kishan Mehta](https://github.com/kishan3).

## What I Have Learned?

The whole GSoC journey was full of learning thanks to my mentors. I learned how to find good open source dependencies to include in our project. I tried my hands on improving code coverage and writing tests for the code. I learned how to optimize code and the need for extensive research before feature addition.

## What I Have Contributed?

As mentioned in my proposal I worked on the implementation of the Optional Language Detection for dateparser and fixing as many issues as possible in the `search_dates` function of the [`dateparser`](https://github.com/scrapinghub/dateparser).


### Optional Language Detection
<center><a href="https://github.com/scrapinghub/dateparser/pull/932"><img src="https://img.shields.io/github/pulls/detail/state/scrapinghub/dateparser/932?label=Language%20Detection"/></a></center>

PR - [Optional Language Detection](https://github.com/scrapinghub/dateparser/pull/932)


Implemented optional language detection to improve language detection. This allows to plug in any language detection library with the dateparser. Out of the box, dateparser supports two libraries [`fasttext`](https://github.com/facebookresearch/fastText) and [`langdetect`](https://github.com/Mimino666/langdetect). The optional language detection works with both parse and search_dates. This PR also introduces a new setting `DEFAULT_LANGUAGES` which is used if no language is detected by default language detection and the optional language detection.

### Reimplimenting `search_dates` (extended goal)
<center><a href="https://github.com/scrapinghub/dateparser/pull/945"><img src="https://img.shields.io/github/pulls/detail/state/scrapinghub/dateparser/945?label=Reimplementing search_dates"/></a></center>

PR - [Reimplimenting `search_dates`](https://github.com/scrapinghub/dateparser/pull/945)

A reimplemented and simplified `search_dates` improves the results and fixes many issues. The entire search_dates is newly implemented and would be easier to maintain. This PR introduces a new feature `search_first_date` which returns the first date in the given string. This PR also fixes around **13 issues**.

### Other `search_dates` improvements

<br>

Adding support for date-related objects `last decade`, `next decade`, etc in `search_date`. This PR fixes **1 issue**.

<center><a href="https://github.com/scrapinghub/dateparser/pull/953"><img src="https://img.shields.io/github/pulls/detail/state/scrapinghub/dateparser/953"/></a></center>

PR - [Improvements in locale:translate_search fixes](https://github.com/scrapinghub/dateparser/pull/953)

<br>


Adding support `search_date` period separator support. Date string like `23.12.2000` can be parsed. This PR fixes **5 issues**.

<center><a href="https://github.com/scrapinghub/dateparser/pull/963"><img src="https://img.shields.io/github/pulls/detail/state/scrapinghub/dateparser/963"/></a></center>

PR - [`search_date` period separator support](https://github.com/scrapinghub/dateparser/pull/963)

<br>



## Other Important Details

As part of our GSoC project, Python Software Foundation requires us to post a weekly blog where we usually post about what we have done in the week and what is coming up next. We can also write about any blockages or issues we are facing. I have also written my weekly blogs so if you want to know weekly details of my project you can refer them here.

[ Weekly Blogs](https://blogs.python-gsoc.org/en/gavishpoddars-blog/)

## Future Work and Final Note

The project is very actively maintained the new `search_dates` and my contributions would improve the library. The main goal of the proposal is achived with the implimentation of the optional language detection and the PR is mergeable. I plan to keep working on the project and contribute as much as I can. Contribute to the `search_dates` function of the library ([`dateparser`](https://github.com/scrapinghub/dateparser)) would be my primary goal.

It was overall a wonderful experience and I learned a lot.
----------------------------------------------------------------------------------------------------------------------------

I would like to thank Google, Python Software Foundation and Zyte for providing me with the opportunity and my mentors [Marc Hernández](https://github.com/noviluni), [Konstantin Lopuhin](https://github.com/lopuhin) and [Kishan Mehta](https://github.com/kishan3).