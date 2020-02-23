# The Six Divisions
The activities of Greater Data Science are classified into 6 divisions:
1. Data Exploration and Preparation
2. Data Representation and Transformation
3. Computing with Data
4. Data Modeling
5. Data Visualization and Presentation
6. Science about Data Science
Let’s go into some detail about each division.

# GDS1: Data Exploration and Preparation. 
Some say that 80% of the effort devoted to data
science is expended by diving into or becoming one with one’s messy data to learn the basics
of what’s in them, so that data can be made ready for further exploitation. We identify two
subactivities:
> • Exploration. Since John Tukey’s coining of the term ‘Exploratory Data Analysis’ (EDA),
we all agree that every data scientist devotes serious time and effort to exploring data to
sanity-check its most basic properties, and to expose unexpected features. Such detective
work adds crucial insights to every data-driven endeavor.
> • Preparation. Many datasets contain anomalies and artifacts.30 Any data-driven project
requires mindfully identifying and addressing such issues. Responses range from reformatting and recoding the values themselves, to more ambitious pre-processing, such as
grouping, smoothing, and subsetting. Often today, one speaks colorfully of data cleaning.

# GDS2: Data Representation and Transformation.
A data scientist works with many different
data sources during a career. These assume a very wide range of formats, often idiosyncratic
ones, and the data scientist has to easily adapt to them all. Current hardware and software
constraints are part of the variety because access and processing may require careful deployment
of distributed resources.
Data scientists very often find that a central step in their work is to implement an appropriate
transformation restructuring the originally given data into a new and more revealing form.
Data Scientists develop skills in two specific areas:
> • Modern Databases. The scope of today’s data representation includes everything from
homely text files and spreadsheets to SQL and noSQL databases, distributed databases,
and live data streams. Data scientists need to know the structures, transformations, and
algorithms involved in using all these different representations.
>  • Mathematical Representations. These are interesting and useful mathematical structures
for representing data of special types, including acoustic, image, sensor, and network data.
For example, to get features with acoustic data, one often transforms to the cepstrum or
the Fourier transform; for image and sensor data the wavelet transform or some other
multi scale transform (e.g. pyramids in deep learning). Data scientists develop facility
with such tools and mature judgement about deploying them.

# GDS3: Computing with Data.
Every data scientist should know and use several languages for
data analysis and data processing. These can include popular languages like R and Python,
but also specific languages for transforming and manipulating text, and for managing complex
computational pipelines. It is not surprising to be involved in ambitious projects using a half
dozen languages in concert.

Beyond basic knowledge of languages, data scientists need to keep current on new idioms for
efficiently using those languages and need to understand the deeper issues associated with
computational efficiency.
Cluster and cloud computing and the ability to run massive numbers of jobs on such clusters
has become an overwhelmingly powerful ingredient of the modern computational landscape.
To exploit this opportunity, data scientists develop workflows which organize work to be split
up across many jobs to be run sequentially or else across many machines.
Data scientists also develop workflows that document the steps of an individual data analysis
or research project.
Finally, data scientists develop packages that abstract commonly-used pieces of workflow and
make them available for use in future projects.

# GDS4: Data Visualization and Presentation. 
Data visualization at one extreme overlaps with
the very simple plots of EDA - histograms, scatterplots, time series plots - but in modern
practice it can be taken to much more elaborate extremes. Data scientists often spend a great
deal of time decorating simple plots with additional color or symbols to bring in an important
new factor, and they often crystallize their understanding of a dataset by developing a new
plot which codifies it. Data scientists also create dashboards for monitoring data processing
pipelines that access streaming or widely distributed data. Finally they develop visualizations
to present conclusions from a modeling exercise or CTF challenge.
GDS5: Data Modeling. Each data scientist in practice uses tools and viewpoints from both of
Leo Breiman’s modeling cultures:
• Generative modeling, in which one proposes a stochastic model that could have generated
the data, and derives methods to infer properties of the underlying generative mechanism.
This roughly speaking coincides with traditional Academic statistics and its offshoots. 31
• Predictive modeling, in which one constructs methods which predict well over some some
given data universe – i.e. some very specific concrete dataset. This roughly coincides with
modern Machine Learning, and its industrial offshoots. 

# GDS6: Science about Data Science. 
Tukey proposed that a ‘science of data analysis’ exists
and should be recognized as among the most complicated of all sciences. He advocated the
study of what data analysts ‘in the wild’ are actually doing, and reminded us that the true
effectiveness of a tool is related to the probability of deployment times the probability of
effective results once deployed.

32Leo Breiman (2001) is correct in pointing out that academic statistics departments (at that time, and even since)
have under-weighted the importance of the predictive culture in courses and hiring. It clearly needs additional emphasis.
33Data Analysis per se is probably too narrow a term, because it misses all the automated data processing that goes
on under the label of Data Science about which we can also make scientific studies of behavior ‘in the wild’.
Data scientists are doing science about data science when they identify commonly-occuring
analysis/processing workflows, for example using data about their frequency of occurrence in
some scholarly or business domain; when they measure the effectiveness of standard workflows
in terms of the human time, the computing resource, the analysis validity, or other performance
metric, and when they uncover emergent phenomena in data analysis, for example new patterns
arising in data analysis workflows, or disturbing artifacts in published analysis results.
The scope here also includes foundational work to make future such science possible – such as
encoding documentation of individual analyes and conclusions in a standard digital format for
future harvesting and meta analysis.
As data analysis and predictive modelling becomes an ever more widely distributed global
enterprise, ‘Science about Data Science’ will grow dramatically in significance.



Source:- 
https://courses.csail.mit.edu/18.337/2015/docs/50YearsDataScience.pdf