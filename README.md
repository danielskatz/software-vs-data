#Software vs Data


> The version of this document of 9 December 2016 has been published as:
>
> Katz DS, Niemeyer KE, Smith AM, Anderson WL, Boettiger C, Hinsen K, Hooft R, Hucka M, Lee A, Löffler F, Pollard T, Rios F. (2016) Software vs. data in the context of citation. PeerJ Preprints 4:e2630v1 https://doi.org/10.7287/peerj.preprints.2630v1


Author/Editors:
Daniel S. Katz,
Kyle E. Niemeyer,
Arfon M. Smith

Additional Authors:
William L. Anderson, Carl Boettiger, Konrad Hinsen, Rob Hooft, Mike Hucka, Allen Lee, Frank Löffler, Tom Pollard, Fernando Rios


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

Explanation if needed,

including or followed by:

Evidence: Citations

---

##List of Differences

###Software is executable, data is not.

A commonsense definition of software is that it is "a set of instructions that direct a computer to do a specific task"<sup id="chun2004-footnote">[Chun 2004](#chun2004)</sup>. On the other hand, data is simply a collection of facts or measurements (real or simulated). In other words, software is functionally active, while data is passive. Of course, software (in form) can be considered data as well, especially to functional programmers familiar with LISP and other languages with homoiconicity<sup id="homoiconicity-footnote">[Kay 1969](#homoiconicity)</sup>. However, from the point of view of conducting research with software, the main difference is that software is associated with action: knowledge creation, information transformation, visualization, etc.  An action can be thought of a functional transformation between two states of data: a "before" (e.g., input files, parameter settings, unstructured or tacit information) to an "after" state (e.g., output files, transformed data, structured knowledge). That is, software generally performs a function upon something (e.g., software processes data), while data generally has a function performed upon it (e.g., data is processed by software). If we accept the definitions of software and data given at the beginning of this section, then (at least in scientific research), the difference between data and software can be summarized by the statement of <sup id="matthews2010-footnote">[Matthews et al. 2010](#matthews2010)</sup>: "we are more interested in what software *does* rather than what software *is*."


###Data provides evidence, software provides a tool.

Software exists to perform a task, while data does not. Software is fundamentally a *logical* construct, while data is fundamentally an *empirical* observation. Software can be used to express or explain processes and concepts, oftentimes with data as input. These differences have important consequences for how each may be re-used in the future: software may be used by any researchers seeking to apply the same methods, data by any researchers seeking evidence about the same facts.


###Software is a creative work, scientific data are facts or observations.

In particular, software is generally subject to copyright protection as a creative work that can continue to evolve over time, while scientific data is frequently considered outside the domain of copyright as it is comprised of _contextual_ facts about the world (you cannot copyright the height of Mt. Everest.) Major scientific data repositories (e.g. [Dryad](http://datadryad.org/), [figshare](https://figshare.com/)) automatically apply licenses suited to data that may not be suited to software.  

Evidence: Can I apply a Creative Commons license to software?<sup id="cc-software-footnote">[Creative Commons](#cc-software)</sup>; Non-software licenses<sup id="choosealicense-footnote">[Choose a License](#choosealicense)</sup>


###Software suffers from a different type of bit rot than data:  It is frequently built to use other software, leading to complex dependencies, and these dependent software packages also frequently change.

In general, software must be constantly maintained and updated in order to continue to function as both the hardware and software environments on which it depends change. Operating systems, software and system libraries, programming language toolchains and other compile-time and run-time dependencies all evolve as their respective maintainers and developers find and fix bugs, and as user requirements demand new features and capabilities.  This is sometimes called "software rot"<sup id="Software-rot-footnote">[Wikipedia-c](#Software-rot)</sup> and other times called "bit rot." On the other hand, bit rot for data, or data degradation<sup id='data-degradation-footnote'>[Wikipedia-a](#data-degradation)</sup>, is generally thought of as changes in the underlying hardware or storage media that holds the bits, or changes in the software capable of interpreting the data. This definition of bit rot also affects software since software is actually stored as a set of bits on a filesystem, but software bit rot is generally thought of as a higher level concern than data- or file-level bit rot.


###The lifetime of software is generally not as long as that of data.

The lifetime of software can reach 20 years or more, especially for well-maintained projects. The life of software can end if the task it was supposed to do is not needed anymore, or if another software does it in a better way. Data, on the other hand, often represents the results of an experiment. It might become less interesting with time, but it cannot be replaced as it is connected to one particular experiment at that particular time. In this sense, software is replaceable (by other software), while data is usually not.

A 1995 NRC Report _Preserving Scientific Data on Our Physical Universe_<sup id="NRC-preserving-footnote">[NRC 1995](#NRC-preserving)</sup>
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

While software is often replaced by newer software, computational models and data analyses can be important digital artifacts that should be preserved<sup id='cml-2014-footnote'>[Rollins et al. 2014](#cml-2014)</sup> along with datasets in order to properly verify or reproduce<sup id='peng-2011-footnote'>[Peng 2011](#peng-2011)</sup> published findings. Long-term preservation of the software used in computational science is a wicked problem as outlined in the final report from the _Preserving.exe: Toward a National Strategy for Preservation Software_ 2013 meeting<sup id='preserve-exe-2013-footnote'>[Preserving.exe 2013](#preserve-exe-2013)</sup>. At that time, best practices to facilitate reproducibility of computational science involve archiving of the following, in durable, plaintext formats:

1. the software itself, in source code form in a trusted digital repository
2. structured or unstructured narrative documentation (e.g., the ODD protocol <sup id='grimm-2013-footnote'>[Grimm 2013](#grimm-2013)</sup>) specifically covering key components of the software 
3. descriptive provenance metadata on the software dependencies needed to compile and run the software as well as any input data dependencies

though these practices may change as virtualization and containerization become more common.

###Additional Differences?

##References

[<b id="choosealicense">Choose a License</b>] Choose an open source license, "Non-software licenses," http://choosealicense.com/non-software/ Accessed: 2016-08-16. [↩](#choosealicense-footnote)

[<b id="chun2004">Chun 2004</b>] W. H. K. Chun, "On software, or the persistence of visual knowledge," Grey Room, vol. 18, pp. 26–51, 2004. doi:10.1162/1526381043320741 [↩](#chun2004-footnote)

[<b id="cc-software">Creative Commons</b>] Creative Commons, FAQ, "Can I apply a Creative Commons license to software?", https://wiki.creativecommons.org/index.php/Frequently_Asked_Questions#Can_I_apply_a_Creative_Commons_license_to_software.3F Accessed: 2016-08-16. [↩](#cc-software-footnote)

[<b id="F11SCWG">FORCE11 Software Citation Working Group</b>] FORCE11 Software Citation Working Group, GitHub repository, https://github.com/force11/force11-scwg. Accessed: 2016-07-10. [↩](#F11SCWG-footnote)

[<b id="grimm-2013">Grimm et al. 2013</b>] Volker Grimm, Gary Polhill, Julia Touza, Documenting Social Simulation Models: The ODD Protocol as a Standard. In _Simulating Social Complexity: A Handbook_, pp. 117-133, 2013. http://dx.doi.org/10.1007/978-3-540-93813-2_7 [↩](#grimm-2013-footnote)

[<b id="matthews2010">Matthews et al. 2010</b>] B. Matthews, A. Shaon, J. Bicarregui, and C. Jones, “A framework for software preservation,” International Journal of Digital Curation, vol. 5, no. 1, pp. 91–105, 2010. doi:10.2218/ijdc.v5i1.145 [↩](#matthews2010-footnote)

[<b id="NRC-preserving">NRC 1995</b>] National Research Council, Preserving Scientific Data on Our Physical Universe: A New Strategy for Archiving the Nation's Scientific Information Resources, 1995.  http://www.nap.edu/catalog/4871.html  [↩](#NRC-preserving-footnote)

[<b id="peng-2011">Peng 2011</b>] Roger D. Peng, Reproducible Research in Computational Science, Science, vol 334, issue 6060, pp. 1226-1227, 2011. http://dx.doi.org/10.1126/science.1213847 [↩](#peng-2011-footnote)

[<b id="preserve-exe-2013">Preserving.exe 2013</b>] Library of Congress, Preserving.exe: Toward a National Strategy for Software Preservation, 2013. http://www.digitalpreservation.gov/multimedia/documents/PreservingEXE_report_final101813.pdf [↩](#cml-2014-footnote)

[<b id="cml-2014">Rollins et al. 2014</b>] Nathan D. Rollins, C. Michael Barton, Sean Bergin, Marco A. Janssen, Allen Lee, A Computational Model Library for publishing model documentation and code, Environmental Modelling and Software, vol 61, pp. 59-64, 2014. http://dx.doi.org/10.1016/j.envsoft.2014.06.022 [↩](#cml-2014-footnote)

[<b id="F11SCWG-web">Smith et al. 2016a</b>] A. M. Smith, D. S. Katz, K. E. Niemeyer, and FORCE11 Software
Citation Working Group “Software Citation Principles,” FORCE2016 Website, https://www.force11.org/software-citation-principles, 2016. Accessed: 2016-07-10. [↩](#F11SCWG-web-footnote)

[<b id="F11SCWG-PeerJCS">Smith et al. 2016b</b>] A. M. Smith, D. S. Katz, K. E. Niemeyer, and FORCE11 Software Citation Working Group, “Software Citation Principles,” PeerJ Computer Science 2:e86, 2016. https://doi.org/10.7717/peerj-cs.86 [↩](#F11SCWG-PeerJCS-footnote)

[<b id="data-degradation">Wikipedia-a</b>] Wikipedia, “Data degradation”. https://en.wikipedia.org/wiki/Data_degradation Accessed: 2016-11-23. [↩](#data-degradation-footnote)

[<b id="homoiconicity">Kay 1969</b>] Kay, A. C. The Reactive Engine. The University of Utah, 1969. [↩](#homoiconicity-footnote)

[<b id="Software-rot">Wikipedia-c</b>] Wikipedia, “Software Rot”. https://en.wikipedia.org/wiki/Software_rot Accessed: 2016-08-18. [↩](#Software-rot-footnote)

