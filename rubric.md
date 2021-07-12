# Rubric

## Introduction (4 levels) 

Is the introduction clear? Is the research question specific and well defined? Does the introduction motivate a specific concept to be measured and explain how it will be operationalized. Does it do a good job of preparing the reader to understand the model specifications?

4. An introduction that is scored in the top level has very successfully made the case for the reader. It will have placed the specific question in context, connected the problem with the statistics and data that will be used, and have generally created a compelling case for continuing to read the report. 
3. An introduction that scores in the third level has done a significant amount of successful work. The reader can place the topic area and the research question; understand and appreciate why this is a question that demands a data based answer. Keeping this introduction from a full, four-point score might be: small issues with writing, some lack of continuity in the argument, or some other such small issue that keeps this from being a wholly convincing introduction. 
2. An introduction that scores in the second level has made some attempt to describe the problem and its importance, but it is missing significant parts of this argument. The language might be poorly chosen, the argument loosely formed, or the context left unexplained; there is considerable room for improvement. 
1. An introduction that is scoring at the first level either doesn’t exist, or has given a very cursory treatment for the setting of the question and why an answer based on statistics is necessary. 

## Conceptualization and Operationalization (4 levels) 

4. A report that is scored in the top level on conceptualization and operationalization will have done a wholly adequate job connecting the context and research question from the introduction to a set of clearly, and precisely defined concepts. From these concepts, the report will have identified data that clearly does a good job of measuring these concepts; the argument will be clear, concise, and complete. 
3. A report that is scored in the third level on conceptualization and operationalization will have done good work to define a concept and a measure that corresponds to that concept. Keeping this report from full marks might be some imprecision in the definition of the concept; or some mis-match between the concept and the eventual data that is used. 
2. A report that scored in the second level on conceptualization and operationalization will have attempted to connect the introduction into defined concepts; and will have also attempted to find measures in the data that map onto those concepts, but will have run into significant challenges. Either the concepts are not developed enough for any measure to be meaningful; or the choice of measure does not match with the concept. 
1. A report that is scored in the first level conceptualization and operationalization will have failed to connect the concepts that have been identified in the introduction to the data in any meaningful way. As a consequence, it is not possible for the reader to know that any analysis that comes from this report has any bearing on the question at hand. 

## Data Wrangling (3 levels) 

3. A report that is scored in the top level on data wrangling will have succeeded -- relative to expectations at this point in the course -- to produce a modern, legible data pipeline from data to analysis. The wrangling *could* be done in the same notebook as the analysis and report. However, because there are many pieces of data that are being marshaled, perhaps the wrangling has be refactored into its own, file. The analysis should have a single source of truth data, and it should be clear what and how, any additional features are derived from this data. At this point in the course, a three point data wrangling can still have issues that keep it from being professional-grade, but these are the types of issues that might be expected for early-programmers: variable names might be communicative, but clumsy; pipelines might work, but be inefficient, etc.
2. A report that scores in the second level data wrangling will have tried, but not fully achieved the aims for a modern, legible data pipeline from data to analysis. None of the problems cast doubt on the results, but might mean that it would be difficult to contribute to this project in the future, difficult to read this analysis for the present reader, or some other such flaw. This level of data wrangling might have several version of the data that do not maintain referrential integrity (in the case of this data, an example of a problem is writing code based on column position rather than column names), or it might have several versions of derived data from the source data (i.e. `anes_data_republicans`, `anes_data_democrats`) that could generate issues with a future pipeline.
1. A report that scores in the first level on data wrangling has significant issues in how the data has been prepared for analysis. The data may choose to use inappropriate, or non-descriptive variables; may have made several mis-steps in the data preparation; or otherwise made choices in the preparation of the data that cast doubt on any results that might come from the analysis. 

## Data Understanding (3 levels) 

In order for a reader to understand or ascribe meaning to your results, they need to understand enough about the data that they can place what you are presenting to them in context.  This can be done with by referencing tables, figures, and summary statistics in the narrative. You might ask yourselves, "Overall, does the report demonstrate a thorough understanding of the data? Does the report convey this understand to its reader -- can the reader, through reading this report, come to the same understanding that the team has come to?" 


3. A report that is scored in the top level on "Data Understanding" will describe features of the data in the narrative to give the reader sufficient understanding of the distribution.  Anomalies will be identified, including censored scales, artifacts of binning, and prominent clusters.  Every single plot or R output included in the report will be discussed in the narrative.
2. A report that is scored in the second level on "Data Understanding" will leave the reader with a good understanding of the data distribution.  Keeping the report from a perfect score might be a failure to comment on some feature of the data that would help the reader to contextualize the results.
1. A report that is scored in the first level will leave the reader with an insufficient understanding of the distribution to fully contextualize the results.  A report that includes an output dump (a plot or R output that is not discussed in the text) will also score in this level.


