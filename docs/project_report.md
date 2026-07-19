# Comprehensive Analysis and Dietary Strategies with Tableau

## A College Food Choices Case Study

## Team Members

| Name | Role |
|---|---|
| Undrakonda Avinash Sai | Team Lead |
| Madagala Chaitanya Sravanthi | Member |
| CHAITHANYA GUPTHA PADMANABUNI | Member |
| Samminga Prema Raju | Member |
| Burreddy Shanmukha Veera Sai | Member |

## 1. Introduction

This project presents a data analytics case study on college students' food choices, dietary habits, lifestyle patterns, and health-related behaviors. The analysis was completed using Tableau to convert raw survey data into meaningful visual insights. The project helps identify how breakfast habits, comfort food reasons, exercise, cooking frequency, eating out, fruit and vegetable intake, vitamin usage, and food preferences relate to student health and wellbeing.

## 2. Problem Statement

College students often experience irregular schedules, academic pressure, limited budgets, and changing lifestyle habits. These factors can lead to skipped meals, unhealthy snacking, frequent eating out, low fruit and vegetable intake, and comfort-food consumption due to boredom or stress. The purpose of this project is to analyze these behaviors and recommend practical dietary strategies for healthier student living.

## 3. Objectives

- To analyze college students' food choice patterns using Tableau.
- To study the relationship between diet habits and health category.
- To compare breakfast habits, cooking frequency, eating out, and comfort food reasons.
- To identify food preference trends among students.
- To build an interactive Tableau dashboard and story for easy interpretation.
- To suggest practical dietary strategies for students and campus food services.

## 4. Dataset Description

The dataset used in this project is stored as `data/college_food_choices_final.csv`. It contains 120 student records and 41 variables. The major fields include student ID, gender, grade level, GPA, weight, breakfast, calories per day, calorie awareness, healthy feeling, life rewarding score, comfort food reason, cooking frequency, eating out frequency, exercise, fruit intake, vegetable intake, vitamin usage, cuisine preferences, current diet, and health category.

## 5. Tools and Technologies Used

- Tableau Public/Desktop for data visualization
- CSV dataset for structured data analysis
- GitHub for project submission and version control
- Flask website scaffold for presenting or embedding the Tableau dashboard

## 6. Data Preparation

The data preparation process included checking column names, validating data types, standardizing categorical values, and confirming that the dataset was ready for Tableau import. Numeric survey-scale fields were maintained as numeric values, while categorical fields such as gender, breakfast type, comfort food reason, favorite cuisine, current diet, and health category were treated as dimensions.

## 7. Tableau Workbook

The Tableau workbook is available in the project folder as `tableau/Food_Choice_Analysis.twb`. It connects to the cleaned dataset and supports dashboard creation for the College Food Choices case study.

Calculated fields used in Tableau:

### Consumption

```tableau
IF [Parameter 2] = "veggies_day" THEN [veggies_day]
ELSEIF [Parameter 2] = "vitamins" THEN [vitamins]
ELSE [fruit_day]
END
```

### Food Selection

```tableau
IF [Parameter 3] = "thai_food" THEN [thai_food]
ELSEIF [Parameter 3] = "italian_food" THEN [italian_food]
ELSEIF [Parameter 3] = "persian_food" THEN [persian_food]
ELSEIF [Parameter 3] = "greek_food" THEN [greek_food]
ELSE [indian_food]
END
```

## 8. Visualizations Created

The project includes the following Tableau visualizations:

- KPI summary showing student count, average GPA, average weight, and average grade level
- Breakfast consumption chart
- Eating out versus cooking frequency analysis
- Health category by gender chart
- Vitamins, fruit, and vegetable consumption comparison
- Health category versus food preference analysis
- Healthy feeling and life rewarding score visualization
- Weight versus exercise frequency analysis
- Comfort food reasons visualization

## 9. Dashboard Description

The main dashboard, titled Food Choice Analysis, combines important charts into one interactive view. It helps users quickly understand student eating patterns, health categories, food preferences, comfort-food behavior, and lifestyle indicators. Parameter controls allow the user to switch between different consumption and cuisine preference measures.

## 10. Key Insights

- Breakfast habits are an important indicator of student dietary routine.
- Comfort-food consumption is commonly connected with boredom, sadness, or stress.
- Students who cook more frequently may have better control over their food choices.
- Eating out frequency can indicate possible dependence on fast food or convenience meals.
- Fruit, vegetable, and vitamin consumption patterns show opportunities for nutrition awareness.
- Health category differences help identify groups that may benefit from targeted dietary guidance.

## 11. Recommendations

- Encourage students to eat simple and nutritious breakfasts.
- Promote affordable balanced meal options in college cafeterias.
- Increase awareness about fruit, vegetable, and vitamin intake.
- Provide healthier alternatives for comfort-food cravings.
- Conduct nutrition awareness programs for students.
- Improve cafeteria menus with calorie-aware and balanced meal labels.
- Encourage cooking skills and simple home-style meal preparation among students.

## 12. Conclusion

This project demonstrates how Tableau can be used to convert student food-choice data into useful insights. The dashboard and story help explain dietary patterns, lifestyle habits, and health-related trends among college students. The analysis supports practical dietary strategies that can improve student wellness, food awareness, and healthier decision-making.

## 13. Project Files

- Dataset: `data/college_food_choices_final.csv`
- Tableau workbook: `tableau/Food_Choice_Analysis.twb`
- Tableau build guide: `tableau/tableau_build_guide.md`
- Project report: `docs/project_report.md`
- Video script: `docs/video_script.md`
