# msds_460_assignment_one
Diet Problem Individual Assignment for Northwestern MSDS 460 course, assignment description below. This assignment will sit in the msds_460_assignment_one repository of olealberto

## Repository Files:
images of packaging can be found in food_label_images folder

diet_problem_python_lpmodel contains the python code used to solve this linear programming model

Diet Problem Write Up - Albert Olea is a pdf that contains the write up of answers as well as table figures from food packaging

ChatGPT Diet Problem Solution.txt details a conversation with an LLM to try and solve this diet problem part 5 




### The Diet Problem Revisited (version 11)

Developed by Thomas W. Miller. Revised January 9, 2025.

Introduced by Stigler (1945) and discussed by Dantzig (1990), the diet problem is a classic problem in constrained optimization often used to introduce linear programming concepts. The diet problem has been studied extensively through the years (van Dooren 2018).

For this assignment, you need to construct a personalized diet using current recommended dietary allowances from the U.S. Food and Drug Administration, updated to account for recent research on sodium intake and health (Mente, O'Donnell, and Yusuf 2021). Interested in learning more about nutrition and healthy living? Check out Nutrients, an open-access journal, at its home page https://www.mdpi.com/journal/nutrientsLinks to an external site. .

The constraints for this linear programming problem, should consider seven components of nutrition and their daily values, as shown in the following table:

Component Max/Min Daily Amount and measure

Sodium Maximum 5,000 milligrams (mg)

Energy Minimum 2,000 Calories (kilocalories, kcal)

Protein Minimum 50 grams (g)

Vitamin D Minimum 20 micrograms (mcg)

Calcium Minimum 1,300 milligrams (mg)

Iron Minimum 18 milligrams (mg)

Potassium Minimum 4,700 milligrams (mg)

Set this up as a standard linear programming problem with decision variables taking any non-negative values. In other words, partial servings are permitted.  

For nutritional constraints, consider setting these to satisfy a weekly diet. That is, multiply each daily requirement by seven (7).

(Optional) Add an eighth nutritional constraint that is especially relevant to anyone interested in weight control. Define the maximum number of Energy/Calories to be consumed each day, and multiply that daily requirement by seven (7).

Nutrition labels on packaged foods should contain information about these eight components of nutrition along with other components. Each of the components represents a constraint in the linear programming problem you are developing.

To adapt the problem to your personal diet, collect nutrition facts from five packaged food items in your household. Use packaged foods that are part of your normal diet and for which you have prices. Also, ensure that the across the set of food items there are positive values for each of the eight components of nutrition. Adjust the price for each food item so that it represents one serving size, as defined on the nutrition facts label. Each food item represents a decision variable in the linear programming problem.

The goal or objective of this problem is to find the minimum-cost diet (servings of food items) that satisfies the eight nutritional requirements. Use Python PuLP or AMPL (perhaps with its Python API). 

Deliverables (150 points total, 30 points for each part)

This git repository has files that can be viewed in Visual Studio Code after the cloning of the repository.  Files with these extensions should work fine:  py, txt, csv, json, png, jpg, md, and pdf.  Export or convert proprietary Microsoft Office files to readable formats for inclusion in the repository: (xlsx to csv, doc and pptx to pdf).

Paper (pdf file in GitHub repository). The paper/write-up should be submitted as a pdf file (two pages max for text, appendices for tables, figures, and images do not count in the two-page max). Think of the paper as comprising the methods and results sections of a written research report. If you like, provide a paragraph on methods and a paragraph about results for each of the five parts of this assignment. As this is an individual assignment about your personal eating habits, it is fine to use the first person in writing this paper. 

Program code (text link/URL to GitHub repository). Key information from the paper should also be included in the README.md markdown file of a public GitHub repository established by the student for this assignment. The GitHub repository should include text files for the program code, and program output, Image files (.jpg or .png extension) should be included for the scanned food labels may also be included in the repository. Include the web address text (URL) for the GitHub repository in the comments form of the assignment posting.  You should be providing a link to a separate repository that can be cloned. It should end with the .git extension.