## Visual Design (5 levels)

5. A report that is scored in the top level will include plots that effectively transmit information, engage the reader's interest, maximize usability, and follow best practices of data visualization.  Titles and labels will be informative and written in plain english, avoiding variable names or other artifacts of R code.  Plots will have a good ratio of information to space or information to ink; a large or complicated plot will not be used when simple plot or table would show the same information more directly.  Axis limits will be chosen to minimize visual distortion and avoid misleading the viewer.  Plots will be free of visual artifacts created by binning.  Colors and line types will be chosen to reinforce the meanings of variable levels and with thought given to accessibility for the visually-impaired.  
4. A report that is scored in the fourth level will include plots that effectively transmit information, do not present major obstacles to usability, and follow best practices for data visualization.  Keeping the report from top score might be some distracting visual artifact, axis labels that do not line up properly with histogram bars, poorly chosen bin widths, a legend that conceals important information, or some other aspect in which the plot might be improved.
3. A report that is scored in the third level will include plots that contain important information and can be effectively used by most readers.  Keeping the report from a top score might be an instance in which a complicated or large plot is used when a compact plot or table would display the same information more effectively, redundant plots that substantially overlap in the information they show, or a moderate problem with axes, binning, labels, or colors.
2. A report that scores in the second level will have chosen a plot that communicates a point to the reader, but that could be more convincing in its effect.  The plot may not have multiple issues that interfere with usability; it may be poorly titled and labeled; or the choice of presentation may not have fully communicated the pattern that the team wants to make. 
1. A report that is scored in the first level will have serious issues with its visual design.

## Model Building and Reporting

Overall, is each step in the model building process supported by EDA? Is the outcome variable (or variables) appropriate? Did the team clearly state why they chose these explanatory variables, does this explanation make sense in term of their research question? Did the team consider available variable transformations and select them with an eye towards model plausibility and interpretability? Are transformations used to expose linear relationships in scatterplots? Is there enough explanation in the text to understand the meaning of each visualization?

- **A Regression Table.** Are the model specifications properly chosen to outline the boundary of reasonable choices? Is it easy to find key coefficients in the regression table? Does the text include a discussion of practical significance for key effects? 

### Arguing for, and Assessing Regression Model (6 levels) 

6. A report that is scored in the top level will have made a clear argument for the statistical models that is appropriate given the data, and the process that generates that data. This argument will be clear, precise, and correct. If there are limitations of the models, these will be identified, and reasoned about, but the report will be correct that this is the most appropriate model that can be conducted with this data. 
5. A report that is scored in the fifth level will have made a clear argument for the statistical model that is appropriate given the data, and the process that generates that data. This argument will be clear, precise, and correct. If there are limitations of the model, these will be identified, and reasoned about, but the report will be correct that this is the most appropriate model that can be conducted with this data. Keeping this argument from full points might be very small imprecision in language or statistics; but the model is correct despite these small issues. 
4. A report that scores is scored in the fourth level will have made an argument for a model, and this argument might be somewhat reasonable but there is significant room for improvement or errors in presentation. For example, metric data might be interpreted as ordinal; or, ordinal data as metric (which is a more serious problem). Or a model might be close to correct, but could instead have utilized a universally better powered model. 
3. A report that scores either in the second or third level will have serious errors in its reasoning about a model. It might use data that is an inappropriate level, or a model that doesn’t inform the question at hand. There is considerable room for improvement in an answer of this form. 
1. A report that scores in the first level will have made very serious errors in its reasoning about a model. This might mean using a model that is unrelated to the question; or a model that is inappropriate to the data or some other very serious error that precludes any result from this model being able to inform the research question. 

### Model Results and Interpretation (6 levels) 

6. A report that scores in the top level will have interpreted the results of the model appropriately, drawn a conclusion about statistical significance; placed these results in context with some statement about practical significance that is compelling to the reader; and will have done so in a way that is clear, concise, and correct. 
5. A report that scores in the fifth level  will have interpreted the results of the model appropriately, drawn a conclusion about statistical significance; placed these results in context with some statement about practical significance that is compelling to the reader. Keeping this from full points might be some lack of clarity or concision; or some very slight error in the interpretation of the model. 
4. A report that scores in the fourth level will have done much of the modeling correctly, but might be missing either a statement of practical significance or interpretation of the results of the model. While the statistics might not be incorrect, they are not making a wholly compelling argument. 
3. A report that scores in the third level will have some considerable errors in the modeling. Either the results will be inappropriately interpreted -- statistically significant results might be interpreted as non-significant for example -- or will have failed to successfully connect the results of the model with an interpretation of what these results mean. 
2. A report that scores in the second level will have very serious issues with how the model results are interpreted. They may be wrong; non-existent; mis-characterized; or some other such very serious issue. If there is any interpretation, it might be incorrect or unhelpful. 
1. A report that scores in the first level will have very serious issues with how the model results are interpreted. They may be wrong; non-existent; mis-characterized; or some other such very serious issue. If there is any interpretation, it might be incorrect or unhelpful. 

