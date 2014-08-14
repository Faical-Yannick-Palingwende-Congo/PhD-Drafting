Scientific computing is experiencing a crisis in terms or reproducible
research. For the vast majority of scientific computing papers it is a
difficult task and sometimes impossible (X%, see [X, Y, Z]) to
reproduce the results in the paper independently from the original
authors. The need for better tools for reproducible research is acute
and is currently being addressed by a number of open science advocates
and developers [e.g. X with Z project] with new tools, standards and
procedures to make reproducibility part of the entire scientific
workflow.

The majority of new tools being advocated and developed for open and
reproducible research are concerned with data storage, analysis and
provenance along with workflow, version control and dissemination
tools [Authorea, Figshare, X, Y, Z]. These tools address the important
area of post data generation analysis and distribution, which have
until now been missing from the canonical scientific computing stack.
However, most of these tools are not addressing the overriding concern
of how the data is generated. This concern is intimately tied to the
concept of event control, which is distinct from both version control
and workflow tools. Event control is concerned with the management of
numerical simulations. The idea that each unique computational job (or
simulation) is launched with a unique ID (independent from the unique
ID for the code version) and as much of the meta-data as possible
surrounding that job is recorded. It is this meta-data that must be
distributed in order to make the generation of data reproducible.

This research is concerned with event control, the act of maintaining
records for each simulation and the computational environment and then
making these records easily available to others. This is a necessary
step in making software execution reproducible, but not
sufficient. This research will be concerned with two main issues:

 * The accurate capture of a computational environment for an arbitrary
   job across multiple architectures in both serial and parallel,
   mainly in Python but possibly in other programming
   languages. Progress in this area has been limited, but tools such
   as Sumatra and research by X show some early promise.

 * The issue of disseminating and sharing event control records via a
   distributed event control system and cloud based storage. This
   necessitates the use of a client/server model for capturing events.

A third more difficult goal of the research is to enable the
reproduction of a simulation from the records captured by the event
control system. This is a difficult and time consuming problem,
evidenced by [X, Y, Z].

[1]: Automated Simulation Management and Reproducible Research, Daniel
Wheeler,
http://wd15.github.io/2014/06/25/automated-simulation-management/

[2]: Imagine, C. Titus Brown, http://ivory.idyll.org/blog/2014-imagine.html

[3]: Implementing Reproducible Research: Victoria Stodden, Friedrich
Leisch, Roger D. Peng, https://osf.io/s9tya/wiki/home/
