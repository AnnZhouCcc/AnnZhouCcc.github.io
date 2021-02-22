---
permalink: /
title: "Looking for research opportunities in Summer 2021 & Planning to attend graduate school in Fall 2022"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---




I am a senior undergraduate student, with a major in Computer Science and a minor in Linguistics, from Washington University in St. Louis. Prior to that, I graduated from River Valley High School, Singapore.

My research interests lie at the intersection of theory and practice. I am excited to work on **algorithm design and analysis when applied to distributed and parallel systems**, or **solve system-related problems from a theoretical standpoint**, be it time complexity or programming model.




Research Experiences
======

Improving access history for determinacy race detection
------
Supervisors: [Dr. Kunal Agrawal](https://www.cse.wustl.edu/~kunal/) and [Dr. I-Ting Angelina Lee](https://www.cse.wustl.edu/~angelee/home_page/), [Parallel Computing Technology Group, WUSTL](http://parallel.cse.wustl.edu/index.html)

Race detection typically consists of two components, reachability analysis and access history. Most of the research
has focused on the former while little attention has been paid to access history, which stores all memory locations previous instructions have
accessed. In theory, the access history component adds no asymptotic overhead, but in practice, it is often the most expensive component. 
We leverage the temporal and spatial locality of parallel programs and combine contiguous memory accesses into intervals. 
We propose coalescing strategies, both in compiler-time and runtime, and a tree-based access history data structure to fully reap the benefit
of maintaining access history at the granularity of intervals.


Parallelizing determinacy race detectors with efficient access history
------
Supervisors: [Dr. Kunal Agrawal](https://www.cse.wustl.edu/~kunal/) and [Dr. I-Ting Angelina Lee](https://www.cse.wustl.edu/~angelee/home_page/), [Parallel Computing Technology Group, WUSTL](http://parallel.cse.wustl.edu/index.html)

Parallelizing race detection systems is not a trivial task. There are three challenges that need to be handled efficiently in order for the tool to perform. First, we need to version the memory accesses such that the tool is not misled by false positives. Second, we need to design a runtime support such that queries and insertions are sent over to access history in batches that do not conflict with each other. Third, in the access history, we need to design data structures and algorithms such that batches of queries and insertions can be processed in parallel.


Tunable deep learning for computational imaging
------
Supervisor: [Dr. Ulugbek Kamilov](https://cigroup.wustl.edu/ulugbek-s-kamilov/), [Computational Imaging Group, WUSTL](https://cigroup.wustl.edu/)

Deep learning has led to a paradigm shift in computational imaging. We want to explore the topic of tunable deep learning, where the goal is to design techniques that enable us to adjust convolutional neural networks without retraining them. We aim to achieve this goal with a specially design scaling paramter that explicitly controls the tradeoff between data fidelity and prior and we want to extend the framework to constrained convolutional neural networks, which are more widely used in practice.


Making online decisions for protecting geolocation privacy of photo collections
------
Supervisor: [Dr. Ayan Chakrabarti](https://projects.ayanc.org/), [Vision & Learning Group, WUSTL](https://vlg.seas.wustl.edu/)

Due to the potential risks of exposing a person’s current location or travel history,
especially when adversarial neural netowrks are powerful enough to predict locations based on pure image pixels of photo collections, researchers have attempted
to protect people’s geolocation privacy in various ways. A popular method, aimed at specifically counteracting
algorithms like IM2GPS and PlaNet that infer only based on image content, tries to mislead location inference by pruning selected photos from photo collections. We frame the problem as a combinatorial optimization problem and aim to “select a minimal set of
images to delete from a given collection, such that the true location is not included in the most
likely locations predicted from the remaining images”. We want to make pruning decisions online when we have not seen the entire photo collection yet.


Publications
======

Efficient Access History for Race Detection
------
Yifan Xu, **Anchengcheng Zhou**, Grace Q. Yin, Kunal Agrawal, I-Ting Angelina Lee, Tao B. Schardl 

Submitted to 33rd ACM Symposium on Parallelism in Algorithms and Architectures (SPAA 2021)

While there has been extensive research on race-detection
algorithms for task parallel programs, most of this research
has focused on optimizing a particular component — namely
reachability analysis, which checks whether two instructions
are logically in parallel. Little attention has been paid to
the other important component, namely the access history,
which stores all memory locations previous instructions have
accessed. In theory, the access history component adds no asymptotic
overhead; however, in practice, it is often the most
expensive component of race detection since it is queried and
(possibly) updated at each memory access. We optimize this
component based on the observation that, typically, strands
within parallel programs access contiguous blocks of memory.
Therefore, instead of maintaining the access history at
the granularity of individual memory locations, we maintain
it at the granularity of these (varying size) intervals. To enable
this access history, we propose (1) compiler and runtime
mechanisms that allow us to efficiently collect these intervals
and (2) a tree-based access history data structure that
allows us to update and query it at this interval granularity.
The resulting tool can race detect fork-join code with amortized
constant overhead, assuming the number of intervals
is small compared to the total work of the computation.



Awards, Honors & Memberships
======
* 8th Heidelberg Laureate Forum Selected Young Researcher (2020)
  * Awarded to 200 researchers globally at all levels from undergraduates to postdocs
* Ernest D. Weiss Junior Award for Academic Excellence (2020)
  * Awarded to the top rank junior of the engineering school (385 students in total)
* Washington University Scholars in Engineering (2018 – 2021)
* Dean’s List, Washington University in St. Louis – All eligible semesters (2018 – 2021)
* Grace Hopper Celebration Scholarship (2018 – 2020)
*	Antoinette Frances Dames Award for Outstanding Academic Performance (2019)
*	Tau Beta Pi Engineering honor society member (2019)
*	Ministry of Education Singapore Full Scholarship Award (2012 – 2016)



Teaching Experiences
======

* Teaching Assistant - Advanced Algorithms and Data Structures, WUSTL (Spring 2020, Spring 2021)
* Teaching Assistant - Algorithms and Data Structures, WUSTL (Fall 2018, Fall 2019)
* Teaching Assistnat - Introduction to Computer Science, WUSTL (Spring 2018)


Work Experiences
======

* Research Assistant - [Yao Chen Lab, WUSTL](https://sites.wustl.edu/yaochenlab/) (January 2021 - Present)
* Software Engineer Co-op Intern - [Audible Inc., Cambridge](https://www.audible.com/) (September 2020 - January 2021)
* Software Engineer Intern - [Palantir Technologies Inc., New York](https://www.palantir.com/) (May 2019 - August 2019)
* Software Engineer Intern - [Mentor Spaces, St. Louis](https://www.mentorspaces.com/) (June 2018 - August 2018)