## Assumptions of the Model (4 levels)

Has the team presented a sober assessment of the CLM assumption that might be problematic for their model? Have they presented their analysis about the consequences of these problems (including random sampling) for the models they estimate? Did they use visual tools or statistical tests, as appropriate? Did they respond appropriately to any violations?

4. A report that scores in the top-level has provided an unassailable assessment of the assumptions of the model. This does not mean that the model necessarily satisfies all assumptions, but that where it does not the reader is promptly notified of the issue, its consequences for the analysis, and potential strategies to remedy these consequences. 
3. A report that scores in the third-level has provided a fair assessment of the assumptions of the model. The team may have failed to satisfy a skeptical reader who: a skeptic might raise concerns that have not been addressed, or might reasonably disagree with the team's assessment of an assumption violation. 
2. A report that scores in the second-level has provided some work to assess the modeling assumptions, but a skeptical reading might quickly point out flaws in the statistical reasoning, or raise issues that the team has not addressed.
1. A report that scores in the bottom-level has provided a cursory treatment of modeling assumptions. Some assessments might be incorrect or non-existent. Reasonable questions from a skeptical reader might be left unaddressed. 

## Omitted Variables Bias (3 levels) 

Did the report miss any important sources of omitted variable bias? Are the estimated directions of bias correct? Was their explanation clear? Is the discussion connected to whether the key effects are real or whether they may be solely an artifact of omitted variable bias?

3. A report that scores in the top-level has thought carefully about omitted variables in a causal model; their thinking is done in a way that would satisfy a skeptical reader. It need not propose to measure all omitted featured, but after the discussion of omitted variables even a skeptical reader should acknowledge that the proposed cause-and-effect relationship is plausible. 
2. A report that scores in the second-level has engaged with the concept of omitted variables, but has not fully addressed the topic. A skeptical reader might propose reasonable features that the team has not considered that would confound the proposed causal relationship. 
1. A report that scores in the first-level has engaged with the concept of omitted varaibles in little more than a cursory manor, or has not engaged with the concept at all. A skeptical reader might pose a fundamental problem for the cause-and-effect relationship that the report has failed to address. 

## Stating a Hypothesis (4 levels) 

4. A report that is scored in the top level on framing a hypothesis will have precisely stated the correct null hypothesis for the conducted test in the regression model.
3. A report that is scored in the third level will have expressed a null consistent with the conducted test. Keeping this hypothesis from scoring full points might be a small lack of the precision; misapplied technical language, or some other flaw that doesn't detract from the broader conceptualization of the test.
2. A report that is scored in the second level will have stated a hypothesis, but it might be loosely related to the question at hand; unclear, or insufficiently precise to serve as a testing basis, or some other serious issue. 
1. A report that is scored in the first level will have significant problems with how the null hypothesis is stated. Either it will be incorrectly stated as an alternative hypothesis; or, it will be unrelated to the question at hand; or some other major flaw. 


## Conclusion and Impacts (3 points) 

3. A top-level conclusion will summarize the team's work, provide the reader with a reminder of the initial question, and will provide recommendations *based on the analysis* that are reasonable generalizations of the narrow statistical modeling work that the team has undertaken. Recommendations made in this section will identify the evidence from the reports' analysis, and will also identify limitations or context that shapes in interpretation of these recommendations. 
2. A second-level conclusion might too simply restate the introduction of the report. It might not be as closely-related to the analysis as it should be. A report with a conclusion that scores in the second-level is better than a report that does not have a conclusion, but it could be strengthed to contribute more. 
1. A first-level conclusion does not make much, if any, contribution to the report overall. This conclusion likely is a rote restatement of the introduction; or, it does not relate to the analysis conducted in the report. A report with an introduction ranked in the first level would most likely be just as strong without this conclusion. 

## Overall Effect (3 levels) 

3. A report that scores in the top level will have met expectations for professionalism in data-based writing, reasoning and argument for this point in the course. It can be presented, as is, to another student in the course, and that student could read, interpret and take away the aims, intents, and conclusions of the report. 
2. A report that scores in the second level will be largely professional; largely clearly written and structured; but will have some problem that inhibits the reader from being able to clearly reason from the report. 
1. A report that scores in the first level will have significant issues in its presentation. These could be spelling, language, argument, formatting, or other issues that cause problems for the reader in their ability to read, evaluate, and take action on what is reported. 