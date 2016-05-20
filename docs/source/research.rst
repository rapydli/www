Research
========

RaPyDLI will design a prototype software framework that provides highly
optimized, distributed, easy-to-use implementations of the basic
primitives that underlie commonly used Deep Learning (DL) modules. This
can scale the platform spectrum from desktops to today’s largest
supercomputers and beyond, to machines with different accelerators such
as GPU and MIC chips. Because DL modules can be mixed, matched, and
combined freely, a surprisingly small set of optimized operations can be
used to represent a rich array of functionality useful for attacking a
range of applications. We have already identified a modest number of key
routines (fewer than 100) grouped into 10 broad categories that are
sufficient to implement many state-of-the-art DL algorithms and have
scaled them up dramatically, with the only change in user software being
a requirement to call our new libraries, as shown in the accompanying
figure. Our co-design process will create a middleware infrastructure
that helps connect, in a highly scalable way, a wide range of
exploratory DL algorithms (many of which are already implemented for
single nodes) to the high-performance operations needed for DL research
on distributed HPC systems. Our approach mimics the way BLAS and BLACS
provided primitives to implement and extend high-level linear algebra
codes.

Further information about research done at RaPyDLI can also be found in
a `presentation <RaPyDLI_June2_2015.pptx>`__ given by Prof. Geoffrey Fox
at the NSF XPS Workshop on June 2, 2015.

|RaPyDLI framework|

**Figure:** RaPyDLI HPC Software framework

Deep Learning has had major impact in areas like speech recognition,
drug discovery, computer vision, and natural language. This success
relies on training large-size neural nets – currently up to 1010
connections trained on 10 million images – using either large-scale
commodity clusters or smaller HPC systems where accelerators perform
with high efficiency. The current terabyte training sets can be expected
to increase usefully. One near-term example application is self-driving
cars. Future goals include a dataset of 2 Petabytes coming from an
estimate of the training data absorbed by a 20 year old human. Progress
in these goals requires a powerful rapid prototyping environment
offering both customizability and high performance execution on new
multicore and accelerator enhanced computing platforms. Specifically,
training deep neural networks for any task requires an extensive design
process in which a researcher must choose various design parameters for
the system and run dozens or even hundreds of experiments to tune its
behavior. Hence, in view of the widely acknowledged complexities of
current and emerging massively multicore and hybrid computing platforms,
the DL community has arrived at a performance/programmability impasse:
new algorithms require substantial code development, so DL users, who
are not typically HPC experts, must be supported by a high-level
programming environment. And yet the software they write must execute
efficiently at scale on next-generation platforms.

Our team will research and develop a high-performance deep learning
software environment and tool chain as well as provide accompanying
benchmarks and tutorials, allowing broad uptake. This activity will be
performed in close collaboration with HPC and Deep Learning communities
as a distributed co-design activity with a team from Indiana University,
Stanford University, and the University of Tennessee, combining unique
expertise in programming environments, DL research, and HPC
computational libraries in a unified endeavor.

The DL area, like many computationally intensive research fields, often
employs small (desktop) systems to prototype new algorithms quickly, yet
is equally dependent on climbing the platform pyramid to larger HPC
systems in order to increase the size of the problems they can attack.
HPC systems exhibit clock frequencies now capped below 4 GHz and
trending downward; latencies in key areas (e.g., memory access, bus,
system interconnect) that are expected to remain relatively stagnant; a
proliferation of hybrid designs; and needed performance increases coming
from increased parallelism. General solutions to this complexity have
proven hard and our co-design approach is to define application areas
that are broad enough to have a significant community value but limited
in requirements so that it is feasible to build custom support that
hides the HPC and parallelism details from the users.

.. |RaPyDLI framework| image:: http://salsaproj.indiana.edu/RaPyDLI/Framework.png
