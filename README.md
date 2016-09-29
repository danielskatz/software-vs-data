#Software vs Data

Author/Editors:
Daniel S. Katz,
Kyle E. Niemeyer,
Arfon M. Smith

Additional Authors:
William L. Anderson, Carl Boettiger, Konrad Hinsen, Mike Hucka, Frank Löffler, Tom Pollard, Fernando Rios


This repository is intended to be used to discuss and document the differences between software and data in the context of citation in the research record.

It has been created in the process of the FORCE11 Software Citation Working Group<sup id="F11SCWG-footnote">[FORCE11 Software Citation Working Group](#F11SCWG)</sup>
writing the FORCE11 Software Citation Principles<sup id="F11SCWG-web-footnote">[Smith et al. 2016a](#F11SCWG-web)</sup>,
and then the editors submitting them to PeerJ Computer Science<sup id="F11SCWG-PeerJCS-footnote">[Smith et al. 2016b](#F11SCWG-PeerJCS)</sup>
and responding to reviewer comments.

We start with the idea that software, while similar to data in terms of not traditionally having been cited in publications, is also different than data. In the context of research (e.g., in science), the term "data" usually refers to electronic records of observations made in the course of a research study ("raw data") or to information derived from such observations by some form of processing ("processed data"), as well as the output of simulation or modeling software ("simulated data"). In the following, we use the term "data" in this specific sense.

The confusion about the distinction between software and data comes in part from the much wider sense that the term "data" has in computing and information science, where it refers to anything that can be processed by a computer. In that sense, software is just a special kind of data.


The remainder of this document gives examples of these differences.

If you want to add a new difference, please do via a pull request.  Similarly, if you want to add a citation or add a new explanation, please also do this via a pull request.  If you want to discuss a difference (for example, you don't think it's correct), please open a new issue or discuss via an existing issue.  If you do add text in a pull request, also add yourself as an additional author in that same request, following the existing format and keeping the additional author list in alphabetic order by surname. (And add a comma after all authors but the last one.)

---

##Format of this document:

###Statement

Explanation if needed

Evidence: Citations

---

##List of Differences

###Software is executable, unlike papers or data.

A commonsense definition of software is that it is "a set of instructions that direct a computer to do a specific task" <sup id="chun2004-footnote">[Chun 2004](#chun2004)</sup>. On the other hand, data is simply a collection of facts or measurements (real or simulated). Of course, software can be considered data as well, especially if viewed as a collection of facts. However, from the point of view of conducting research with software, the main difference is that software is associated with action: knowledge creation, information transformation, visualization, etc.  An action can be thought of joining two states of data: a "before" (e.g., input files, parameter settings, unstructured or tacit information) to an "after" state (e.g., output files, transformed data, structured knowledge). If we accept the definitions of software and data given at the begining of this section, then (at least in scientific research), the difference between data and software can be summarized by the statement of <sup id="matthews2010-footnote">[Matthews et al. 2010](#matthews2010)</sup>: "we are more interested in what software *does* rather than what software *is*."

###Data provides evidence, software provides a tool.

Software exists to perform a task, data does not. Data is fundamentally an *emperical* observation, while software is fundamentally a *logical* construct. These differences have important consequences for how each may be re-used in future: software may be used by any researchers seeking to apply the same method, data by any researchers seeking evidence about the same factd.

Evidence: Citations?

###Software is a creative work, data are facts.

In particular, software is generally subject to copyright protection as a creative work, while data is frequently considered outside the domain of copyright as it is comprised of facts about the world (you cannot copyright the 
height of Mt. Everest.) Major scientific data repositories (e.g. Dryad, FigShare) automatically apply licenses suited to data that may not be suited to software.  

Evidence: Can I apply a Creative Commons license to software?<sup id="cc-software-footnote">[Creative Commons](#cc-software)</sup>; Non-software licenses<sup id="choosealicense-footnote">[Choose a License](#choosealicense)</sup>


###Software can be used to express or explain concepts, unlike data.

Explanation?

Possible this can be merged with one of the previous statements

Evidence: Citations?

###Software is active, data is passive.

A functional way of distinguishing between software and data is to say that software is active, while data is passive. That is, software generally performs a function upon something (e.g. software processes data), while data generally has a function performed upon it (e.g. data is processed by software).

See discussion in https://github.com/danielskatz/software-vs-data/issues/15

Again, perhaps this can be merged with a previous statement.

More Explanation?


###Software suffers from a different type of bit rot than data:  It is frequently built to use other software, leading to complex dependencies, and these dependent software packages also frequently change.

Software must be constantly maintained so that it continues to function as both the hardware and software environments (including software dependencies) that it is used on changes, as developers find and fix bugs, and as user requirements demand new features and capabilities.  This is sometimes called "software rot"<sup id="Software-rot-footnote">[Wikipedia](#Software-rot)</sup> and other times called "bit rot." On the other hand, bit rot for data is generally thought of as the underlying hardware that holds the bits changing, or software that can interpret the data also needing to be updated.  These types of bit rot also affect software&mdash;the software is actually stored as a set of bits, and these bits must be interpretted, often as ASCII or UNICODE characters&mdash;but software bit rot is generally thought of as a concern of a higher level on top of this.


More explanation?

Evidence: Citations?


###Software is generally smaller than data, so a number of the storage and preservation constraints on data don’t apply to software.

Explanation?

Evidence: Citations?


###The lifetime of software is generally not as long as that of data.

The lifetime of software can reach 20 years or more, especially for well-maintained projects. The life of software can end if the task it was supposed to do is not needed anymore, or if another software does it in a better way. Data, on the other hand, often represents the results of an experiment. It might become less interesting with time, but it cannot be replaced as it is connected to one particular experiment at that particular time. In this sense, software is replaceable (by other software), while data is usually not.

A 1995 NRC Report "Preserving Scientific Data on Our Physical Universe"<sup id="NRC-preserving-footnote">[NRC 1995](#NRC-preserving)</sup>
provides the following recommendations regarding retention criteria and the appraisal process (p. 40):
"As a general rule, all observational data that are nonredundant,
useful, and documented well enough for most primary uses should be
permanently maintained. Laboratory data sets are candidates for
long-term preservation if there is no realistic chance of repeating
the experiment, or if the cost and intellectual effort required to
collect and validate the data were so great that the long-term
retention is clearly justified. For both observational and
experimental data, the following retention criteria should be used
to determine whether a data set should be saved: uniqueness, adequacy
of documentation (metadata), availability of hardware to read the data
records, cost of replacement, and evaluation by peer review. Complete
metadata should define the content, format or representation,
structure, and context of a data set."

More Explanation?

More Evidence: Citations?


###Additional Differences?

##References

[<b id="choosealicense">Choose a License</b>] Choose an open source license, "Non-software licenses," http://choosealicense.com/non-software/ Accessed: 2016-08-16. [↩](#choosealicense-footnote)

[<b id="chun2004">Chun 2004</b>] W. H. K. Chun, "On software, or the persistence of visual knowledge," Grey Room, vol. 18, pp. 26–51, 2004. doi:10.1162/1526381043320741 [↩](#chun2004-footnote)

[<b id="cc-software">Creative Commons</b>] Creative Commons, FAQ, "Can I apply a Creative Commons license to software?", https://wiki.creativecommons.org/index.php/Frequently_Asked_Questions#Can_I_apply_a_Creative_Commons_license_to_software.3F Accessed: 2016-08-16. [↩](#cc-software-footnote)

[<b id="F11SCWG">FORCE11 Software Citation Working Group</b>] FORCE11 Software Citation Working Group, GitHub repository, https://github.com/force11/force11-scwg. Accessed: 2016-07-10. [↩](#F11SCWG-footnote)

[<b id="matthews2010">Matthews et al. 2010</b>] B. Matthews, A. Shaon, J. Bicarregui, and C. Jones, “A framework for software preservation,” International Journal of Digital Curation, vol. 5, no. 1, pp. 91–105, 2010. doi:10.2218/ijdc.v5i1.145 [↩](#matthews2010-footnote)

[<b id="NRC-preserving">NRC 1995</b>] National Research Council, Preserving Scientific Data on Our Physical Universe: A New Strategy for Archiving the Nation's Scientific Information Resources, 1995.  http://www.nap.edu/catalog/4871.html  [↩](#NRC-preserving-footnote)

[<b id="F11SCWG-web">Smith et al. 2016a</b>] A. M. Smith, D. S. Katz, K. E. Niemeyer, and FORCE11 Software
Citation Working Group “Software Citation Principles,” FORCE2016 Website, https://www.force11.org/software-citation-principles, 2016. Accessed: 2016-07-10. [↩](#F11SCWG-web-footnote)

[<b id="F11SCWG-PeerJCS">Smith et al. 2016b</b>] A. M. Smith, D. S. Katz, K. E. Niemeyer, and FORCE11 Software Citation Working Group, “Software Citation Principles,” PeerJ CS 2:e86, 2016. https://doi.org/10.7717/peerj-cs.86 [↩](#F11SCWG-PeerJCS-footnote)

[<b id="Software-rot">Wikipedia</b>] Wikipedia, “Software Rot”. https://en.wikipedia.org/wiki/Software_rot Accessed: 2016-08-18. [↩](#Software-rot-footnote)

