Project: Decarbonization Policy for One Country
================
Jonathan Gilligan
2021-04-05

-   [Introduction](#introduction)
-   [Establishing a Goal](#establishing-a-goal)
-   [Realizing the Goal](#realizing-the-goal)
-   [Format](#format)
-   [Data Sources](#data-sources)

# Introduction

This assignment will be more free-form than the lab assignments we have
done earlier in the semester. For this assignment, you will build on the
work you did for the bottom-up and top-down decarbonization analysis and
investigate how decarbonization might play out in one specific country.
You can work on your own or in a team of two or three for this
assignment. You will choose one country, decide what that country’s
greenhouse gas emissions target should be for the year 2050, and then
sketch out a plan for how that country could achieve its goal.

You and your team will turn in a written report (one report from the
whole team is acceptable) before midnight on Friday April 30. The report
is not meant to be an exhaustive research report. I expect a length of
around 5 pages of doublespaced text (or equivalently, around 3 pages
singlespaced) per team member, plus appropriate figures, tables, and
references.

Unlike previous assignments, you may use RMarkdown, Word, or any other
word-processing mode that you wish when writing your report, but I would
like to you produce PDF output (e.g., if you’re writing in Word, save a
copy in PDF format).

# Establishing a Goal

Briefly, look at what your country has pledged to do for emissions
reduction for the 2015 Paris Agreements
(<http://spappssecext.worldbank.org/sites/indc/Pages/INDCHome.aspx> and
the individual Country Briefs at
<http://spappssecext.worldbank.org/sites/indc/Pages/Content_Brief.aspx>).
The individual country briefs are long and have a lot of material.
However, there is a single page with the economy-wide mitigation
targets, whcih give a *target year*, a *target type*, and a number for
the target type. The European Union submitted a collective NDC rather
than separate commitments from each member country.

For instance, the United States pledged a target year of 2025, a target
type of “*absolute emission reduction compared to base year (%) 2005*,”
and a target amount of 26–28%, which means that the US has pledged that
by 2025, it will have cut its annual greenhouse gas emissions 26–28%
below the emissions in 2005. The European Union has pledged a target
year of 2030, a target type of *absolute emissions reduction compared to
base year (%) 1990*, and a target number of 40%, so it pledges that by
2030 it will have cut its annual emissions 40% below what it was in
1990.

China chose a different type of target type. It chose a target year of
2030, a target type of “*reduction in emission intensity per GDP
compared to base year (%) 2005*,” and a target number of 60–65%. This
means that China is pledging that by 2030 it will have cut the economic
intensity of greenhouse gas emissions (the Kaya variable *ef*) 60–65%
below what it was in 2005.

A challenge for policy analysts is comparing the different kinds of
targets that different countries specified in their Nationally
Destermined Contributions.

To choose your country’s goal for 2050 consider what the country is
planning to do by 2030 or whichever target year it specifies in its
Nationally Determined Contribution and then consider how much more the
country might reasonably plan to do by 2050 to make a fair contribution
to reducing global greenhouse gas emissions while also taking into
account the need for less-developed nations to grow their economies in
order to lift people out of poverty.

For simplicity, I recommend that you focus on carbon dioxide emissions
from burning fossil fuels rather than on all different kinds of
greenhouse gases.

There is no right answer, and it would be possible to write a 50-page
paper just on this part, but that is not what I want you to do. Rather,
just present a simple overview of the issues your country faces and how
you would choose a goal.

For instance, you could look back to 1965 (when the data on energy and
emissions in the `kayadata` package begins) and add up the total
emissions from your country and compare it to the total emissions of the
world during that period and then consider how your country’s fraction
of total emissions compare to your country’s fraction of the total world
population or the total world Gross Domestic Product (GDP).

You may want to refer to the table below, which lists emissions
reductions from 2005–2050 for different parts of the world that would
meet a global 36% emissions target in 2050. This table comes from the
IPCC’s representative concentration pathway (RCP) database and is based
on the pathway called “RCP 2.6,”" which gives about a two-thirds
probability of keeping global warming below 2° C. However, this table
was produced from an economic model and does not take account of
political and ethical considerations, such as fairness, so you are not
obliged to choose the same goal that this table lists for your country
or its region.

|        Region         | Year | Reduction from 2005 |
|:---------------------:|-----:|--------------------:|
| Australia/New Zealand | 2050 |                 82% |
|        Canada         | 2050 |                 72% |
|         China         | 2050 |                 78% |
|         India         | 2050 |                 73% |
|         Japan         | 2050 |                 66% |
|      South Korea      | 2050 |                 67% |
|     United States     | 2050 |                 73% |
|        Africa         | 2050 |                 28% |
|     Latin America     | 2050 |                 40% |
|      Middle East      | 2050 |                 32% |
|    Southeast Asia     | 2050 |                -17% |
|    Western Europe     | 2050 |                 74% |
|         World         | 2050 |                 36% |

# Realizing the Goal

Once you have chosen a goal, you should apply the same kinds of methods
that we used in the bottom-up and top-down decarbonization analyses to
estimate what your conuntry’s population and per-capita GDP may be **in
2050**, and what the implications are for energy efficiency and the
mixture of fuels that should supply its energy needs. This is a place to
research the country’s natural resources, current energy supply, and
opportunities to decarbonize.

For instance, if your country is mountainous with many rivers, you may
want to expand hydroelectricity. On the other hand, if it is relatively
flat, has few rivers, or if all the major rivers already have dams and
generators, then you may want to look at other sources of energy. If
your country receives a lot of sunshine, you may want to emphasize solar
energy. Don’t forget to think about nuclear energy as well as renewables
like hydroelectricity, wind, and solar.

I am not asking you to give a thorough engineering and economic
assessment of the energy transition, but to give a brief overview of the
major opportunities and obstacles to clean energy in your country and
what you think would be the best strategy for reducing emissions.

# Format

This is a lab report, not a formal research paper, so you do not need to
structure it as a formal paper. My grading rubric for the written report
will be:

-   Thoughtful and sensible analysis of goals \[30%\]
-   Thoughtful and sensible analysis of how to realize the goal \[30%\]
-   Good use of the data for your country \[20%\]
-   Organization of the report (do the parts fit together well and tell
    a clear story) \[10%\]
-   Quality of writing \[5%\]
-   Appropriate use of citations and references \[5%\]

You may choose to turn this in as an RMarkdown document (knitted to PDF,
of course) or a Word document (saved as PDF), or any other format that
you have rendered as PDF.

The key is that you explain clearly how you do your analysis. You can
either use RMarkdown or you can turn in a document written with a
word-processor and refer the reader to R scripts or an RMarkdown
document with “supporting information” that contains the details of your
calculations and quantitative analysis.

You will turn this assignment in by accepting the assignment on GitHub
Classroom, cloning the repository to your own computer, saving your
final products in the repository and committing and pushing them to
GitHub.

# Data Sources

The `kayadata` package has data on the Kaya identity variables for 81
countries and top-down projections for 78 countries.

If you are working on a country that’s not one of these, you may want to
look at additional data, such as the International Energy Agency’s
energy and emissions analyses. These reports are extremely expensive to
buy, but the Vanderbilt Library provides free online access to the World
Energy Outlook reports from 1999–2020 through the Vanderbilt library
catalog. The 2020 report is available at this link
<https://doi-org.proxy.library.vanderbilt.edu/10.1787/20725302>. **When
you open this page, there will be a button to buy a PDF of the report
for more than $100, but you can ignore that. There are also buttons to
download the PDF of the full report, or individual chapters, for free.
Do not spend your money buying something the library will give you
legally and free.** You can also get detailed data for energy use in the
the OECD nations at
<https://doi-org.proxy.library.vanderbilt.edu/10.1787/379b6cdc-en>.

The U.S. Energy Information Administration publishes detailed country
profiles for a number of countries at
<https://www.eia.gov/outlooks/ieo/>, with data on many individual
countries at <https://www.eia.gov/beta/international/> and brief country
and regional analysis reports at
<https://www.eia.gov/beta/international/analysis.cfm>

This list of data sources is not exhaustive and you should feel free to
explore other sources of information, but don’t feel that you have to
spend hours in the library or the internet chasing down data. It is fine
for this assignment to use “good enough” data or to substitute estimates
if you can’t find exact numbers for what you’re looking for. Just be
clear about how you’re doing your analysis.
