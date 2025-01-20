# msds_460_assignment_one
Diet Problem Individual Assignment for Northwestern MSDS 460 course, assignment description below


Each assignment in this course should be assigned to its own unique repository.

The Diet Problem Revisited (version 11)

Developed by Thomas W. Miller. Revised January 9, 2025.

Introduced by Stigler (1945) and discussed by Dantzig (1990), the diet problem is a classic problem in constrained optimization often used to introduce linear programming concepts. The diet problem has been studied extensively through the years (van Dooren 2018).

For this assignment, you need to construct a personalized diet using current recommended dietary allowances from the U.S. Food and Drug Administration, updated to account for recent research on sodium intake and health (Mente, O'Donnell, and Yusuf 2021). Interested in learning more about nutrition and healthy living? Check out Nutrients, an open-access journal, at its home page https://www.mdpi.com/journal/nutrientsLinks to an external site. .

The constraints for this linear programming problem, should consider seven components of nutrition and their daily values, as shown in the following table:

Component

Max/Min

Daily Amount and measure

Sodium

Maximum

5,000 milligrams (mg)

Energy

Minimum

2,000 Calories (kilocalories, kcal)

Protein

Minimum

50 grams (g)

Vitamin D

Minimum

20 micrograms (mcg)

Calcium

Minimum

1,300 milligrams (mg)

Iron

Minimum

18 milligrams (mg)

Potassium

Minimum

4,700 milligrams (mg)

Set this up as a standard linear programming problem with decision variables taking any non-negative values. In other words, partial servings are permitted.  

For nutritional constraints, consider setting these to satisfy a weekly diet. That is, multiply each daily requirement by seven (7).

(Optional) Add an eighth nutritional constraint that is especially relevant to anyone interested in weight control. Define the maximum number of Energy/Calories to be consumed each day, and multiply that daily requirement by seven (7).

Nutrition labels on packaged foods should contain information about these eight components of nutrition along with other components. Each of the components represents a constraint in the linear programming problem you are developing.

To adapt the problem to your personal diet, collect nutrition facts from five packaged food items in your household. Use packaged foods that are part of your normal diet and for which you have prices. Also, ensure that the across the set of food items there are positive values for each of the eight components of nutrition. Adjust the price for each food item so that it represents one serving size, as defined on the nutrition facts label. Each food item represents a decision variable in the linear programming problem.

The goal or objective of this problem is to find the minimum-cost diet (servings of food items) that satisfies the eight nutritional requirements. Use Python PuLP or AMPL (perhaps with its Python API). 

Deliverables (150 points total, 30 points for each part)

Your git repository should have files that can be viewed in Visual Studio Code after the cloning of the repository.  Files with these extensions should work fine:  py, txt, csv, json, png, jpg, md, and pdf.  Export or convert proprietary Microsoft Office files to readable formats for inclusion in the repository: (xlsx to csv, doc and pptx to pdf).

Paper (pdf file in GitHub repository). The paper/write-up should be submitted as a pdf file (two pages max for text, appendices for tables, figures, and images do not count in the two-page max). Think of the paper as comprising the methods and results sections of a written research report. If you like, provide a paragraph on methods and a paragraph about results for each of the five parts of this assignment. As this is an individual assignment about your personal eating habits, it is fine to use the first person in writing this paper. 

Program code (text link/URL to GitHub repository). Key information from the paper should also be included in the README.md markdown file of a public GitHub repository established by the student for this assignment. The GitHub repository should include text files for the program code, and program output, Image files (.jpg or .png extension) should be included for the scanned food labels may also be included in the repository. Include the web address text (URL) for the GitHub repository in the comments form of the assignment posting.  You should be providing a link to a separate repository that can be cloned. It should end with the .git extension.

This assignment has five graded components, with each component worth 30 points:

Part 1. Provide documentation for the five packaged food items you have selected for the assignment. Photographs of the Nutrition Facts labels are sufficient. Show your price calculations for serving sizes. [If you cook meals for yourself and prefer not to use packaged food items in this assignment, see the Assignment Addendum below.]
Part 2. Specify the linear programming problem in standard form, showing decision variables, objective function with cost coefficients, and weekly nutritional constraints. Describe the problem in plain English. Implement the linear programming problem using Python PuLP or AMPL. Provide the program code and output/listing as plain text files, posting within a GitHub repository dedicated to this assignment. 
Part 3. Solve the linear programming problem using your Python PuLP or AMPL code. Describe the solution, showing units (serving sizes) for each of the five food items. What is the minimum cost solution? How much would you need to spend on food each week? Include the text file (listing) of your solution in the GitHub repository.
Part 4. Solutions to the diet problem are notorious for their lack of variety. Suppose you require at least one serving of each food item or meal during the week, setting constraints in the diet problem accordingly. Solve the revised linear programming problem. How do these additional constraints change the solution? How much more would you have to spend on food each week? Include the text file (listing) of your solution of this revised problem in the GitHub repository. Suppose this diet solution continues to lack variety. Describe how could you add further variety to your diet by making additional revisions to the model specification.
Part 5. Large language models (LLMs), as implemented with ChatGPT, Gemini 2.0 Flash, or other generative AI systems, are being used to solve many problems in data science. Select an LLM-based service or agent with which to work. Pick a free plan or one that is freely available to Northwestern students. (Do not pay for services in completing this assignment.) Indicate which service you have selected, providing its web address or uniform resource locator (URL). See if you can get your selected LLM agent to specify a model for The Diet Problem. See to what extent you can get the agent to develop computer code for The Diet Problem. Report on your success or failure. Provide a step-by-step review of your work. What prompts did you use? How did the conversation with the LLM agent go? Were you able to build on the conversation or to tailor it to your specific needs? As part of the GitHub repository for this assignment, include a plain text file of the complete conversation that you had with the LLM agent. Comment on your experience. Could an LLM agent be used to complete this assignment?
Assignment Addendum. What if you prefer to cook for yourself rather than use packaged food items? This is OK. After all, the first assignment is intended to be relevant to you and your diet. But if you cook for yourself, you have more work to do in setting up the problem than students who use packaged goods.

When the assignment refers to a packaged good item and one serving the item, think of one-serving meal from the menu of ingredients you would use for that one-serving meal. Use your knowledge of the cost of the ingredients and the nutrients in those ingredients in the measures required in the recipe for each mean/serving. You may have to do research to get these values.

For each meal/serving, you need to sum across the ingredient costs to get the meal costs, and you need to sum across the ingredient nutrient contributions to get the nutrient contributions.

If you take this cook-for-yourself approach, be sure to document your recipes, as well as your calculations of meal/serving costs and meal/serving nutrient contributions. You can provide these calculations in an appendix to your written report in lieu of providing photographs of nutrient contributions from packaged goods.

References

Dantzig, George B. 1990. “The Diet Problem.” Informs. 20:4, 43–47. Available on Course Reserves.

Food and Drug Administration, Department of Health and Human Services. 2016. Food Labeling: Revision of the Nutrition and Supplemental Facts Labels. Available at https://s3.amazonaws.com/public-inspection.federalregister.gov/2016-11867.pdfLinks to an external site.

Fourer, Robert, David M. Gay, and Brian W. Kernighan. 2003. AMPL: A Modeling Language for Mathematical Programming (second edition). Belmont, CA: Brooks/Cole. [ISBN-13: 978-0-534-38809-6] Chapter 2, Diet and Other Input Models: Minimizing Costs, pages 27–42. Available onlineLinks to an external site..(https://ampl.com/wp-content/uploads/BOOK.pdf) Check out the Lex Fridman interview from July 2020: Brian Kernighan on UNIX, C, AWK, AMPL, and Go ProgrammingLinks to an external site..
Mente, Andrew, Martin O'Donnell, and Salim Yusuf. 2021, September. "Sodium Intake and Health: What Should We Recommend Based on the Current Evidence?" Nutrients, 13(9): 3232. Available online at https://www.mdpi.com/2072-6643/13/9/3232Links to an external site. . This is part of the September 2021 special issue of Nutrients: "Towards Better Dietary Guidelines: New Approaches Based on Recent Science."  

Stigler, George. 1945. “The Cost of Subsistence.” Journal of Farm Economics, 25:2, 303–314. Available online at https://math.berkeley.edu/~mgu/MA170/Diet.pdfLinks to an external site.

van Dooren, Corné. 2018, June. “A Review of the Use of Linear Programming to Optimize Diets, Nutritiously, Economically and Environmentally.” Frontiers in Nutrition, 4, Article 48. Available online at https://www.frontiersin.org/articles/10.3389/fnut.2018.00048/fullLinks to an external site.
