# Strategic Subject (SSL) Data Analysis

The Chicago Police Department recently released de-identified information from arrest data used
in its Strategic Subject List (SSL) model which assigns scores from 1-500 to individuals
based on their likelihood to become "parties to violence" in the future,
whether as potential victims or perpetrators. The information is on the [Chicago
Open Data Portal](https://data.cityofchicago.org/Public-Safety/Strategic-Subject-List/4aki-r3np).
The model is said to have gone through at least 5 iterations, with this being one
of the later versions.

The data description indicates that this is the output of the algorithm being
applied to all CPD arrest data in that time period (August 1, 2012 through July 31,
2016), and not necessarily the list itself. However, the distinction between "high
priority" individuals--often cited as being between 400 and 1,400 people--is not
clear.

Additionally, according to [CPD Special Order 09-11](http://directives.chicagopolice.org/directives/data/a7a57b85-155e9f4b-50c15-5e9f-7742e3ac8b0ab2d3.html?hl=true)
the default view for the Strategic Subjects List dashboard used by CPD personnel
lists "all subjects with an SSL score of one or higher are shown and placed in
descending order of score." If all scores are taken into consideration and viewed
by CPD, then there is value in looking at patterns across all individuals on the
list rather than just individuals with the highest scores, especially when the
cutoffs/totals aren't made clear.

## Total Numbers on the List

In total, at the time this model was run for (July 31, 2016, for the period from
August 1, 2012 through July 31, 2016), there were 398,684 individuals in the records
of arrest data used to produce this list. There is no clear indication of how many individuals
CPD considers to be "on the list", but over time numbers ranging from 426 ([in the initial iteration evaluated by RAND](https://link.springer.com/article/10.1007/s11292-016-9272-0)) to
to 1,400 ([in a May 2016 New York Times Story](https://link.springer.com/article/10.1007/s11292-016-9272-0)),
with one source referring to 30,000 individuals being included ([September 2015 Chicago Sun-Times story](http://chicago.suntimes.com/news/four-of-eight-men-slain-wednesday-on-police-at-risk-list/)).

## List Cutoffs

In stories describing the SSL, multiple cutoffs have been mentioned for individuals to be considered "on the list",
or to be on the list and given additional scrutiny. The RAND evaluation (linked above) gave the impression that
the scores are created and then a semi-manual selection process happens, which resulted in 426 individuals.

However, other stories have often referred to scores of 400 and above as being subject to higher levels of
scrutiny, but often aren't explicit about whether they are an actual cutoff for being on the SSL or not. A
[May 2016 Chicago Tribune editorial](http://www.chicagotribune.com/news/opinion/editorials/ct-gangs-police-loury-algorithm-edit-md-20160510-story.html)
puts the cutoff for inclusion at the "upper 200s or higher", which at the time Chicago police Superintendent Eddie Johnson
described as only being made up of 1,300 people. This cutoff of the upper 200s is also mentioned in a
[December 2016 LA Times story](http://www.latimes.com/nation/la-na-chicago-shootings-20161226-story.html). However,
looking at the released data, 287,404 (72.09%) of the 398,684 individuals had score of 250 or above.

## Counts by Score

| Score  | Count Individuals |
|--------|-------------------|
| > 0    | 398,684           |
| >= 100 | 397,917           |
| >= 150 | 391,046           |
| >= 200 | 354,994           |
| >= 250 | 287,404           |
| >= 300 | 173,001           |
| >= 350 | 29,212            |
| >= 400 | 3,721             |
| >= 450 | 709               |
