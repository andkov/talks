
<style type="text/css">
.small-code pre code {
   font-size: 1.1em;
}
</style>


Scientific Collaboration with GitHub
========================================================
author: Andrey Koval
date:  Jan 19, 2017
autosize: true

[Hawai<U+02BB>i Institute of Marine Biology](http://www.himb.hawaii.edu/about-us/contact/)


Context links
=======================
- my github page : [github.com/andkov](https://github.com/andkov)
- IALSA organization : [github.com/IALSA](https://github.com/IALSA)
- Centre on Aging colloquium on reproducible science [video](https://www.popdata.bc.ca/events/OAHColloquium_2014), [slides](https://ialsa.github.io/COAG-colloquium-2014F/)
- please see the [full version](https://rawgit.com/OuhscBbmc/BbmcResources/master/Publications/Presentation2015-08-GitHub/beasley-github-2015-08.html)  of this presentation by the orignal author, Will Beasley

Overview of Git
========================================================
**Git** is the underlying **version control system**.  It's  similar to 'Track Changes' in MS Word, with three huge differences:

1. Collaborators can make changes simultaneously. Track Changes frequently involves a painful cognitive load to  reconcile different versions.
2. The entire history is accessible -not just the most recent version. At anytime, you can turn back the clock to any committed change ([example](https://github.com/IALSA/IALSA-2015-Portland/commits/master)).
3. Coordinates an entire repository of files, not just isolated documents.

Overview of GitHub
========================================================
**GitHub** is an online service that leverages Git, and adds some sauce for scientists
* Hosts the repository online.
    * Code.
    * Data.
    * Reports & output.
* Adds options for user permissions, such as read-only<br/>(unlike Dropbox).
* Tools for visualizing code differences and developer activity.
* Project Management Tracking, "Issues", & notifications.

Outline
========================================================
1. Benefits Complete examples.
2. Creation and organization.
3. Communicate with statisticians and non-statisticians.

Benefits
========================================================
* Reproducibility for internal team.
* RAnalysisSkeleton : stencil repo
* Hosting reports.


Complete examples
========================================================
### Academic
* [github.com/IALSA/IALSA-2015-Portland](https://github.com/IALSA/IALSA-2015-Portland)
* [github.com/IALSA/ialsa-2016-terminal-decline](https://github.com/IALSA/ialsa-2016-terminal-decline)
* [github.com/andkov/fear-of-childbirth](https://github.com/andkov/fear-of-childbirth)

### Hobby
* [github.com/andkov/gitRmusic](https://github.com/andkov/gitRmusic)
* [github.com/kona-beer](https://github.com/andkov/kona-beer)
* [github.com/andkov/gin-n-tonic-2016](https://github.com/andkov/gin-n-tonic-2016)
* [github.com/andkov/Pinot-Noir](https://github.com/andkov/Pinot-Noir)



Reproducibility for Internal Team
========================================================
* Easier to be disciplined about:
    * maintaining a current & coherent code base.
    * *programmatic* data manipulation (instead of *manual*).
    * encapsulating analyses in different files.
* Team members can more easily review and synchronize changes.
* Easier to jump between computers.
* [github.com/OuhscBbmc/DeSheaToothakerIntroStats](https://github.com/OuhscBbmc/DeSheaToothakerIntroStats) quickly becomes a small website.

Reproducibility for Outsiders
========================================================
* The inputs (ie, data and code) can be inspected & downloaded immediately.
    * Details too trivial for your article are available too.
* The outputs (ie, stats, graphs, and reports) can be compared to their results.
* Ideally the exactly software versions are easily determined.

Benefits of Hosting Reports
========================================================
* Single URL to send to anyone interested<br/>(not just those with access to the OU file server).
* Single report to send anyone<br/>(not a bunch of loose graphic files).


RAnalysisSkeleton Repository
========================================================
This is minimal example that contains elements of most of my moderately sized projects (say, takes a few weeks start to finish).

https://github.com/wibeasley/RAnalysisSkeleton.

We'll return to this after we finish the slides.

Project Management and Communication
========================================================
* Communicate with internal and external collaborators.
* Three forms of communication have their place.
    1. Long-term documentation stored in the repository.  It should outlive GitHub.
    2. Email has private/internal thoughts & criticisms.
    3. GitHub issues host publically acceptable thoughts & criticisms.  Treat as public.  Don't assume GitHub will be in business in three years; forntunately the code & reports aren't tied to GitHub.  
* Example issues: [developing graphs](https://github.com/IALSA/IALSA-2015-Portland/issues/159) and [compile tables](https://github.com/IALSA/IALSA-2015-Portland/issues/143).

Distributing/Hosting Static Reports
========================================================
The [markdown report](https://github.com/wibeasley/RAnalysisSkeleton/blob/master/Analyses/Report1/Report1.md) is a quick way, but has narrow margins.

For *public* repositories, routing the [html report](https://rawgit.com/wibeasley/RAnalysisSkeleton/master/analysis/report_1/report_1.html) through `http://rawgit.com` is typically better.

For private reports, `knitr` produces a self-contained html report.  The graphics, text, and numeric output is in a single file you can email.  Anyone with a modern browser can open the file.

Inspecting the **diffs** is a great way to see if the results changed over time.


Resources
========================================================
### Git and GitHub Mechanics
 * http://git-scm.com/
 * https://help.github.com/
 * [Version Control with Git](http://shop.oreilly.com/product/0636920022862.do), Loeliger & McCullough (2012)
 * ? [Introducing GitHub: a Non-Technical Guide](http://shop.oreilly.com/product/0636920033059.do), Bell & Beer (2014)

### [Implementing Reproducible Research](http://www.crcpress.com/product/isbn/9781466561595)
 * Victoria Stodden, Friedrich Leisch, Roger D. Peng (editors; 2014)

### [Reproducible Research with R and RStudio](http://christophergandrud.github.io/RepResR-RStudio/)
 * Christopher Gandrud (2013, 2015)
